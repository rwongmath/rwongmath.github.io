---
school: UCLA
number: Math 32AH
coursetitle: Calculus of Several Variables, Honors
title: Math 32AH&#58; Calculus of Several Variables, Honors

layout: single

toc: true
toc_label: "Content"
toc_icon: "atlas"

21Fall: true
22Fall: true
23Fall: true
---


{% capture syllabus %}assets/syllabus/{{ page.number | split: " " | first }}_{{ page.number | split: " " | last }}_Syllabus.pdf{% endcapture %}

You can find the [course syllabus here]({{ syllabus | relative_url }}).

You can view the **[course lecture notes](https://github.com/rwongmath/HonorsMultivariableCalculus/blob/main/HonorsMultivariableCalculus.pdf)** for 32AH here.

**How can we describe the physical world mathematically?** What changes, and what stays the same when we move from single variable calculus to multivariable calculus?  What does it mean to take a derivative of a multivariable function?

Multivariable calculus is the mathematical language that allows us to describe the geometry of the physical world around us, such as the motion of planets in orbit, the behavior of electromagnetic forces, or the path of steepest ascent through the hills of Los Angeles. In this course, you will develop the reasoning and questioning skills needed to explore these geometric concepts and apply them to real-life situations.  Moreover, you will become fluent in communicating your ideas through the mathematical language of multivariable calculus.

The course 32AH differs from 32A in that it covers the topics of multivariable calculus with more mathematical rigor.  Moreover, it builds the foundation for more advanced topics, such as linear algebra, real analysis, and differential geometry. 

This course is recommended for students interested in learning about advanced mathematics. 

<!--end_excerpt-->

<hr>

# Schedule

|  | Learning Outcome      | Textbook Section |      Lectures|                                                        
| ---| ----------------------------         | ------ | ------------------------------------------------------------ |
{% for objective in site.data.Math_32AH_Learning_Objectives -%}
  | {{ objective.number }} | <b>{{ objective.name }}</b>. {{ objective.description }} | {{ objective.textbook }} | {{ objective.lectures }} |
{% endfor %}


<div class="standout" markdown="1">
# Learning Objectives: 

The goals of the course are that you: 

* Acquire an understanding of the geometry of Euclidean space, linear transformations, and the differential calculus of multivariable functions.
* Develop the reasoning and questioning skills needed to explore these (mathematical) topics and apply them to real-life situations.
* Develop the collaboration and communication skills needed to convey your (mathematical) ideas.

Below you will find the explicit learning objectives associated to each of these goals.
</div>

## Multivariable Calculus Objectives (MV)
<div class="standoutlist" markdown="1">
<ol>
{% for objective in site.data.Math_32AH_Learning_Objectives %}
  <li> <b>{{ objective.name }}</b>. {{ objective.description }}
  </li>
{% endfor %}
</ol>
</div>

## Mathematical Reasoning Objectives (MR)

<div class="standoutlist" markdown="1">
0. **Reason abstractly and quantitatively.**  Use mathematics to model real-world situations and to interpret and solve problems.  Make appropriate assumptions and approximations to simplify a complicated situation. Draw pictures or study examples to provide insight.  Attend to the meaning of quantities instead of just computing them. Consider the units involved.
0. **Make sense of problems and persevere in solving them.**  Understand what a problem is asking for. Analyze the givens, constraints, and goals of a problem. Break large/complex problems into smaller/simpler problems. Check answers using alternate methods.
0. **Build intuition.**  Investigate and create specific examples and counterexamples. Look for and make use of structure or repeated patterns. Look for both general methods and shortcuts.  Seek to understand unexpected results.
0. **Use appropriate tools strategically.**  Consider the available tools when solving a mathematical problem. Understand and use stated assumptions, definitions, and previously established results.
0. **Construct viable arguments.**  Make conjectures, and use assumptions, definitions, and/or previously established results to prove or disprove them. Use strategies such as direct proofs, contrapositive statements, proof by cases, or proof by contradiction.
0. **Be creative and explore mathematics.** Do more than find a solution. Look for novel or elegant solutions. See what changes when you add, change, or weaken hypotheses. Draw connections between topics and ideas.
</div>

## Mathematical Communication Objectives (MC)
<div class="standoutlist" markdown="1">
0. **Ask questions.**  Notice, identify, and clarify sources of confusion. Look for connections and relationships between ideas. Explore topics and ideas deeply.
0. **Use and develop mathematical fluency.**  Use standard mathematical notations and terms (as discussed in class or demonstrated in course materials).  Clearly indicate and explain any use of non-standard shorthand, notation, or tools.
0. **Analyze and constructively critique the reasoning of others.**  Actively listen and summarize key ideas to check comprehension. Test conjectures against examples and potential counterexamples. Assess and reconcile various approaches to problems. Work together to find errors and fix flaws.
0. **Explain and justify your reasoning.**  Communicate and justify your conclusions to others. Indicate the general strategy or argument, and identify the key step or idea(s). Listen and reflect to the critiques of others.  Work together to find errors and fix flaws.
0. **Attend to precision.**  Communicate precisely to others. Use clear definitions, and carefully state any assumptions or results used.  Be able to explain heuristics/arguments in depth.
0. **Be clear and concise.**  se the appropriate amount of generality or specificity in arguments.  Avoid use of any extraneous assumptions, hypotheses, or statements. Indicate any figures or examples that you have in mind.
0. **Review, reflect, and revise.** Review previous work and assess the positives and negatives. Reflect on your strategies and look for ways to improve. Use feedback to grow and develop your mathematical reasoning or communication skills.
</div>