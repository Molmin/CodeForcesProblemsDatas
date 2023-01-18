## Description

<div><p>You are going to work in Codeforces as an intern in a team of <span class="tex-span"><i>n</i></span> engineers, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. You want to give each engineer a souvenir: a T-shirt from your country (T-shirts are highly desirable in Codeforces). Unfortunately you don't know the size of the T-shirt each engineer fits in. There are <span class="tex-span"><i>m</i></span> different sizes, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>m</i></span>, and each engineer will fit in a T-shirt of exactly one size.</p><p>You don't know the engineers' exact sizes, so you asked your friend, Gerald. Unfortunately, he wasn't able to obtain the exact sizes either, but he managed to obtain for each engineer <span class="tex-span"><i>i</i></span> and for all sizes <span class="tex-span"><i>j</i></span>, the probability that the size of the T-shirt that fits engineer <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>j</i></span>.</p><p>Since you're planning to give each engineer one T-shirt, you are going to bring with you exactly <span class="tex-span"><i>n</i></span> T-shirts. For those <span class="tex-span"><i>n</i></span> T-shirts, you can bring any combination of sizes (you can bring multiple T-shirts with the same size too!). You don't know the sizes of T-shirts for each engineer when deciding what sizes to bring, so you have to pick this combination based only on the probabilities given by your friend, Gerald. </p><p>Your task is to maximize the expected number of engineers that receive a T-shirt of his size. </p><p>This is defined more formally as follows. When you finally arrive at the office, you will ask each engineer his T-shirt size. Then, if you still have a T-shirt of that size, you will give him one of them. Otherwise, you don't give him a T-shirt. You will ask the engineers in order starting from engineer <span class="tex-span">1</span>, then engineer <span class="tex-span">2</span>, and so on until engineer <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000, 1 ≤ <i>m</i> ≤ 300)</span>, denoting the number of engineers and the number of T-shirt sizes, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line represents the probability that the <span class="tex-span"><i>i</i></span>-th engineer fits in a T-shirt of size <span class="tex-span"><i>j</i></span>. Each probability will be given as an integer between <span class="tex-span">0</span> and <span class="tex-span">1000</span>, inclusive. The actual probability should be calculated as the given number divided by <span class="tex-span">1000</span>. </p><p>It is guaranteed that for any engineer, the sum of the probabilities for all <span class="tex-span"><i>m</i></span> T-shirts is equal to one.</p></div><div class="output-specification"><p>Print a single real number denoting the maximum possible expected number of engineers that will receive a T-shirt.</p><p>For the answer the absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span> is acceptable.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000, 1 ≤ <i>m</i> ≤ 300)</span>, denoting the number of engineers and the number of T-shirt sizes, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line represents the probability that the <span class="tex-span"><i>i</i></span>-th engineer fits in a T-shirt of size <span class="tex-span"><i>j</i></span>. Each probability will be given as an integer between <span class="tex-span">0</span> and <span class="tex-span">1000</span>, inclusive. The actual probability should be calculated as the given number divided by <span class="tex-span">1000</span>. </p><p>It is guaranteed that for any engineer, the sum of the probabilities for all <span class="tex-span"><i>m</i></span> T-shirts is equal to one.</p>

## Output

<p>Print a single real number denoting the maximum possible expected number of engineers that will receive a T-shirt.</p><p>For the answer the absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span> is acceptable.</p>





```input1
2 2
500 500
500 500

```




```input2
3 3
1000 0 0
1000 0 0
0 1000 0

```




```input3
1 4
100 200 300 400

```




```output1
1.500000000000

```




```output2
3.000000000000

```




```output3
0.400000000000

```



## Note

<p>For the first example, bring one T-shirt of each size. With <span class="tex-span">0.5</span> chance, either both engineers fit inside T-shirts of size <span class="tex-span">1</span> or both fit inside T-shirts of size <span class="tex-span">2</span>. With the other <span class="tex-span">0.5</span> chance, one engineer fits inside a T-shirt of size <span class="tex-span">1</span> and the other inside a T-shirt of size <span class="tex-span">2</span>. If the first is true, the number of engineers that receive a T-shirt is one. If the second is true, the number of such engineers is two. Hence, the expected number of engineers who receive a T-shirt is <span class="tex-span">1.5</span>. This is maximum possible expected number of engineers for all sets of T-shirts. </p><p>For the second example, bring two T-shirts of size <span class="tex-span">1</span> and one T-shirt of size <span class="tex-span">2</span>. This way, each engineer will definitely receive a T-shirt of his size.</p><p>For the third example, bring one T-shirt of size <span class="tex-span">4</span>.</p>
