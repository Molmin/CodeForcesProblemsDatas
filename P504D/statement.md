## Description

<div><p>After Misha's birthday he had many large numbers left, scattered across the room. Now it's time to clean up and Misha needs to put them in a basket. He ordered this task to his pet robot that agreed to complete the task at certain conditions. Before the robot puts a number <span class="tex-span"><i>x</i></span> to the basket, Misha should answer the question: is it possible to choose one or multiple numbers that already are in the basket, such that their XOR sum equals <span class="tex-span"><i>x</i></span>? </p><p>If the answer is positive, you also need to give the indexes of these numbers. If there are multiple options of choosing numbers, you are allowed to choose any correct option. After Misha's answer the robot puts the number to the basket.</p><p>Initially the basket is empty. Each integer you put in the basket takes some number. The first integer you put into the basket take number <span class="tex-span">0</span>, the second integer takes number <span class="tex-span">1</span> and so on.</p><p>Misha needs to clean up the place as soon as possible but unfortunately, he isn't that good at mathematics. He asks you to help him.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>), showing how many numbers are scattered around the room.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the numbers in the order in which the robot puts them in the basket. Each number is a positive integer strictly less than <span class="tex-span">10<sup class="upper-index">600</sup></span> that doesn't contain leading zeroes. </p></div><div class="output-specification"><p>For each number either print a <span class="tex-span">0</span> on the corresponding line, if the number cannot be represented as a XOR sum of numbers that are in the basket, or print integer <span class="tex-span"><i>k</i></span> showing how many numbers are in the representation and the indexes of these numbers. Separate the numbers by spaces. Each number can occur in the representation at most once.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>), showing how many numbers are scattered around the room.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the numbers in the order in which the robot puts them in the basket. Each number is a positive integer strictly less than <span class="tex-span">10<sup class="upper-index">600</sup></span> that doesn't contain leading zeroes. </p>

## Output

<p>For each number either print a <span class="tex-span">0</span> on the corresponding line, if the number cannot be represented as a XOR sum of numbers that are in the basket, or print integer <span class="tex-span"><i>k</i></span> showing how many numbers are in the representation and the indexes of these numbers. Separate the numbers by spaces. Each number can occur in the representation at most once.</p>





```input1
7
7
6
5
4
3
2
1

```




```input2
2
5
5

```




```output1
0
0
0
3 0 1 2
2 1 2
2 0 2
2 0 1

```




```output2
0
1 0

```



## Note

<p>The XOR sum of numbers is the result of bitwise sum of numbers modulo 2.</p>
