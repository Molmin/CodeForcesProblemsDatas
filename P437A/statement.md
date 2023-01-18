## Description

<div><p>Once upon a time a child got a test consisting of multiple-choice questions as homework. A multiple-choice question consists of four choices: <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span>, <span class="tex-font-style-tt">C</span> and <span class="tex-font-style-tt">D</span>. Each choice has a description, and the child should find out the only one that is correct.</p><p>Fortunately the child knows how to solve such complicated test. The child will follow the algorithm:</p><ul> <li> If there is some choice whose description at least twice shorter than all other descriptions, or at least twice longer than all other descriptions, then the child thinks the choice is great. </li><li> If there is exactly one great choice then the child chooses it. Otherwise the child chooses <span class="tex-font-style-tt">C</span> (the child think it is the luckiest choice). </li></ul><p>You are given a multiple-choice questions, can you predict child's choose?</p></div><div class="input-specification"><p>The first line starts with "<span class="tex-font-style-tt">A.</span>" (without quotes), then followed the description of choice <span class="tex-font-style-tt">A</span>. The next three lines contains the descriptions of the other choices in the same format. They are given in order: <span class="tex-font-style-tt">B</span>, <span class="tex-font-style-tt">C</span>, <span class="tex-font-style-tt">D</span>. <span class="tex-font-style-bf">Please note</span>, that the description goes after prefix "<span class="tex-font-style-tt">X.</span>", so the prefix mustn't be counted in description's length.</p><p>Each description is non-empty and consists of at most <span class="tex-span">100</span> characters. Each character can be either uppercase English letter or lowercase English letter, or "<span class="tex-font-style-tt">_</span>". </p></div><div class="output-specification"><p>Print a single line with the child's choice: "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">D</span>" (without quotes).</p></div>

## Input

<p>The first line starts with "<span class="tex-font-style-tt">A.</span>" (without quotes), then followed the description of choice <span class="tex-font-style-tt">A</span>. The next three lines contains the descriptions of the other choices in the same format. They are given in order: <span class="tex-font-style-tt">B</span>, <span class="tex-font-style-tt">C</span>, <span class="tex-font-style-tt">D</span>. <span class="tex-font-style-bf">Please note</span>, that the description goes after prefix "<span class="tex-font-style-tt">X.</span>", so the prefix mustn't be counted in description's length.</p><p>Each description is non-empty and consists of at most <span class="tex-span">100</span> characters. Each character can be either uppercase English letter or lowercase English letter, or "<span class="tex-font-style-tt">_</span>". </p>

## Output

<p>Print a single line with the child's choice: "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">D</span>" (without quotes).</p>





```input1
A.VFleaKing_is_the_author_of_this_problem
B.Picks_is_the_author_of_this_problem
C.Picking_is_the_author_of_this_problem
D.Ftiasch_is_cute

```




```input2
A.ab
B.abcde
C.ab
D.abc

```




```input3
A.c
B.cc
C.c
D.c

```




```output1
D

```




```output2
C

```




```output3
B

```



## Note

<p>In the first sample, the first choice has length 39, the second one has length 35, the third one has length 37, and the last one has length 15. The choice <span class="tex-font-style-tt">D</span> (length 15) is twice shorter than all other choices', so it is great choice. There is no other great choices so the child will choose <span class="tex-font-style-tt">D</span>.</p><p>In the second sample, no choice is great, so the child will choose the luckiest choice <span class="tex-font-style-tt">C</span>.</p><p>In the third sample, the choice <span class="tex-font-style-tt">B</span> (length 2) is twice longer than all other choices', so it is great choice. There is no other great choices so the child will choose <span class="tex-font-style-tt">B</span>.</p>
