## Description

<div><p>Anya loves to fold and stick. Today she decided to do just that.</p><p>Anya has <span class="tex-span"><i>n</i></span> cubes lying in a line and numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right, with natural numbers written on them. She also has <span class="tex-span"><i>k</i></span> stickers with exclamation marks. We know that the number of stickers does not exceed the number of cubes.</p><p>Anya can stick an exclamation mark on the cube and get the factorial of the number written on the cube. For example, if a cube reads <span class="tex-span">5</span>, then after the sticking it reads <span class="tex-span">5!</span>, which equals <span class="tex-span">120</span>.</p><p>You need to help Anya count how many ways there are to choose some of the cubes and stick on some of the chosen cubes at most <span class="tex-span"><i>k</i></span> exclamation marks so that the sum of the numbers written on the chosen cubes after the sticking becomes equal to <span class="tex-span"><i>S</i></span>. Anya can stick at most one exclamation mark on each cube. Can you do it?</p><p>Two ways are considered the same if they have the same set of chosen cubes and the same set of cubes with exclamation marks.</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 25</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">16</sup></span>)&nbsp;—&nbsp;the number of cubes and the number of stickers that Anya has, and the sum that she needs to get. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;—&nbsp;the numbers, written on the cubes. The cubes in the input are described in the order from left to right, starting from the first one. </p><p>Multiple cubes can contain the same numbers.</p></div><div class="output-specification"><p>Output the number of ways to choose some number of cubes and stick exclamation marks on some of them so that the sum of the numbers became equal to the given number <span class="tex-span"><i>S</i></span>.</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 25</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">16</sup></span>)&nbsp;—&nbsp;the number of cubes and the number of stickers that Anya has, and the sum that she needs to get. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;—&nbsp;the numbers, written on the cubes. The cubes in the input are described in the order from left to right, starting from the first one. </p><p>Multiple cubes can contain the same numbers.</p>

## Output

<p>Output the number of ways to choose some number of cubes and stick exclamation marks on some of them so that the sum of the numbers became equal to the given number <span class="tex-span"><i>S</i></span>.</p>





```input1
2 2 30
4 3

```




```input2
2 2 7
4 3

```




```input3
3 1 1
1 1 1

```




```output1
1

```




```output2
1

```




```output3
6

```



## Note

<p>In the first sample the only way is to choose both cubes and stick an exclamation mark on each of them.</p><p>In the second sample the only way is to choose both cubes but don't stick an exclamation mark on any of them.</p><p>In the third sample it is possible to choose any of the cubes in three ways, and also we may choose to stick or not to stick the exclamation mark on it. So, the total number of ways is six.</p>
