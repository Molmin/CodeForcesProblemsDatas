## Description

<div><p>Little girl Alyona is in a shop to buy some copybooks for school. She study four subjects so she wants to have equal number of copybooks for each of the subjects. There are three types of copybook's packs in the shop: it is possible to buy one copybook for <span class="tex-span"><i>a</i></span> rubles, a pack of two copybooks for <span class="tex-span"><i>b</i></span> rubles, and a pack of three copybooks for <span class="tex-span"><i>c</i></span> rubles. Alyona already has <span class="tex-span"><i>n</i></span> copybooks.</p><p>What is the minimum amount of rubles she should pay to buy such number of copybooks <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>n</i> + <i>k</i></span> is divisible by <span class="tex-span">4</span>? There are infinitely many packs of any type in the shop. Alyona can buy packs of different type in the same purchase.</p></div><div class="input-specification"><p>The only line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the minimum amount of rubles she should pay to buy such number of copybooks <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>n</i> + <i>k</i></span> is divisible by <span class="tex-span">4</span>.</p></div>

## Input

<p>The only line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the minimum amount of rubles she should pay to buy such number of copybooks <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>n</i> + <i>k</i></span> is divisible by <span class="tex-span">4</span>.</p>





```input1
1 1 3 4

```




```input2
6 2 1 1

```




```input3
4 4 4 4

```




```input4
999999999 1000000000 1000000000 1000000000

```




```output1
3

```




```output2
1

```




```output3
0

```




```output4
1000000000

```



## Note

<p>In the first example Alyona can buy <span class="tex-span">3</span> packs of <span class="tex-span">1</span> copybook for <span class="tex-span">3<i>a</i> = 3</span> rubles in total. After that she will have <span class="tex-span">4</span> copybooks which she can split between the subjects equally. </p><p>In the second example Alyuna can buy a pack of <span class="tex-span">2</span> copybooks for <span class="tex-span"><i>b</i> = 1</span> ruble. She will have <span class="tex-span">8</span> copybooks in total.</p><p>In the third example Alyona can split the copybooks she already has between the <span class="tex-span">4</span> subject equally, so she doesn't need to buy anything.</p><p>In the fourth example Alyona should buy one pack of one copybook.</p>
