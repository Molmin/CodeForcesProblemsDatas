## Description

<div><p>Dima worked all day and wrote down on a long paper strip his favorite number $n$ consisting of $l$ digits. Unfortunately, the strip turned out to be so long that it didn't fit in the Dima's bookshelf.</p><p>To solve the issue, Dima decided to split the strip into two non-empty parts so that each of them contains a <span class="tex-font-style-bf">positive</span> integer without leading zeros. After that he will compute the sum of the two integers and write it down on a new strip.</p><p>Dima wants the resulting integer to be as small as possible, because it increases the chances that the sum will fit it in the bookshelf. Help Dima decide what is the minimum sum he can obtain.</p></div><div class="input-specification"><p>The first line contains a single integer $l$ ($2 \le l \le 100\,000$)&nbsp;— the length of the Dima's favorite number.</p><p>The second line contains the positive integer $n$ initially written on the strip: the Dima's favorite number.</p><p>The integer $n$ consists of exactly $l$ digits and it does not contain leading zeros. Dima guarantees, that there is at least one valid way to split the strip.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the smallest number Dima can obtain.</p></div>

## Input

<p>The first line contains a single integer $l$ ($2 \le l \le 100\,000$)&nbsp;— the length of the Dima's favorite number.</p><p>The second line contains the positive integer $n$ initially written on the strip: the Dima's favorite number.</p><p>The integer $n$ consists of exactly $l$ digits and it does not contain leading zeros. Dima guarantees, that there is at least one valid way to split the strip.</p>

## Output

<p>Print a single integer&nbsp;— the smallest number Dima can obtain.</p>





```input1
7
1234567
```




```input2
3
101
```




```output1
1801
```




```output2
11
```



## Note

<p>In the first example Dima can split the number $1234567$ into integers $1234$ and $567$. Their sum is $1801$.</p><p>In the second example Dima can split the number $101$ into integers $10$ and $1$. Their sum is $11$. Note that it is impossible to split the strip into "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">01</span>" since the numbers can't start with zeros.</p>
