## Description

<div><p>Levko loves all sorts of sets very much.</p><p>Levko has two arrays of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... , <i>b</i><sub class="lower-index"><i>m</i></sub></span> and a prime number <span class="tex-span"><i>p</i></span>. Today he generates <span class="tex-span"><i>n</i></span> sets. Let's describe the generation process for the <span class="tex-span"><i>i</i></span>-th set:</p><ol> <li> First it has a single number <span class="tex-span">1</span>. </li><li> Let's take any element <span class="tex-span"><i>c</i></span> from this set. For all <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) if number <span class="tex-span">(<i>c</i>·<i>a</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>b</i><sub class="lower-index"><i>j</i></sub></sup>)&nbsp;<i>mod</i>&nbsp;<i>p</i></span> doesn't occur in the set, then add it to the set. </li><li> Repeat step <span class="tex-span">2</span> as long as we can add at least one element to our set. </li></ol><p>Levko wonders, how many numbers belong to at least one set. That is, he wants to know what size is the union of <span class="tex-span"><i>n</i></span> generated sets.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>p</i></span> is prime. </p><p>The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i></span>). The third line contains space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... , <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>The single number — the size of the union of the sets.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>p</i></span> is prime. </p><p>The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i></span>). The third line contains space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... , <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>The single number — the size of the union of the sets.</p>





```input1
1 1 7
2
5

```




```input2
1 2 7
2
2 4

```




```input3
2 1 7
1 6
2

```




```input4
2 1 7
1 6
5

```




```output1
3

```




```output2
3

```




```output3
1

```




```output4
2

```


