## Description

<div><p>Astronaut Natasha arrived on Mars. She knows that the Martians are very poor aliens. To ensure a better life for the Mars citizens, their emperor decided to take tax from every tourist who visited the planet. Natasha is the inhabitant of Earth, therefore she had to pay the tax to enter the territory of Mars.</p><p>There are $n$ banknote denominations on Mars: the value of $i$-th banknote is $a_i$. Natasha has an infinite number of banknotes of each denomination.</p><p>Martians have $k$ fingers on their hands, so they use a number system with base $k$. In addition, the Martians consider the digit $d$ (in the number system with base $k$) divine. Thus, if the last digit in Natasha's tax amount written in the number system with the base $k$ is $d$, the Martians will be happy. Unfortunately, Natasha does not know the Martians' divine digit yet.</p><p>Determine for which values $d$ Natasha can make the Martians happy.</p><p>Natasha can use only her banknotes. Martians don't give her change.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 100\,000$, $2 \le k \le 100\,000$)&nbsp;— the number of denominations of banknotes and the base of the number system on Mars.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— denominations of banknotes on Mars.</p><p>All numbers are given in decimal notation.</p></div><div class="output-specification"><p>On the first line output the number of values $d$ for which Natasha can make the Martians happy.</p><p>In the second line, output all these values in increasing order.</p><p>Print all numbers in decimal notation.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 100\,000$, $2 \le k \le 100\,000$)&nbsp;— the number of denominations of banknotes and the base of the number system on Mars.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— denominations of banknotes on Mars.</p><p>All numbers are given in decimal notation.</p>

## Output

<p>On the first line output the number of values $d$ for which Natasha can make the Martians happy.</p><p>In the second line, output all these values in increasing order.</p><p>Print all numbers in decimal notation.</p>





```input1
2 8
12 20

```




```input2
3 10
10 20 30

```




```output1
2
0 4
```




```output2
1
0
```



## Note

<p>Consider the first test case. It uses the octal number system.</p><p>If you take one banknote with the value of $12$, you will get $14_8$ in octal system. The last digit is $4_8$.</p><p>If you take one banknote with the value of $12$ and one banknote with the value of $20$, the total value will be $32$. In the octal system, it is $40_8$. The last digit is $0_8$.</p><p>If you take two banknotes with the value of $20$, the total value will be $40$, this is $50_8$ in the octal system. The last digit is $0_8$.</p><p>No other digits other than $0_8$ and $4_8$ can be obtained. Digits $0_8$ and $4_8$ could also be obtained in other ways.</p><p>The second test case uses the decimal number system. The nominals of all banknotes end with zero, so Natasha can give the Martians only the amount whose decimal notation also ends with zero.</p>
