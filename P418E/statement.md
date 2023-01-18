## Description

<div><p>In order to ensure confidentiality, the access to the "Russian Code Cup" problems is password protected during the problem development process.</p><p>To select a password, the jury can generate a special table that contains <span class="tex-span"><i>n</i></span> columns and the infinite number of rows. To construct a table, the first row is fixed, and all the others are obtained by the following rule:</p><p>In the row <span class="tex-span"><i>i</i></span> at position <span class="tex-span"><i>p</i></span> there is a number equal to the number of times <span class="tex-span"><i>a</i>[<i>i</i> - 1][<i>p</i>]</span> occurs on the prefix <span class="tex-span"><i>a</i>[<i>i</i> - 1][1... <i>p</i>]</span>.</p><p>To ensure the required level of confidentiality, the jury must be able to perform the following operations: </p><ul> <li> Replace number <span class="tex-span"><i>a</i>[1][<i>p</i>]</span> by <span class="tex-span"><i>v</i></span> and rebuild the table. </li><li> Find the number <span class="tex-span"><i>a</i>[<i>x</i>][<i>y</i>]</span>, which will be the new password. </li></ul><p>Doing all these steps manually is very tedious, so the jury asks you to help him. Write a program that responds to the request of the jury.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of columns. The second line contains the description of the first row of the table, that is, <span class="tex-span"><i>n</i></span> integers, which are not less than <span class="tex-span">1</span> and do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>The third line of the input contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100000</span>) — the number of requests.</p><p>Next, each row contains a description of the request, which consists of three integers: </p><ul> <li> If the first number is equal to <span class="tex-span">1</span>, then the remaining two numbers are <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>). So, you should put value <span class="tex-span"><i>v</i></span> in the position <span class="tex-span"><i>p</i></span> in the first row. </li><li> If the first number is equal to <span class="tex-span">2</span>, then the remaining two numbers are <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>y</i> ≤ <i>n</i></span>) — the row and column of the table cell from which you want to get value. </li></ul></div><div class="output-specification"><p>Print an answer for each request of the second type in the order you receive them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of columns. The second line contains the description of the first row of the table, that is, <span class="tex-span"><i>n</i></span> integers, which are not less than <span class="tex-span">1</span> and do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>The third line of the input contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100000</span>) — the number of requests.</p><p>Next, each row contains a description of the request, which consists of three integers: </p><ul> <li> If the first number is equal to <span class="tex-span">1</span>, then the remaining two numbers are <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>). So, you should put value <span class="tex-span"><i>v</i></span> in the position <span class="tex-span"><i>p</i></span> in the first row. </li><li> If the first number is equal to <span class="tex-span">2</span>, then the remaining two numbers are <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>y</i> ≤ <i>n</i></span>) — the row and column of the table cell from which you want to get value. </li></ul>

## Output

<p>Print an answer for each request of the second type in the order you receive them.</p>





```input1
6
1 2 2 2 3 1
3
2 2 3
1 3 3
2 3 4

```




```output1
2
1

```


