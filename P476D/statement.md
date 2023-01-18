## Description

<div><p>Dreamoon likes to play with sets, integers and <img align="middle" class="tex-formula" src="file://n1yLltvu.png" style="max-width: 100.0%;max-height: 100.0%;">. <img align="middle" class="tex-formula" src="file://6Nsy1qDb.png" style="max-width: 100.0%;max-height: 100.0%;"> is defined as the largest positive integer that divides both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>Let <span class="tex-span"><i>S</i></span> be a set of exactly four distinct integers greater than <span class="tex-span">0</span>. Define <span class="tex-span"><i>S</i></span> to be of rank <span class="tex-span"><i>k</i></span> if and only if for all pairs of distinct elements <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> from <span class="tex-span"><i>S</i></span>, <img align="middle" class="tex-formula" src="file://n5QaZ1hq.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Given <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span>, Dreamoon wants to make up <span class="tex-span"><i>n</i></span> sets of rank <span class="tex-span"><i>k</i></span> using integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> such that no integer is used in two different sets (of course you can leave some integers without use). Calculate the minimum <span class="tex-span"><i>m</i></span> that makes it possible and print one possible solution.</p></div><div class="input-specification"><p>The single line of the input contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000, 1 ≤ <i>k</i> ≤ 100</span>).</p></div><div class="output-specification"><p>On the first line print a single integer — the minimal possible <span class="tex-span"><i>m</i></span>. </p><p>On each of the next <span class="tex-span"><i>n</i></span> lines print four space separated integers representing the <span class="tex-span"><i>i</i></span>-th set.</p><p>Neither the order of the sets nor the order of integers within a set is important. If there are multiple possible solutions with minimal <span class="tex-span"><i>m</i></span>, print any one of them.</p></div>

## Input

<p>The single line of the input contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000, 1 ≤ <i>k</i> ≤ 100</span>).</p>

## Output

<p>On the first line print a single integer — the minimal possible <span class="tex-span"><i>m</i></span>. </p><p>On each of the next <span class="tex-span"><i>n</i></span> lines print four space separated integers representing the <span class="tex-span"><i>i</i></span>-th set.</p><p>Neither the order of the sets nor the order of integers within a set is important. If there are multiple possible solutions with minimal <span class="tex-span"><i>m</i></span>, print any one of them.</p>





```input1
1 1

```




```input2
2 2

```




```output1
5
1 2 3 5

```




```output2
22
2 4 6 22
14 18 10 16

```



## Note

<p>For the first example it's easy to see that set <span class="tex-span">{1, 2, 3, 4}</span> isn't a valid set of rank 1 since <img align="middle" class="tex-formula" src="file://vfXrQpYn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
