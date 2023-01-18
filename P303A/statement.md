## Description

<div><p>Bike is interested in permutations. A permutation of length <span class="tex-span"><i>n</i></span> is an integer sequence such that each integer from 0 to <span class="tex-span">(<i>n</i> - 1)</span> appears exactly once in it. For example, <span class="tex-span">[0, 2, 1]</span> is a permutation of length 3 while both <span class="tex-span">[0, 2, 2]</span> and <span class="tex-span">[1, 2, 3]</span> is not.</p><p>A permutation triple of permutations of length <span class="tex-span"><i>n</i></span> <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> is called a Lucky Permutation Triple if and only if <img align="middle" class="tex-formula" src="file://ra8gc0Co.png" style="max-width: 100.0%;max-height: 100.0%;">. The sign <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>a</i></span>. The modular equality described above denotes that the remainders after dividing <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>b</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>n</i></span> and dividing <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>n</i></span> are equal.</p><p>Now, he has an integer <span class="tex-span"><i>n</i></span> and wants to find a Lucky Permutation Triple. Could you please help him?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>If no Lucky Permutation Triple of length <span class="tex-span"><i>n</i></span> exists print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, you need to print three lines. Each line contains <span class="tex-span"><i>n</i></span> space-seperated integers. The first line must contain permutation <span class="tex-span"><i>a</i></span>, the second line — permutation <span class="tex-span"><i>b</i></span>, the third — permutation <span class="tex-span"><i>c</i></span>.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>If no Lucky Permutation Triple of length <span class="tex-span"><i>n</i></span> exists print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, you need to print three lines. Each line contains <span class="tex-span"><i>n</i></span> space-seperated integers. The first line must contain permutation <span class="tex-span"><i>a</i></span>, the second line — permutation <span class="tex-span"><i>b</i></span>, the third — permutation <span class="tex-span"><i>c</i></span>.</p><p>If there are multiple solutions, print any of them.</p>





```input1
5

```




```input2
2

```




```output1
1 4 3 2 0
1 0 2 4 3
2 4 0 1 3

```




```output2
-1

```



## Note

<p>In Sample 1, the permutation triple <span class="tex-span">([1, 4, 3, 2, 0], [1, 0, 2, 4, 3], [2, 4, 0, 1, 3])</span> is Lucky Permutation Triple, as following holds:</p><ul> <li> <img align="middle" class="tex-formula" src="file://ewks8SqP.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> <img align="middle" class="tex-formula" src="file://SlhRIlDj.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> <img align="middle" class="tex-formula" src="file://obAIVknb.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> <img align="middle" class="tex-formula" src="file://ToEbS7dW.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> <img align="middle" class="tex-formula" src="file://jOqqoLMW.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>In Sample 2, you can easily notice that no lucky permutation triple exists.</p>
