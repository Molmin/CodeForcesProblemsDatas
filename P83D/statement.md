## Description

<div><p><span class="tex-font-style-underline">One quite ordinary day Valera went to school (there's nowhere else he should go on a week day). In a maths lesson his favorite teacher Ms. Evans told students about divisors. Despite the fact that Valera loved math, he didn't find this particular topic interesting. Even more, it seemed so boring that he fell asleep in the middle of a lesson. And only a loud ringing of a school bell could interrupt his sweet dream.</span> </p><p><span class="tex-font-style-underline">Of course, the valuable material and the teacher's explanations were lost. However, Valera will one way or another have to do the homework. As he does not know the new material absolutely, he cannot do the job himself. That's why he asked you to help. You're his best friend after all, you just cannot refuse to help.</span> </p><p>Valera's home task has only one problem, which, though formulated in a very simple way, has not a trivial solution. Its statement looks as follows: if we consider all positive integers in the interval <span class="tex-span">[<i>a</i>;<i>b</i>]</span> then it is required to count the amount of such numbers in this interval that their <span class="tex-font-style-bf">smallest divisor</span> will be a certain integer <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">(you do not have to consider divisor equal to one)</span>. In other words, you should count the amount of such numbers from the interval <span class="tex-span">[<i>a</i>;<i>b</i>]</span>, that are not divisible by any number between <span class="tex-span">2</span> and <span class="tex-span"><i>k</i> - 1</span> and yet are divisible by <span class="tex-span"><i>k</i></span>. </p></div><div class="input-specification"><p>The first and only line contains three positive integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 2·10<sup class="upper-index">9</sup>, 2 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>). </p></div><div class="output-specification"><p>Print on a single line the answer to the given problem. </p></div>

## Input

<p>The first and only line contains three positive integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 2·10<sup class="upper-index">9</sup>, 2 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>). </p>

## Output

<p>Print on a single line the answer to the given problem. </p>





```input1
1 10 2

```




```input2
12 23 3

```




```input3
6 19 5

```




```output1
5

```




```output2
2

```




```output3
0

```



## Note

<p>Comments to the samples from the statement: </p><p>In the first sample the answer is numbers <span class="tex-span">2, 4, 6, 8, 10</span>.</p><p>In the second one — <span class="tex-span">15, 21</span></p><p>In the third one there are no such numbers.</p>
