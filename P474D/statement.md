## Description

<div><p>We saw the little game Marmot made for Mole's lunch. Now it's Marmot's dinner time and, as we all know, Marmot eats flowers. At every dinner he eats some red and white flowers. Therefore a dinner can be represented as a sequence of several flowers, some of them white and some of them red.</p><p>But, for a dinner to be tasty, there is a rule: Marmot wants to eat white flowers only in groups of size <span class="tex-span"><i>k</i></span>.</p><p>Now Marmot wonders in how many ways he can eat between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> flowers. As the number of ways could be very large, print it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>Input contains several test cases.</p><p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>t</i></span> represents the number of test cases.</p><p>The next <span class="tex-span"><i>t</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), describing the <span class="tex-span"><i>i</i></span>-th test.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines to the standard output. The <span class="tex-span"><i>i</i></span>-th line should contain the number of ways in which Marmot can eat between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> flowers at dinner modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>Input contains several test cases.</p><p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>t</i></span> represents the number of test cases.</p><p>The next <span class="tex-span"><i>t</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), describing the <span class="tex-span"><i>i</i></span>-th test.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines to the standard output. The <span class="tex-span"><i>i</i></span>-th line should contain the number of ways in which Marmot can eat between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> flowers at dinner modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
3 2
1 3
2 3
4 4

```




```output1
6
5
5

```



## Note

<ul> <li> For <span class="tex-span"><i>K</i></span> = <span class="tex-span">2</span> and length <span class="tex-span">1</span> Marmot can eat (<span class="tex-span"><i>R</i></span>). </li><li> For <span class="tex-span"><i>K</i></span> = <span class="tex-span">2</span> and length <span class="tex-span">2</span> Marmot can eat (<span class="tex-span"><i>RR</i></span>) and (<span class="tex-span"><i>WW</i></span>). </li><li> For <span class="tex-span"><i>K</i></span> = <span class="tex-span">2</span> and length <span class="tex-span">3</span> Marmot can eat (<span class="tex-span"><i>RRR</i></span>), (<span class="tex-span"><i>RWW</i></span>) and (<span class="tex-span"><i>WWR</i></span>). </li><li> For <span class="tex-span"><i>K</i></span> = <span class="tex-span">2</span> and length <span class="tex-span">4</span> Marmot can eat, for example, (<span class="tex-span"><i>WWWW</i></span>) or (<span class="tex-span"><i>RWWR</i></span>), but for example he can't eat (<span class="tex-span"><i>WWWR</i></span>). </li></ul>
