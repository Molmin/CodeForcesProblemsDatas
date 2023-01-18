## Description

<div><p>Dr. Evil kidnapped Mahmoud and Ehab in the evil land because of their performance in the Evil Olympiad in Informatics (EOI). He decided to give them some problems to let them go.</p><p>Dr. Evil is interested in sets, He has a set of <span class="tex-span"><i>n</i></span> integers. Dr. Evil calls a set of integers <span class="tex-font-style-it">evil</span> if the <span class="tex-font-style-it">MEX</span> of it is exactly <span class="tex-span"><i>x</i></span>. the <span class="tex-font-style-it">MEX</span> of a set of integers is the minimum non-negative integer that doesn't exist in it. For example, the <span class="tex-font-style-it">MEX</span> of the set <span class="tex-span">{0, 2, 4}</span> is <span class="tex-span">1</span> and the <span class="tex-font-style-it">MEX</span> of the set <span class="tex-span">{1, 2, 3}</span> is <span class="tex-span">0</span> .</p><p>Dr. Evil is going to make his set <span class="tex-font-style-it">evil</span>. To do this he can perform some operations. During each operation he can add some non-negative integer to his set or erase some element from it. What is the minimal number of operations Dr. Evil has to perform to make his set <span class="tex-font-style-it">evil</span>?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 100</span>)&nbsp;— the size of the set Dr. Evil owns, and the desired <span class="tex-font-style-it">MEX</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct non-negative integers not exceeding <span class="tex-span">100</span> that represent the set.</p></div><div class="output-specification"><p>The only line should contain one integer&nbsp;— the minimal number of operations Dr. Evil should perform.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 100</span>)&nbsp;— the size of the set Dr. Evil owns, and the desired <span class="tex-font-style-it">MEX</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct non-negative integers not exceeding <span class="tex-span">100</span> that represent the set.</p>

## Output

<p>The only line should contain one integer&nbsp;— the minimal number of operations Dr. Evil should perform.</p>





```input1
5 3
0 4 5 6 7

```




```input2
1 0
0

```




```input3
5 0
1 2 3 4 5

```




```output1
2

```




```output2
1

```




```output3
0

```



## Note

<p>For the first test case Dr. Evil should add <span class="tex-span">1</span> and <span class="tex-span">2</span> to the set performing <span class="tex-span">2</span> operations.</p><p>For the second test case Dr. Evil should erase <span class="tex-span">0</span> from the set. After that, the set becomes empty, so the <span class="tex-font-style-it">MEX</span> of it is <span class="tex-span">0</span>.</p><p>In the third test case the set is already <span class="tex-font-style-it">evil</span>.</p>
