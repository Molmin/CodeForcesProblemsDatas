## Description

<div><p>Petya and Vasya are competing with each other in a new interesting game as they always do.</p><p>At the beginning of the game Petya has to come up with an array of $N$ positive integers. Sum of all elements in his array should be equal to $S$. Then Petya has to select an integer $K$ such that $0 \leq K \leq S$.</p><p>In order to win, Vasya has to find a non-empty subarray in Petya's array such that the sum of all selected elements equals to either $K$ or $S - K$. Otherwise Vasya loses.</p><p>You are given integers $N$ and $S$. You should determine if Petya can win, considering Vasya plays optimally. If Petya can win, help him to do that.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $S$ ($1 \leq N \leq S \leq 10^{6}$)&nbsp;— the required length of the array and the required sum of its elements.</p></div><div class="output-specification"><p>If Petya can win, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. Then print Petya's array in the second line. The array should contain $N$ positive integers with sum equal to $S$. In the third line print $K$. If there are many correct answers, you can print any of them.</p><p>If Petya can't win, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any register (lowercase or uppercase).</p></div>

## Input

<p>The first line contains two integers $N$ and $S$ ($1 \leq N \leq S \leq 10^{6}$)&nbsp;— the required length of the array and the required sum of its elements.</p>

## Output

<p>If Petya can win, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. Then print Petya's array in the second line. The array should contain $N$ positive integers with sum equal to $S$. In the third line print $K$. If there are many correct answers, you can print any of them.</p><p>If Petya can't win, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any register (lowercase or uppercase).</p>





```input1
1 4
```




```input2
3 4
```




```input3
3 8
```




```output1
YES
4
2
```




```output2
NO
```




```output3
YES
2 1 5
4
```


