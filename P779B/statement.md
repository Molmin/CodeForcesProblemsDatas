## Description

<div><p>Polycarp is crazy about round numbers. He especially likes the numbers divisible by <span class="tex-span">10<sup class="upper-index"><i>k</i></sup></span>.</p><p>In the given number of <span class="tex-span"><i>n</i></span> Polycarp wants to remove the least number of digits to get a number that is divisible by <span class="tex-span">10<sup class="upper-index"><i>k</i></sup></span>. For example, if <span class="tex-span"><i>k</i> = 3</span>, in the number <span class="tex-font-style-tt">30020</span> it is enough to delete a single digit (<span class="tex-font-style-tt">2</span>). In this case, the result is <span class="tex-font-style-tt">3000</span> that is divisible by <span class="tex-span">10<sup class="upper-index">3</sup> = 1000</span>.</p><p>Write a program that prints the minimum number of digits to be deleted from the given integer number <span class="tex-span"><i>n</i></span>, so that the result is divisible by <span class="tex-span">10<sup class="upper-index"><i>k</i></sup></span>. The result should not start with the unnecessary leading zero (i.e., zero can start only the number <span class="tex-font-style-tt">0</span>, which is required to be written as exactly one digit).</p><p>It is guaranteed that the answer exists.</p></div><div class="input-specification"><p>The only line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 2 000 000 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 9</span>).</p><p>It is guaranteed that the answer exists. All numbers in the input are written in traditional notation of integers, that is, without any extra leading zeros.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>w</i></span> — the required minimal number of digits to erase. After removing the appropriate <span class="tex-span"><i>w</i></span> digits from the number <span class="tex-span"><i>n</i></span>, the result should have a value that is divisible by <span class="tex-span">10<sup class="upper-index"><i>k</i></sup></span>. The result can start with digit <span class="tex-font-style-tt">0</span> in the single case (the result is zero and written by exactly the only digit <span class="tex-font-style-tt">0</span>).</p></div>

## Input

<p>The only line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 2 000 000 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 9</span>).</p><p>It is guaranteed that the answer exists. All numbers in the input are written in traditional notation of integers, that is, without any extra leading zeros.</p>

## Output

<p>Print <span class="tex-span"><i>w</i></span> — the required minimal number of digits to erase. After removing the appropriate <span class="tex-span"><i>w</i></span> digits from the number <span class="tex-span"><i>n</i></span>, the result should have a value that is divisible by <span class="tex-span">10<sup class="upper-index"><i>k</i></sup></span>. The result can start with digit <span class="tex-font-style-tt">0</span> in the single case (the result is zero and written by exactly the only digit <span class="tex-font-style-tt">0</span>).</p>





```input1
30020 3

```




```input2
100 9

```




```input3
10203049 2

```




```output1
1

```




```output2
2

```




```output3
3

```



## Note

<p>In the example 2 you can remove two digits: 1 and any 0. The result is number 0 which is divisible by any number.</p>
