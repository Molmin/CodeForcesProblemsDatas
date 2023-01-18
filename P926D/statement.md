## Description

<div><p>A classroom in a school has six rows with <span class="tex-span">3</span> desks in each row. Two people can use the same desk: one sitting on the left and one sitting on the right. </p><p>Some places are already occupied, and some places are vacant. Petya has just entered the class and wants to occupy the most convenient place. The conveniences of the places are shown on the picture:</p><center> <img class="tex-graphics" src="file://P8dqMRjo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here, the desks in the top row are the closest to the blackboard, while the desks in the bottom row are the furthest from the blackboard.</p><p>You are given a plan of the class, where '<span class="tex-font-style-tt">*</span>' denotes an occupied place, '<span class="tex-font-style-tt">.</span>' denotes a vacant place, and the aisles are denoted by '<span class="tex-font-style-tt">-</span>'. </p><p>Find any of the most convenient vacant places for Petya.</p></div><div class="input-specification"><p>The input consists of <span class="tex-span">6</span> lines. Each line describes one row of desks, starting from the closest to the blackboard. Each line is given in the following format: two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the left desk in the current row; a character '<span class="tex-font-style-tt">-</span>' — the aisle; two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the center desk in the current row; a character '<span class="tex-font-style-tt">-</span>' — the aisle; two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the right desk in the current row. So, the length of each of the six lines is <span class="tex-span">8</span>.</p><p>It is guaranteed that there is at least one vacant place in the classroom.</p></div><div class="output-specification"><p>Print the plan of the classroom after Petya takes one of the most convenient for him places. Mark this place with the letter '<span class="tex-font-style-tt">P</span>'. There should be exactly one letter '<span class="tex-font-style-tt">P</span>' in the plan. Petya can only take a vacant place. In all other places the output should coincide with the input.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The input consists of <span class="tex-span">6</span> lines. Each line describes one row of desks, starting from the closest to the blackboard. Each line is given in the following format: two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the left desk in the current row; a character '<span class="tex-font-style-tt">-</span>' — the aisle; two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the center desk in the current row; a character '<span class="tex-font-style-tt">-</span>' — the aisle; two characters, each is '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">.</span>' — the description of the right desk in the current row. So, the length of each of the six lines is <span class="tex-span">8</span>.</p><p>It is guaranteed that there is at least one vacant place in the classroom.</p>

## Output

<p>Print the plan of the classroom after Petya takes one of the most convenient for him places. Mark this place with the letter '<span class="tex-font-style-tt">P</span>'. There should be exactly one letter '<span class="tex-font-style-tt">P</span>' in the plan. Petya can only take a vacant place. In all other places the output should coincide with the input.</p><p>If there are multiple answers, print any.</p>





```input1
..-**-..
..-**-..
..-..-..
..-..-..
..-..-..
..-..-..

```




```input2
**-**-**
**-**-**
..-**-.*
**-**-**
..-..-..
..-**-..

```




```input3
**-**-*.
*.-*.-**
**-**-**
**-**-**
..-..-..
..-**-..

```




```output1
..-**-..
..-**-..
..-..-..
..-P.-..
..-..-..
..-..-..

```




```output2
**-**-**
**-**-**
..-**-.*
**-**-**
..-P.-..
..-**-..

```




```output3
**-**-*.
*.-*P-**
**-**-**
**-**-**
..-..-..
..-**-..

```



## Note

<p>In the first example the maximum convenience is <span class="tex-span">3</span>.</p><p>In the second example the maximum convenience is <span class="tex-span">2</span>.</p><p>In the third example the maximum convenience is <span class="tex-span">4</span>.</p>
