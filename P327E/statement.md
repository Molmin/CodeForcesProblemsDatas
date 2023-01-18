## Description

<div><p>Iahub wants to meet his girlfriend Iahubina. They both live in <span class="tex-span"><i>Ox</i></span> axis (the horizontal axis). Iahub lives at point 0 and Iahubina at point <span class="tex-span"><i>d</i></span>.</p><p>Iahub has <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The sum of those numbers is <span class="tex-span"><i>d</i></span>. Suppose <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> is a permutation of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>. Then, let <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub></span> and so on. The array b is called a "route". There are <span class="tex-span"><i>n</i>!</span> different routes, one for each permutation <span class="tex-span"><i>p</i></span>.</p><p>Iahub's travel schedule is: he walks <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> steps on <span class="tex-span"><i>Ox</i></span> axis, then he makes a break in point <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>. Then, he walks <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> more steps on <span class="tex-span"><i>Ox</i></span> axis and makes a break in point <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">2</sub></span>. Similarly, at <span class="tex-span"><i>j</i></span>-th <span class="tex-span">(1 ≤ <i>j</i> ≤ <i>n</i>)</span> time he walks <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> more steps on <span class="tex-span"><i>Ox</i></span> axis and makes a break in point <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">2</sub> + ... + <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Iahub is very superstitious and has <span class="tex-span"><i>k</i></span> integers which give him bad luck. He calls a route "good" if he never makes a break in a point corresponding to one of those <span class="tex-span"><i>k</i></span> numbers. For his own curiosity, answer how many good routes he can make, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>). The following line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2</span>). The fourth line contains <span class="tex-span"><i>k</i></span> positive integers, representing the numbers that give Iahub bad luck. Each of these numbers does not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Output a single integer — the answer of Iahub's dilemma modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>). The following line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2</span>). The fourth line contains <span class="tex-span"><i>k</i></span> positive integers, representing the numbers that give Iahub bad luck. Each of these numbers does not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Output a single integer — the answer of Iahub's dilemma modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p>





```input1
3
2 3 5
2
5 7

```




```input2
3
2 2 2
2
1 3

```




```output1
1

```




```output2
6

```



## Note

<p>In the first case consider six possible orderings:</p><ul> <li> [2, 3, 5]. Iahub will stop at position 2, 5 and 10. Among them, 5 is bad luck for him. </li><li> [2, 5, 3]. Iahub will stop at position 2, 7 and 10. Among them, 7 is bad luck for him. </li><li> [3, 2, 5]. He will stop at the unlucky 5. </li><li> [3, 5, 2]. This is a valid ordering. </li><li> [5, 2, 3]. He got unlucky twice (5 and 7). </li><li> [5, 3, 2]. Iahub would reject, as it sends him to position 5. </li></ul><p>In the second case, note that it is possible that two different ways have the identical set of stopping. In fact, all six possible ways have the same stops: [2, 4, 6], so there's no bad luck for Iahub.</p>
