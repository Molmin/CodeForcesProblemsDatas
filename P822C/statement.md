## Description

<div><p>It's well known that the best way to distract from something is to do one's favourite thing. Job is such a thing for Leha.</p><p>So the hacker began to work hard in order to get rid of boredom. It means that Leha began to hack computers all over the world. For such zeal boss gave the hacker a vacation of exactly <span class="tex-span"><i>x</i></span> days. You know the majority of people prefer to go somewhere for a vacation, so Leha immediately went to the travel agency. There he found out that <span class="tex-span"><i>n</i></span> vouchers left. <span class="tex-span"><i>i</i></span>-th voucher is characterized by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> — day of departure from Vičkopolis, day of arriving back in Vičkopolis and cost of the voucher correspondingly. The duration of the <span class="tex-span"><i>i</i></span>-th voucher is a value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> + 1</span>.</p><p>At the same time Leha wants to split his own vocation into two parts. Besides he wants to spend as little money as possible. Formally Leha wants to choose exactly two vouchers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>i</i> ≠ <i>j</i>)</span> so that they don't intersect, sum of their durations is <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>x</i></span> and their total cost is as minimal as possible. Two vouchers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> don't intersect if only at least one of the following conditions is fulfilled: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>l</i><sub class="lower-index"><i>j</i></sub></span> or <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub> &lt; <i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help Leha to choose the necessary vouchers!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>x</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of vouchers in the travel agency and the duration of Leha's vacation correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — description of the voucher.</p></div><div class="output-specification"><p>Print a single integer — a minimal amount of money that Leha will spend, or print <span class="tex-span"> - 1</span> if it's impossible to choose two disjoint vouchers with the total duration <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>x</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of vouchers in the travel agency and the duration of Leha's vacation correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — description of the voucher.</p>

## Output

<p>Print a single integer — a minimal amount of money that Leha will spend, or print <span class="tex-span"> - 1</span> if it's impossible to choose two disjoint vouchers with the total duration <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>x</i></span>.</p>





```input1
4 5
1 3 4
1 2 5
5 6 1
1 2 4

```




```input2
3 2
4 6 3
2 4 1
3 5 4

```




```output1
5

```




```output2
-1

```



## Note

<p>In the first sample Leha should choose first and third vouchers. Hereupon the total duration will be equal to <span class="tex-span">(3 - 1 + 1) + (6 - 5 + 1) = 5</span> and the total cost will be <span class="tex-span">4 + 1 = 5</span>.</p><p>In the second sample the duration of each voucher is <span class="tex-span">3</span> therefore it's impossible to choose two vouchers with the total duration equal to <span class="tex-span">2</span>.</p>
