## Description

<div><p>The Fair Nut likes kvass very much. On his birthday parents presented him $n$ kegs of kvass. There are $v_i$ liters of kvass in the $i$-th keg. Each keg has a lever. You can pour your glass by <span class="tex-font-style-bf">exactly</span> $1$ liter pulling this lever. The Fair Nut likes this drink very much, so he wants to pour his glass by $s$ liters of kvass. But he wants to do it, so kvass level in the least keg is as much as possible.</p><p>Help him find out how much kvass can be in the least keg or define it's not possible to pour his glass by $s$ liters of kvass.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $s$ ($1 \le n \le 10^3$, $1 \le s \le 10^{12}$)&nbsp;— the number of kegs and glass volume.</p><p>The second line contains $n$ integers $v_1, v_2, \ldots, v_n$ ($1 \le v_i \le 10^9$)&nbsp;— the volume of $i$-th keg.</p></div><div class="output-specification"><p>If the Fair Nut cannot pour his glass by $s$ liters of kvass, print $-1$. Otherwise, print a single integer&nbsp;— how much kvass in the least keg can be.</p></div>

## Input

<p>The first line contains two integers $n$ and $s$ ($1 \le n \le 10^3$, $1 \le s \le 10^{12}$)&nbsp;— the number of kegs and glass volume.</p><p>The second line contains $n$ integers $v_1, v_2, \ldots, v_n$ ($1 \le v_i \le 10^9$)&nbsp;— the volume of $i$-th keg.</p>

## Output

<p>If the Fair Nut cannot pour his glass by $s$ liters of kvass, print $-1$. Otherwise, print a single integer&nbsp;— how much kvass in the least keg can be.</p>





```input1
3 3
4 3 5

```




```input2
3 4
5 3 4

```




```input3
3 7
1 2 3

```




```output1
3

```




```output2
2

```




```output3
-1

```



## Note

<p>In the first example, the answer is $3$, the Fair Nut can take $1$ liter from the first keg and $2$ liters from the third keg. There are $3$ liters of kvass in each keg.</p><p>In the second example, the answer is $2$, the Fair Nut can take $3$ liters from the first keg and $1$ liter from the second keg.</p><p>In the third example, the Fair Nut can't pour his cup by $7$ liters, so the answer is $-1$.</p>
