---
permalink: /research/
title: "Research"

layout: single

toc: true
toc_label: "Content"
toc_icon: "journal-whills"

---

{% assign update = site.data.lastupdated %}
{% assign statement = site.static_files | where: "basename", "Richard_Wong_Research_Statement" | first %}

> "In mathematics, the art of asking questions is more valuable than solving problems."

<cite>--- [Georg Cantor](https://en.wikipedia.org/wiki/Georg_Cantor)</cite>
{: .small} 

My research interests are in computations in **equivariant stable homotopy theory**. The study of homotopy theory originates in algebraic topology, with the investigation of algebraic invariants such as (co)homology groups or homotopy groups. By passing from topological spaces to spectra, one can further study *stable* invariants, and in the presence of a group action, one can study *equivariant* invariants as well.

While homotopy theory has its origins in algebraic topology, its core tools and ideas have spread and found use in other areas of mathematics. In my research, I apply the computational methods of homotopy theory to answer questions about the **modular representation theory of finite groups**.

My **[Research Statement](/assets/Richard_Wong_Research_Statement)** can be found here (last updated {{ update.research }}).

[Click here for a brief, non-technical statement](/research/nontechnical) of my research interests, as well as an undergraduate level introduction to stable homotopy theory.

<!--end_excerpt-->

<hr>
<div class="standout" markdown="1">

# Papers/Preprints

{% include /list_papers.md %}

I gave a talk on this paper at the Workshop on Homotopy Theory and Group Theory at CRM Barcelona. The [video recording is available](https://youtu.be/z2Svytb7LkI).

</div>

<hr>

# Future Directions

In my research, I apply the computational methods of homotopy theory to answer questions about the **modular representation theory** of finite groups G over a field of characteristic p, where p divides the order of the group. One particvular problem of interest is in computing the **group of endo-trivial modules**.

Modular representation theory was revolutionized by a focus on an invariant denoted StMod(kG), the *stable module category of G*. Notably, StMod(kG) has a homotopy-theoretic interpretation as a stable symmetric-monoidal ∞-category. Correspondingly, the group of endo-trivial modules is intepreted as the **Picard group of the stable module category**, which consists of objects in StMod(kG) that are invertible with respect to the tensor product.

For p-groups, this group of endo-trivial modules was originally computed by work of Carlson-Thévenaz using group cohomology and the theory of support varieties. However, in joint work with van de Meer, I provide new, homotopical proofs for their results for cyclic p-groups and (generalized) quaternion groups using the descent ideas of Mathew-Stojanoska. This provides new insights into the classical representation-theoretic proofs of Carlson-Thévenaz.

In future work, I propose to construct and compute homotopy invariants that have representation-theoretic significance. In particular, I am interested in (1) using homotopy theory to compute endo-trivial modules for other classes of groups, (2) studying other invariants of StMod(kG), and (3) computing endo-trivial modules for variants of StMod(kG) coming from tensor-triangular geometry.