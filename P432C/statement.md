## Description

<div><p>You have an array <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span>, containing distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Your task is to sort this array in increasing order with the following operation (you may need to apply it multiple times):</p><ul> <li> choose two indexes, <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>; <span class="tex-span">(<i>j</i> - <i>i</i> + 1)</span> is a prime number); </li><li> swap the elements on positions <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>; in other words, you are allowed to apply the following sequence of assignments: <span class="tex-span"><i>tmp</i> = <i>a</i>[<i>i</i>], <i>a</i>[<i>i</i>] = <i>a</i>[<i>j</i>], <i>a</i>[<i>j</i>] = <i>tmp</i></span> (<span class="tex-span"><i>tmp</i></span> is a temporary variable). </li></ul><p>You do not need to minimize the number of used operations. However, you need to make sure that there are at most <span class="tex-span">5<i>n</i></span> operations.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> <span class="tex-span">(1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>In the first line, print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 5<i>n</i>)</span> — the number of used operations. Next, print the operations. Each operation must be printed as "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>" (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>; <span class="tex-span">(<i>j</i> - <i>i</i> + 1)</span> is a prime).</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> <span class="tex-span">(1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i>)</span>.</p>

## Output

<p>In the first line, print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 5<i>n</i>)</span> — the number of used operations. Next, print the operations. Each operation must be printed as "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>" (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>; <span class="tex-span">(<i>j</i> - <i>i</i> + 1)</span> is a prime).</p><p>If there are multiple answers, you can print any of them.</p>





```input1
3
3 2 1

```




```input2
2
1 2

```




```input3
4
4 2 3 1

```




```output1
1
1 3

```




```output2
0

```




```output3
3
2 4
1 2
2 4

```


