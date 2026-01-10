---
title: "A quick primer on modifying existing LaTeX for digital accessibility"
layout: single
categories:
tags:
  - Rice
---

I have been working on making my course materials (e.g. worksheets, syllabi, slides) digitally accessible over winter break.  

This post is a guide to the packages, commands, and other tweaks that I have compiled from across various sources to make my existing TeX files compile correctly as tagged pdfs.  This post should be thought of as a supplement to [the Tagging Project](https://latex3.github.io/tagging-project/)'s  [Guidelines for using LaTeX to generate accessible PDF](https://latex3.github.io/tagging-project/documentation/usage-instructions).

Sample tex files and materials are [included below](#sample-materials), and I have [checked that they are parsed correctly by VoiceOver](https://webaim.org/articles/voiceover/) (Apple's built-in screen reader), and also pass the tests on my LMS (Canvas,  Ally Course Accessibility Report).  

**DISCLAIMER:** I am not an expert on accessibility nor an expert in the inner workings of TeX, and this post is not legal advice, nor it is a guarantee that your documents will automatically satisfy any or all accessibility standards or legal regulations.  

<!--end_excerpt-->

# Context

If you are interested in learning more about digital accessibility in regards to mathematics, a good reference to get acquainted is [Accessibility for the Working Mathematician](https://arxiv.org/abs/2505.22667) by Julius Ross.  

The tl;dr is that making documents accessible takes work, beyond the challenge of **writing appropriate alt text** (see sections 3.2-3.4).  It may also require philosophical changes in **how you structure your documents** (see section 3.5).  You may also need to **remove or replace certain classes or packages** (for example, `beamer` cannot create tagged pdfs, and will need to be replaced by [`ltx-talk`](https://ctan.org/pkg/ltx-talk)).

My understanding is that if you were to start from scratch, many experts are recommending how to compose documents using a system that can create both HTML and pdf (and other) outputs such as [Ximera](https://ximera.osu.edu/) or [PreTeXt](https://pretextbook.org/).  

I will probably learn PreTeXt over the summer, and I definitely see the value in writing HTML output.  However, I think there is value in having accessible pdfs because they are documents that can be downloaded and used by people without a stable or reliable internet connection (or [when Canvas goes down](https://www.wired.com/story/the-aws-outage-was-a-nightmare-for-college-students/)).

---

Below are the modifications you will need to create digitally accessible pdfs from  your TeX files.  You can see [sample TeX files](#sample-materials) below.

# 1. Change your compiler to LuaLaTeX and update your TeX version

LuaLaTeX is recommended by the tagging project; but the packages and commands detailed below should work with pdfLaTeX.  After switching to using LuaLaTeX, I saw no difference in compile times for the documents I am working on.

You should also make sure that you have the latest version of TeX installed (currently LaTeX 2025-11-01 as of this post).  This is important for new classes and packages being developed, such as [`ltx-talk`](https://ctan.org/pkg/ltx-talk?lang=en).

If you use Overleaf, [here are instructions on how to change compiler and TeX version](https://docs.overleaf.com/getting-started/recompiling-your-project/selecting-a-tex-live-version-and-latex-compiler).

**Note:** the distribution of TeX used by overleaf (TexLive 2025) is not as up to date as the latest distribution of TeX (e.g. it does not yet have support for `ltx-talk`, but you can opt into the [Overleaf Labs program](https://www.overleaf.com/labs/participate) for access to newer versions of TeX).

# 2. Turn on tagging

To create tagged pdfs from your TeX files, you should include this code in the preamble (e.g. before `\begin{document}`): 

```
\DocumentMetadata{
  tagging=on,
  tagging-setup={math/setup=mathml-SE,math/alt/use}
}
```

The `tagging-setup={math/setup=mathml-SE,math/alt/use}` option turns on the necessary code for screenreaders to read mathematics (see [below](#4-create-alt-text-for-equations)).

This command has other options - you can set the language (which is US English by default), the PDF standard, etc.

[See the documentation for `\DocumentMetadata` here](https://texdoc.org/serve/documentmetadata-support-code.pdf/0).



# 3. Set up the title & author

To set the title and author of the PDF, you should include this code in the preamble:

```
\usepackage{hyperref}
```


and you should include this code in the body of the document (e.g. immediately after `\begin{document}`) 

```
\hypersetup{
pdftitle={Spring 2026 Math 102 Syllabus},
pdfauthor={Richard Wong},
pdfdisplaydoctitle%
}
```


# 4. Create alt text for equations

The tagging project renders math formulas and equations using MathML, but some screenreaders (e.g. VoiceOver, Ally) treats them like images which require alt text.

The option `tagging-setup={math/setup=mathml-SE,math/alt/use}` in the `\DocumentMetaData` command [described above](#2-turn-on-tagging) will automatically generate the alt text via the latex commands used.  For example, the formula  $\displaystyle \int_0^1 xe^{-x^2} \ dx$ has alt text 

> Latex formula starts `\begin{math} \int_0^1 xe^{-x^2} \ dx \end{math}` Latex formula ends

This setup also allows screen readers to "dig in" and navigate these formulas (e.g. one can move back and forth between the bounds of integration, or different parts of the integrand).

**Note:** Because the alt text currently repeats verbatim the latex commands used, you should be careful about the macros that you use.


[See the documentation for math content here](https://texdoc.org/serve/latex-lab-math/0).



# 5. Create alt text for images

Adding alt text to images is easy - simply use the alt-text options in `\includegraphics`:

```
\includegraphics[alt={A picture of me and Ernie}]{ernie_mueller2020.jpg} 
```


However, in my opinion, **_writing_ appropriate alt text** is the most difficult part of making your documents accessible.

Especially in the context of teaching, writing alt text requires you to think carefully about the pedagogical intent of the image. (see [Ross 3.2-3.4](https://arxiv.org/abs/2505.22667)) 

THe AMS, EMS, LMS, and SIAM also recently published [Author Guidelines for Preparing Accessible Mathematics Content](https://epubs.siam.org/pb-assets/author_guidelines_accessible_mathematics.pdf), which set standards for labeling complex math diagrams (with examples).

# 6. Label table headers

To indicate the headers of the table, you can include this code immediately before the relevant table:

```
\tagpdfsetup{table/header-rows={1}}
```


[See the documentation for tables here](https://texdoc.org/serve/latex-lab-table/0).


# 7. Check headings and navigation

This is another challenge of making accessible documents - you should make sure that your existing documents use headings (e.g. `\section` or `\subsection`, etc.) appropriately.

That is, you should make sure your document does not use purely visual commands (e.g. `\textbf`, `\Large`, etc.) to indicate headings or sections.

Otherwise, the command `\DocumentMetadata` [described above](#2-turn-on-tagging) will take care of the tagging.




# 8. Check package compatibility

If you are still encountering errors (which is likely), you should check package compatibility with [the Tagging Project's compatibility tracker](https://latex3.github.io/tagging-project/tagging-status/).  

A lot of packages are currently supported, but some packages are not supported yet (for example, packages like `titlesec`).

Other packages will never be supported due to the way the package works (e.g. `beamer`).  In that case, you should look to alternatives (e.g. `ltx-talk`).

# Sample Materials

A worksheet for the second day of Calc II:

- [tex file](/assets/materials/02_mad_minute.tex)
- [tagged pdf](/assets/materials/02_mad_minute.pdf)

A syllabus for Calc II:

- [tex file](/assets/materials/Math_102_Syllabus.tex)
- [tagged pdf](/assets/syllabus/Math_102_Syllabus.pdf)