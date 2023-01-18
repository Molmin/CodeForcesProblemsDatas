## Description

<div><p>Petya was late for the lesson too. The teacher gave him an additional task. For some array <span class="tex-span"><i>a</i></span> Petya should find the number of different ways to select non-empty subset of elements from it in such a way that their product is equal to a square of some integer.</p><p>Two ways are considered different if sets of indexes of elements chosen by these ways are different.</p><p>Since the answer can be very large, you should find the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>First line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 70</span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of different ways to choose some elements so that their product is a square of a certain integer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>First line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 70</span>)&nbsp;— the elements of the array.</p>

## Output

<p>Print one integer&nbsp;— the number of different ways to choose some elements so that their product is a square of a certain integer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
1 1 1 1

```




```input2
4
2 2 2 2

```




```input3
5
1 2 4 5 8

```




```output1
15

```




```output2
7

```




```output3
7

```



## Note

<p>In first sample product of elements chosen by any way is <span class="tex-span">1</span> and <span class="tex-span">1 = 1<sup class="upper-index">2</sup></span>. So the answer is <span class="tex-span">2<sup class="upper-index">4</sup> - 1 = 15</span>.</p><p>In second sample there are six different ways to choose elements so that their product is <span class="tex-span">4</span>, and only one way so that their product is <span class="tex-span">16</span>. So the answer is <span class="tex-span">6 + 1 = 7</span>.</p>
