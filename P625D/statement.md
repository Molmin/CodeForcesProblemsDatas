## Description

<div><p>Vitya is studying in the third grade. During the last math lesson all the pupils wrote on arithmetic quiz. Vitya is a clever boy, so he managed to finish all the tasks pretty fast and Oksana Fillipovna gave him a new one, that is much harder.</p><p>Let's denote a <span class="tex-font-style-it">flip operation</span> of an integer as follows: number is considered in decimal notation and then reverted. If there are any leading zeroes afterwards, they are thrown away. For example, if we flip <span class="tex-span">123</span> the result is the integer <span class="tex-span">321</span>, but flipping <span class="tex-span">130</span> we obtain <span class="tex-span">31</span>, and by flipping <span class="tex-span">31</span> we come to <span class="tex-span">13</span>.</p><p>Oksana Fillipovna picked some number <span class="tex-span"><i>a</i></span> without leading zeroes, and flipped it to get number <span class="tex-span"><i>a</i><sub class="lower-index"><i>r</i></sub></span>. Then she summed <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>r</i></sub></span>, and told Vitya the resulting value <span class="tex-span"><i>n</i></span>. His goal is to find any valid <span class="tex-span"><i>a</i></span>.</p><p>As Oksana Fillipovna picked some small integers as <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>r</i></sub></span>, Vitya managed to find the answer pretty fast and became interested in finding some general algorithm to deal with this problem. Now, he wants you to write the program that for given <span class="tex-span"><i>n</i></span> finds any <span class="tex-span"><i>a</i></span> without leading zeroes, such that <span class="tex-span"><i>a</i> + <i>a</i><sub class="lower-index"><i>r</i></sub> = <i>n</i></span> or determine that such <span class="tex-span"><i>a</i></span> doesn't exist.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">100 000</sup></span>).</p></div><div class="output-specification"><p>If there is no such positive integer <span class="tex-span"><i>a</i></span> without leading zeroes that <span class="tex-span"><i>a</i> + <i>a</i><sub class="lower-index"><i>r</i></sub> = <i>n</i></span> then print <span class="tex-span">0</span>. Otherwise, print any valid <span class="tex-span"><i>a</i></span>. If there are many possible answers, you are allowed to pick any.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">100 000</sup></span>).</p>

## Output

<p>If there is no such positive integer <span class="tex-span"><i>a</i></span> without leading zeroes that <span class="tex-span"><i>a</i> + <i>a</i><sub class="lower-index"><i>r</i></sub> = <i>n</i></span> then print <span class="tex-span">0</span>. Otherwise, print any valid <span class="tex-span"><i>a</i></span>. If there are many possible answers, you are allowed to pick any.</p>





```input1
4

```




```input2
11

```




```input3
5

```




```input4
33

```




```output1
2

```




```output2
10

```




```output3
0

```




```output4
21

```



## Note

<p>In the first sample <span class="tex-span">4 = 2 + 2</span>, <span class="tex-span"><i>a</i> = 2</span> is the only possibility.</p><p>In the second sample <span class="tex-span">11 = 10 + 1</span>, <span class="tex-span"><i>a</i> = 10</span>&nbsp;— the only valid solution. Note, that <span class="tex-span"><i>a</i> = 01</span> is incorrect, because <span class="tex-span"><i>a</i></span> can't have leading zeroes.</p><p>It's easy to check that there is no suitable <span class="tex-span"><i>a</i></span> in the third sample.</p><p>In the fourth sample <span class="tex-span">33 = 30 + 3 = 12 + 21</span>, so there are three possibilities for <span class="tex-span"><i>a</i></span>: <span class="tex-span"><i>a</i> = 30</span>, <span class="tex-span"><i>a</i> = 12</span>, <span class="tex-span"><i>a</i> = 21</span>. Any of these is considered to be correct answer.</p>
