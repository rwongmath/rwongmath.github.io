---
school: UCLA
number: Math 94
coursetitle: Explorations of Mathematics in the Physical World
title: Math 94&#58; Explorations of Mathematics in the Physical World

layout: single

toc: true
toc_label: "Content"
toc_icon: "atlas"

23Summer: true
---


{% capture syllabus %}assets/syllabus/{{ page.number | split: " " | first }}_{{ page.number | split: " " | last }}_Syllabus.pdf{% endcapture %}

You can find the [course syllabus here]({{ syllabus | relative_url }}).

**How can we describe the physical world mathematically?**  How can we use mathematics to describe phenomena in physics, chemistry, or other STEM fields?  How should we think about and interpret mathematical formulas?

Mathematics is a language that allows us to describe the geometry of the physical world around us, such as estimating the number of candies in a jar, the trajectory of a baseball, the behavior of chemical reactions, or the amount of water flowing out of a bottle. 

In this course, you will develop the reasoning and questioning skills needed to explore these calculus concepts and apply them to real-life and STEM situations.  Moreover, you will become fluent in communicating your ideas through the language of mathematics.


<!--end_excerpt-->

<hr>

# Schedule

|  | Learning Outcome      |      Week|                                                        
| ---| ----------------------------       | ------------------------------------------------------------ |
{% for objective in site.data.Math_94_Learning_Objectives -%}
  | {{ objective.number }} | <b>{{ objective.name }}</b>. {{ objective.description }}  | {{ objective.week }} |
{% endfor %}

<hr>
# Learning Objectives: 
<div class="standout" markdown="1">


The goals of the course are that you: 

* Develop the reasoning and questioning skills needed to explore STEM topics.
* Develop the reasoning and questioning skills needed to explore these (mathematical) topics and apply them to real-life situations.
* Develop the collaboration and communication skills needed to convey your (mathematical) ideas.

Below you will find the explicit learning objectives associated to each of these goals.
</div>


## Summer Bridge Objectives (B)
<div class="standoutlist" markdown="1">
<ol>
{% for objective in site.data.Math_94_Learning_Objectives %}
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