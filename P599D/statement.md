## Description

<div><p>Spongebob is already tired trying to reason his weird actions and calculations, so he simply asked you to find all pairs of n and m, such that there are exactly <span class="tex-span"><i>x</i></span> distinct squares in the table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. For example, in a <span class="tex-span">3 × 5</span> table there are <span class="tex-span">15</span> squares with side one, <span class="tex-span">8</span> squares with side two and <span class="tex-span">3</span> squares with side three. The total number of distinct squares in a <span class="tex-span">3 × 5</span> table is <span class="tex-span">15 + 8 + 3 = 26</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of squares inside the tables Spongebob is interested in.</p></div><div class="output-specification"><p>First print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of tables with exactly <span class="tex-span"><i>x</i></span> distinct squares inside.</p><p>Then print <span class="tex-span"><i>k</i></span> pairs of integers describing the tables. Print the pairs in the order of increasing <span class="tex-span"><i>n</i></span>, and in case of equality&nbsp;— in the order of increasing <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of squares inside the tables Spongebob is interested in.</p>

## Output

<p>First print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of tables with exactly <span class="tex-span"><i>x</i></span> distinct squares inside.</p><p>Then print <span class="tex-span"><i>k</i></span> pairs of integers describing the tables. Print the pairs in the order of increasing <span class="tex-span"><i>n</i></span>, and in case of equality&nbsp;— in the order of increasing <span class="tex-span"><i>m</i></span>.</p>





```input1
26

```




```input2
2

```




```input3
8

```




```output1
6
1 26
2 9
3 5
5 3
9 2
26 1

```




```output2
2
1 2
2 1

```




```output3
4
1 8
2 3
3 2
8 1

```



## Note

<p>In a <span class="tex-span">1 × 2</span> table there are <span class="tex-span">2</span> <span class="tex-span">1 × 1</span> squares. So, <span class="tex-span">2</span> distinct squares in total.</p><center> <img class="tex-graphics" height="113px" src="file://aNr9xC8U.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center><p>In a <span class="tex-span">2 × 3</span> table there are <span class="tex-span">6</span> <span class="tex-span">1 × 1</span> squares and <span class="tex-span">2</span> <span class="tex-span">2 × 2</span> squares. That is equal to <span class="tex-span">8</span> squares in total.</p><center> <img class="tex-graphics" height="151px" src="file://fOkvzRmK.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
