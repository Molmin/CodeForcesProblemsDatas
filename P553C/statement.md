## Description

<div><p>There are many anime that are about "love triangles": Alice loves Bob, and Charlie loves Bob as well, but Alice hates Charlie. You are thinking about an anime which has <span class="tex-span"><i>n</i></span> characters. The characters are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Every pair of two characters can either mutually love each other or mutually hate each other (there is no neutral state).</p><p>You hate love triangles (A-B are in love and B-C are in love, but A-C hate each other), and you also hate it when nobody is in love. So, considering any three characters, you will be happy if exactly one pair is in love (A and B love each other, and C hates both A and B), or if all three pairs are in love (A loves B, B loves C, C loves A).</p><p>You are given a list of <span class="tex-span"><i>m</i></span> known relationships in the anime. You know for sure that certain pairs love each other, and certain pairs hate each other. You're wondering how many ways you can fill in the remaining relationships so you are happy with every triangle. Two ways are considered different if two characters are in love in one way but hate each other in the other. Print this count modulo <span class="tex-span">1 000 000 007</span>.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines will contain the description of the known relationships. The <span class="tex-span"><i>i</i></span>-th line will contain three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is 1, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are in love, otherwise, they hate each other (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <img align="middle" class="tex-formula" src="file://ttWka7m2.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each pair of people will be described no more than once.</p></div><div class="output-specification"><p>Print a single integer equal to the number of ways to fill in the remaining pairs so that you are happy with every triangle modulo <span class="tex-span">1 000 000 007</span>. </p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines will contain the description of the known relationships. The <span class="tex-span"><i>i</i></span>-th line will contain three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is 1, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are in love, otherwise, they hate each other (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <img align="middle" class="tex-formula" src="file://ttWka7m2.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each pair of people will be described no more than once.</p>

## Output

<p>Print a single integer equal to the number of ways to fill in the remaining pairs so that you are happy with every triangle modulo <span class="tex-span">1 000 000 007</span>. </p>





```input1
3 0

```




```input2
4 4
1 2 1
2 3 1
3 4 0
4 1 0

```




```input3
4 4
1 2 1
2 3 1
3 4 0
4 1 1

```




```output1
4

```




```output2
1

```




```output3
0

```



## Note

<p>In the first sample, the four ways are to: </p><ul> <li> Make everyone love each other </li><li> Make 1 and 2 love each other, and 3 hate 1 and 2 (symmetrically, we get 3 ways from this). </li></ul><p>In the second sample, the only possible solution is to make 1 and 3 love each other and 2 and 4 hate each other.</p>
