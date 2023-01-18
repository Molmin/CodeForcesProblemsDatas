## Description

<div><p>Efim just received his grade for the last test. He studies in a special school and his grade can be equal to any positive decimal fraction. First he got disappointed, as he expected a way more pleasant result. Then, he developed a tricky plan. Each second, he can ask his teacher to round the grade at any place after the decimal point (also, he can ask to round to the nearest integer). </p><p>There are <span class="tex-span"><i>t</i></span> seconds left till the end of the break, so Efim has to act fast. Help him find what is the maximum grade he can get in no more than <span class="tex-span"><i>t</i></span> seconds. Note, that he can choose to not use all <span class="tex-span"><i>t</i></span> seconds. Moreover, he can even choose to not round the grade at all.</p><p>In this problem, classic rounding rules are used: while rounding number to the <span class="tex-span"><i>n</i></span>-th digit one has to take a look at the digit <span class="tex-span"><i>n</i> + 1</span>. If it is less than <span class="tex-span">5</span> than the <span class="tex-span"><i>n</i></span>-th digit remain unchanged while all subsequent digits are replaced with <span class="tex-span">0</span>. Otherwise, if the <span class="tex-span"><i>n</i> + 1</span> digit is greater or equal to <span class="tex-span">5</span>, the digit at the position <span class="tex-span"><i>n</i></span> is increased by <span class="tex-span">1</span> (this might also change some other digits, if this one was equal to <span class="tex-span">9</span>) and all subsequent digits are replaced with <span class="tex-span">0</span>. At the end, all trailing zeroes are thrown away.</p><p>For example, if the number <span class="tex-span">1.14</span> is rounded to the first decimal place, the result is <span class="tex-span">1.1</span>, while if we round <span class="tex-span">1.5</span> to the nearest integer, the result is <span class="tex-span">2</span>. Rounding number <span class="tex-span">1.299996121</span> in the fifth decimal place will result in number <span class="tex-span">1.3</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of Efim's grade and the number of seconds till the end of the break respectively.</p><p>The second line contains the grade itself. It's guaranteed that the grade is a positive number, containing at least one digit after the decimal points, and it's representation doesn't finish with <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>Print the maximum grade that Efim can get in <span class="tex-span"><i>t</i></span> seconds. Do not print trailing zeroes.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of Efim's grade and the number of seconds till the end of the break respectively.</p><p>The second line contains the grade itself. It's guaranteed that the grade is a positive number, containing at least one digit after the decimal points, and it's representation doesn't finish with <span class="tex-span">0</span>.</p>

## Output

<p>Print the maximum grade that Efim can get in <span class="tex-span"><i>t</i></span> seconds. Do not print trailing zeroes.</p>





```input1
6 1
10.245

```




```input2
6 2
10.245

```




```input3
3 100
9.2

```




```output1
10.25

```




```output2
10.3

```




```output3
9.2

```



## Note

<p>In the first two samples Efim initially has grade <span class="tex-span">10.245</span>. </p><p>During the first second Efim can obtain grade <span class="tex-span">10.25</span>, and then <span class="tex-span">10.3</span> during the next second. Note, that the answer <span class="tex-span">10.30</span> will be considered incorrect.</p><p>In the third sample the optimal strategy is to not perform any rounding at all.</p>
