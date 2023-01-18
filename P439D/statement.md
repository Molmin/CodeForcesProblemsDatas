## Description

<div><p>Devu and his brother love each other a lot. As they are super geeks, they only like to play with arrays. They are given two arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> by their father. The array <span class="tex-span"><i>a</i></span> is given to Devu and <span class="tex-span"><i>b</i></span> to his brother. </p><p>As Devu is really a naughty kid, he wants the minimum value of his array <span class="tex-span"><i>a</i></span> should be at least as much as the maximum value of his brother's array <span class="tex-span"><i>b</i></span>. </p><p>Now you have to help Devu in achieving this condition. You can perform multiple operations on the arrays. In a single operation, you are allowed to decrease or increase any element of any of the arrays by 1. Note that you are allowed to apply the operation on any index of the array multiple times.</p><p>You need to find minimum number of operations required to satisfy Devu's condition so that the brothers can play peacefully without fighting. </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line will contain <span class="tex-span"><i>n</i></span> space-separated integers representing content of the array <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line will contain <span class="tex-span"><i>m</i></span> space-separated integers representing content of the array <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>You need to output a single integer representing the minimum number of operations needed to satisfy Devu's condition.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line will contain <span class="tex-span"><i>n</i></span> space-separated integers representing content of the array <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line will contain <span class="tex-span"><i>m</i></span> space-separated integers representing content of the array <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>You need to output a single integer representing the minimum number of operations needed to satisfy Devu's condition.</p>





```input1
2 2
2 3
3 5

```




```input2
3 2
1 2 3
3 4

```




```input3
3 2
4 5 6
1 2

```




```output1
3

```




```output2
4

```




```output3
0

```



## Note

<p>In example <span class="tex-span">1</span>, you can increase <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> by <span class="tex-span">1</span> and decrease <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> by <span class="tex-span">1</span> and then again decrease <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> by <span class="tex-span">1</span>. Now array <span class="tex-span"><i>a</i></span> will be [<span class="tex-span">3</span>; <span class="tex-span">3</span>] and array <span class="tex-span"><i>b</i></span> will also be [<span class="tex-span">3</span>; <span class="tex-span">3</span>]. Here minimum element of <span class="tex-span"><i>a</i></span> is at least as large as maximum element of <span class="tex-span"><i>b</i></span>. So minimum number of operations needed to satisfy Devu's condition are <span class="tex-span">3</span>.</p><p>In example <span class="tex-span">3</span>, you don't need to do any operation, Devu's condition is already satisfied. </p>
