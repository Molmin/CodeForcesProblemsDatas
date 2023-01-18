## Description

<div><p>The classic programming language of Bitland is Bit++. This language is so peculiar and complicated.</p><p>The language is that peculiar as it has exactly one variable, called <span class="tex-span"><i>x</i></span>. Also, there are two operations:</p><ul> <li> Operation <span class="tex-font-style-tt">++</span> increases the value of variable <span class="tex-span"><i>x</i></span> by 1. </li><li> Operation <span class="tex-font-style-tt">--</span> decreases the value of variable <span class="tex-span"><i>x</i></span> by 1. </li></ul><p>A statement in language Bit++ is a sequence, consisting of exactly one operation and one variable <span class="tex-span"><i>x</i></span>. The statement is written without spaces, that is, it can only contain characters "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">X</span>". Executing a statement means applying the operation it contains.</p><p>A programme in Bit++ is a sequence of statements, each of them needs to be executed. Executing a programme means executing all the statements it contains.</p><p>You're given a programme in language Bit++. The initial value of <span class="tex-span"><i>x</i></span> is <span class="tex-span">0</span>. Execute the programme and find its final value (the value of the variable when this programme is executed).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 150)</span> — the number of statements in the programme.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain a statement each. Each statement contains exactly one operation (<span class="tex-font-style-tt">++</span> or <span class="tex-font-style-tt">--</span>) and exactly one variable <span class="tex-span"><i>x</i></span> (denoted as letter «<span class="tex-font-style-tt">X</span>»). Thus, there are no empty statements. The operation and the variable can be written in any order.</p></div><div class="output-specification"><p>Print a single integer — the final value of <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 150)</span> — the number of statements in the programme.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain a statement each. Each statement contains exactly one operation (<span class="tex-font-style-tt">++</span> or <span class="tex-font-style-tt">--</span>) and exactly one variable <span class="tex-span"><i>x</i></span> (denoted as letter «<span class="tex-font-style-tt">X</span>»). Thus, there are no empty statements. The operation and the variable can be written in any order.</p>

## Output

<p>Print a single integer — the final value of <span class="tex-span"><i>x</i></span>.</p>





```input1
1
++X

```




```input2
2
X++
--X

```




```output1
1

```




```output2
0

```


