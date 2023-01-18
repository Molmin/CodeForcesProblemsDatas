## Description

<div><p>A lot of people associate Logo programming language with turtle graphics. In this case the turtle moves along the straight line and accepts commands "<span class="tex-font-style-tt">T</span>" ("turn around") and "<span class="tex-font-style-tt">F</span>" ("move 1 unit forward").</p><p>You are given a list of commands that will be given to the turtle. You have to change exactly <span class="tex-span"><i>n</i></span> commands from the list (one command can be changed several times). How far from the starting point can the turtle move after it follows <span class="tex-font-style-bf">all</span> the commands of the modified list?</p></div><div class="input-specification"><p>The first line of input contains a string <span class="tex-span"><i>commands</i></span> — the original list of commands. The string <span class="tex-span"><i>commands</i></span> contains between 1 and 100 characters, inclusive, and contains only characters "<span class="tex-font-style-tt">T</span>" and "<span class="tex-font-style-tt">F</span>".</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of commands you have to change in the list.</p></div><div class="output-specification"><p>Output the maximum distance from the starting point to the ending point of the turtle's path. The ending point of the turtle's path is turtle's coordinate after it follows <span class="tex-font-style-bf">all</span> the commands of the modified list.</p></div>

## Input

<p>The first line of input contains a string <span class="tex-span"><i>commands</i></span> — the original list of commands. The string <span class="tex-span"><i>commands</i></span> contains between 1 and 100 characters, inclusive, and contains only characters "<span class="tex-font-style-tt">T</span>" and "<span class="tex-font-style-tt">F</span>".</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of commands you have to change in the list.</p>

## Output

<p>Output the maximum distance from the starting point to the ending point of the turtle's path. The ending point of the turtle's path is turtle's coordinate after it follows <span class="tex-font-style-bf">all</span> the commands of the modified list.</p>





```input1
FT
1

```




```input2
FFFTFFF
2

```




```output1
2

```




```output2
6

```



## Note

<p>In the first example the best option is to change the second command ("<span class="tex-font-style-tt">T</span>") to "<span class="tex-font-style-tt">F</span>" — this way the turtle will cover a distance of 2 units.</p><p>In the second example you have to change two commands. One of the ways to cover maximal distance of 6 units is to change the fourth command and first or last one.</p>
