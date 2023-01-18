## Description

<div><p>John Doe offered his sister Jane Doe find the gcd of some set of numbers <span class="tex-span"><i>a</i></span>.</p><p>Gcd is a positive integer <span class="tex-span"><i>g</i></span>, such that all number from the set are evenly divisible by <span class="tex-span"><i>g</i></span> and there isn't such <span class="tex-span"><i>g</i>'</span> <span class="tex-span">(<i>g</i>' &gt; <i>g</i>)</span>, that all numbers of the set are evenly divisible by <span class="tex-span"><i>g</i>'</span>.</p><p>Unfortunately Jane couldn't cope with the task and John offered her to find the ghd of the same subset of numbers.</p><p>Ghd is a positive integer <span class="tex-span"><i>g</i></span>, such that at least half of numbers from the set are evenly divisible by <span class="tex-span"><i>g</i></span> and there isn't such <span class="tex-span"><i>g</i>'</span> <span class="tex-span">(<i>g</i>' &gt; <i>g</i>)</span> that at least half of the numbers from the set are evenly divisible by <span class="tex-span"><i>g</i>'</span>.</p><p>Jane coped with the task for two hours. Please try it, too.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) showing how many numbers are in set <span class="tex-span"><i>a</i></span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup>)</span>. Please note, that given set can contain <span class="tex-font-style-bf">equal</span> numbers.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer <span class="tex-span"><i>g</i></span> — the Ghd of set <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) showing how many numbers are in set <span class="tex-span"><i>a</i></span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup>)</span>. Please note, that given set can contain <span class="tex-font-style-bf">equal</span> numbers.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer <span class="tex-span"><i>g</i></span> — the Ghd of set <span class="tex-span"><i>a</i></span>.</p>





```input1
6
6 2 3 4 5 6

```




```input2
5
5 5 6 10 15

```




```output1
3

```




```output2
5

```


