## Description

<div><p>The Beroil corporation structure is hierarchical, that is it can be represented as a tree. Let's examine the presentation of this structure as follows:</p><ul> <li> <span class="tex-span"><i>employee</i></span> ::= <span class="tex-span"><i>name</i></span><span class="tex-font-style-tt">.</span> | <span class="tex-span"><i>name</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>employee</i><sub class="lower-index">1</sub></span><span class="tex-font-style-tt">,</span><span class="tex-span"><i>employee</i><sub class="lower-index">2</sub></span><span class="tex-font-style-tt">,</span> ... <span class="tex-font-style-tt">,</span><span class="tex-span"><i>employee</i><sub class="lower-index"><i>k</i></sub></span><span class="tex-font-style-tt">.</span> </li><li> <span class="tex-span"><i>name</i></span> ::= name of an employee </li></ul><p>That is, the description of each employee consists of his name, a colon (<span class="tex-font-style-tt">:</span>), the descriptions of all his subordinates separated by commas, and, finally, a dot. If an employee has no subordinates, then the colon is not present in his description.</p><p>For example, line <span class="tex-font-style-tt">MIKE:MAX.,ARTEM:MIKE..,DMITRY:DMITRY.,DMITRY...</span> is the correct way of recording the structure of a corporation where the director <span class="tex-font-style-tt">MIKE</span> has subordinates <span class="tex-font-style-tt">MAX</span>, <span class="tex-font-style-tt">ARTEM</span> and <span class="tex-font-style-tt">DMITRY</span>. <span class="tex-font-style-tt">ARTEM</span> has a subordinate whose name is <span class="tex-font-style-tt">MIKE</span>, just as the name of his boss and two subordinates of <span class="tex-font-style-tt">DMITRY</span> are called <span class="tex-font-style-tt">DMITRY</span>, just like himself.</p><p>In the Beroil corporation every employee can only correspond with his subordinates, at that the subordinates are not necessarily direct. Let's call an uncomfortable situation the situation when a person whose name is <span class="tex-span"><i>s</i></span> writes a letter to another person whose name is also <span class="tex-span"><i>s</i></span>. In the example given above are two such pairs: a pair involving <span class="tex-font-style-tt">MIKE</span>, and two pairs for <span class="tex-font-style-tt">DMITRY</span> (a pair for each of his subordinates).</p><p>Your task is by the given structure of the corporation to find the number of uncomfortable pairs in it.</p><center><img class="tex-graphics" src="file://7MDHfgjb.png" style="max-width: 100.0%;max-height: 100.0%;"></center></div><div class="input-specification"><p>The first and single line contains the corporation structure which is a string of length from 1 to 1000 characters. It is guaranteed that the description is correct. Every name is a string consisting of capital Latin letters from 1 to 10 symbols in length.</p></div><div class="output-specification"><p>Print a single number — the number of uncomfortable situations in the company.</p></div>

## Input

<p>The first and single line contains the corporation structure which is a string of length from 1 to 1000 characters. It is guaranteed that the description is correct. Every name is a string consisting of capital Latin letters from 1 to 10 symbols in length.</p>

## Output

<p>Print a single number — the number of uncomfortable situations in the company.</p>





```input1
MIKE:MAX.,ARTEM:MIKE..,DMITRY:DMITRY.,DMITRY...

```




```input2
A:A..

```




```input3
A:C:C:C:C.....

```




```output1
3

```




```output2
1

```




```output3
6

```


