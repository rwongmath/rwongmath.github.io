---
school: UCLA
number: Math 115A
coursetitle: Linear Algebra
title: Math 115A&#58; Linear Algebra

layout: single

toc: true
toc_label: "Content"
toc_icon: "atlas"

23Spring: true
---


{% capture syllabus %}assets/syllabus/{{ page.number | split: " " | first }}_{{ page.number | split: " " | last }}_Syllabus.pdf{% endcapture %}

You can find the [course syllabus here]({{ syllabus | relative_url }}).

**What does it mean to prove a theorem?**  Why are the theorems you saw in Math 33A true?  How do we generalize the properties of $\mathbb{R}^n$ as a vector space over $\mathbb{R}$?

115A is the *second* course in linear algebra.  In math 33A, you learned the computational tools of linear algebra in $\mathbb{R}^n$. In math 115A, you will learn how to prove the theorems and tools you saw in 33A.  Moreover, you will generalize these theorems to the setting of abstract vector spaces.

115A may also be your first exposure to mathematical proofs.  In other words, this course will help you develop the mathematical reasoning and questioning skills needed to explore abstract mathematical concepts. Moreover, you will become fluent in communicating your mathematical ideas, and you will develop the ability to prove (or find counterexamples) to mathematical statements. 

This course provides the foundation for exploring other topics in advanced mathematics.


<!--end_excerpt-->

# Schedule

|  | Learning Outcome      | Textbook Section |      Lectures|                                                        
| ---| ----------------------------         | ------ | ------------------------------------------------------------ |
{% for objective in site.data.Math_115A_Learning_Objectives -%}
  | {{ objective.number }} | <b>{{ objective.name }}</b>. {{ objective.description }} | {{ objective.textbook }} | {{ objective.lectures }} |
{% endfor %}



# Learning Objectives: 

The goals of the course are that you: 

* Acquire an understanding of the geometry of Euclidean space, linear transformations, and the differential calculus of multivariable functions.
* Develop the reasoning and questioning skills needed to explore these (mathematical) topics and apply them to real-life situations.
* Develop the collaboration and communication skills needed to convey your (mathematical) ideas.

Below you will find the explicit learning objectives associated to each of these goals.

## Linear Algebra Objectives (LA)

<ol>
{% for objective in site.data.Math_115A_Learning_Objectives %}
  <li> <b>{{ objective.name }}</b>. {{ objective.description }}
  </li>
{% endfor %}
</ol>

## Mathematical Reasoning Objectives (MR)
0. **Reason abstractly and quantitatively.**  Use mathematics to model real-world situations and to interpret and solve problems.  Make appropriate assumptions and approximations to simplify a complicated situation. Draw pictures or study examples to provide insight.  Attend to the meaning of quantities instead of just computing them. Consider the units involved.
0. **Make sense of problems and persevere in solving them.**  Understand what a problem is asking for. Analyze the givens, constraints, and goals of a problem. Break large/complex problems into smaller/simpler problems. Check answers using alternate methods.
0. **Build intuition.**  Investigate and create specific examples and counterexamples. Look for and make use of structure or repeated patterns. Look for both general methods and shortcuts.  Seek to understand unexpected results.
0. **Use appropriate tools strategically.**  Consider the available tools when solving a mathematical problem. Understand and use stated assumptions, definitions, and previously established results.
0. **Construct viable arguments.**  Make conjectures, and use assumptions, definitions, and/or previously established results to prove or disprove them. Use strategies such as direct proofs, contrapositive statements, proof by cases, or proof by contradiction.
0. **Be creative and explore mathematics.** Do more than find a solution. Look for novel or elegant solutions. See what changes when you add, change, or weaken hypotheses. Draw connections between topics and ideas.

## Mathematical Communication Objectives (MC)
0. **Ask questions.**  Notice, identify, and clarify sources of confusion. Look for connections and relationships between ideas. Explore topics and ideas deeply.
0. **Use and develop mathematical fluency.**  Use standard mathematical notations and terms (as discussed in class or demonstrated in course materials).  Clearly indicate and explain any use of non-standard shorthand, notation, or tools.
0. **Analyze and constructively critique the reasoning of others.**  Actively listen and summarize key ideas to check comprehension. Test conjectures against examples and potential counterexamples. Assess and reconcile various approaches to problems. Work together to find errors and fix flaws.
0. **Explain and justify your reasoning.**  Communicate and justify your conclusions to others. Indicate the general strategy or argument, and identify the key step or idea(s). Listen and reflect to the critiques of others.  Work together to find errors and fix flaws.
0. **Attend to precision.**  Communicate precisely to others. Use clear definitions, and carefully state any assumptions or results used.  Be able to explain heuristics/arguments in depth.
0. **Be clear and concise.**  se the appropriate amount of generality or specificity in arguments.  Avoid use of any extraneous assumptions, hypotheses, or statements. Indicate any figures or examples that you have in mind.
0. **Review, reflect, and revise.** Review previous work and assess the positives and negatives. Reflect on your strategies and look for ways to improve. Use feedback to grow and develop your mathematical reasoning or communication skills.