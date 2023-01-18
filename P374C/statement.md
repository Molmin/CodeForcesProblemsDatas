## Description

<div><p>Inna and Dima bought a table of size <span class="tex-span"><i>n</i> × <i>m</i></span> in the shop. Each cell of the table contains a single letter: "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">I</span>", "<span class="tex-font-style-tt">M</span>", "<span class="tex-font-style-tt">A</span>".</p><p>Inna loves Dima, so she wants to go through his name as many times as possible as she moves through the table. For that, Inna acts as follows:</p><ol> <li> initially, Inna chooses some cell of the table where letter "<span class="tex-font-style-tt">D</span>" is written; </li><li> then Inna can move to some side-adjacent table cell that contains letter "<span class="tex-font-style-tt">I</span>"; then from this cell she can go to one of the side-adjacent table cells that contains the written letter "<span class="tex-font-style-tt">M</span>"; then she can go to a side-adjacent cell that contains letter "<span class="tex-font-style-tt">A</span>". Then Inna assumes that she has gone through her sweetheart's name; </li><li> Inna's next move can be going to one of the side-adjacent table cells that contains letter "<span class="tex-font-style-tt">D</span>" and then walk on through name DIMA in the similar manner. Inna never skips a letter. So, from the letter "<span class="tex-font-style-tt">D</span>" she always goes to the letter "<span class="tex-font-style-tt">I</span>", from the letter "<span class="tex-font-style-tt">I</span>" she always goes the to letter "<span class="tex-font-style-tt">M</span>", from the letter "<span class="tex-font-style-tt">M</span>" she always goes to the letter "<span class="tex-font-style-tt">A</span>", and from the letter "<span class="tex-font-style-tt">A</span>" she always goes to the letter "<span class="tex-font-style-tt">D</span>". </li></ol><p>Depending on the choice of the initial table cell, Inna can go through name DIMA either an infinite number of times or some positive finite number of times or she can't go through his name once. Help Inna find out what maximum number of times she can go through name DIMA.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>)</span>. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines that describe Inna and Dima's table. Each line contains <span class="tex-span"><i>m</i></span> characters. Each character is one of the following four characters: "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">I</span>", "<span class="tex-font-style-tt">M</span>", "<span class="tex-font-style-tt">A</span>". </p><p>Note that it is not guaranteed that the table contains at least one letter "<span class="tex-font-style-tt">D</span>".</p></div><div class="output-specification"><p>If Inna cannot go through name DIMA once, print on a single line "<span class="tex-font-style-tt">Poor Dima!</span>" without the quotes. If there is the infinite number of names DIMA Inna can go through, print "<span class="tex-font-style-tt">Poor Inna!</span>" without the quotes. Otherwise print a single integer — the maximum number of times Inna can go through name DIMA.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>)</span>. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines that describe Inna and Dima's table. Each line contains <span class="tex-span"><i>m</i></span> characters. Each character is one of the following four characters: "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">I</span>", "<span class="tex-font-style-tt">M</span>", "<span class="tex-font-style-tt">A</span>". </p><p>Note that it is not guaranteed that the table contains at least one letter "<span class="tex-font-style-tt">D</span>".</p>

## Output

<p>If Inna cannot go through name DIMA once, print on a single line "<span class="tex-font-style-tt">Poor Dima!</span>" without the quotes. If there is the infinite number of names DIMA Inna can go through, print "<span class="tex-font-style-tt">Poor Inna!</span>" without the quotes. Otherwise print a single integer — the maximum number of times Inna can go through name DIMA.</p>





```input1
1 2
DI

```




```input2
2 2
MA
ID

```




```input3
5 5
DIMAD
DIMAI
DIMAM
DDMAA
AAMID

```




```output1
Poor Dima!

```




```output2
Poor Inna!

```




```output3
4

```



## Note

<p>Notes to the samples:</p><p>In the first test sample, Inna cannot go through name DIMA a single time.</p><p>In the second test sample, Inna can go through the infinite number of words DIMA. For that, she should move in the clockwise direction starting from the lower right corner.</p><p>In the third test sample the best strategy is to start from the cell in the upper left corner of the table. Starting from this cell, Inna can go through name DIMA four times. </p>
