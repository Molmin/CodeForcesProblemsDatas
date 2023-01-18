## Description

<div><p>You are playing a new famous fighting game: Kortal Mombat XII. You have to perform a brutality on your opponent's character.</p><p>You are playing the game on the new generation console so your gamepad have $26$ buttons. Each button has a single lowercase Latin letter from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' written on it. All the letters on buttons are pairwise distinct.</p><p>You are given a sequence of hits, the $i$-th hit deals $a_i$ units of damage to the opponent's character. To perform the $i$-th hit you have to press the button $s_i$ on your gamepad. Hits are numbered from $1$ to $n$.</p><p>You know that if you press some button <span class="tex-font-style-bf">more than</span> $k$ times <span class="tex-font-style-bf">in a row</span> then it'll break. You cherish your gamepad and don't want to break any of its buttons.</p><p>To perform a brutality you have to land some of the hits of the given sequence. <span class="tex-font-style-bf">You are allowed to skip any of them, however changing the initial order of the sequence is prohibited</span>. The total damage dealt is the sum of $a_i$ over all $i$ for the hits which weren't skipped.</p><p><span class="tex-font-style-bf">Note that if you skip the hit then the counter of consecutive presses the button won't reset</span>.</p><p>Your task is to skip some hits to deal the <span class="tex-font-style-bf">maximum</span> possible total damage to the opponent's character and not break your gamepad buttons.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$) — the number of hits and the maximum number of times you can push the same button in a row.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the damage of the $i$-th hit.</p><p>The third line of the input contains the string $s$ consisting of exactly $n$ lowercase Latin letters — the sequence of hits (each character is the letter on the button you need to press to perform the corresponding hit).</p></div><div class="output-specification"><p>Print one integer $dmg$ — the <span class="tex-font-style-bf">maximum</span> possible damage to the opponent's character you can deal without breaking your gamepad buttons.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$) — the number of hits and the maximum number of times you can push the same button in a row.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the damage of the $i$-th hit.</p><p>The third line of the input contains the string $s$ consisting of exactly $n$ lowercase Latin letters — the sequence of hits (each character is the letter on the button you need to press to perform the corresponding hit).</p>

## Output

<p>Print one integer $dmg$ — the <span class="tex-font-style-bf">maximum</span> possible damage to the opponent's character you can deal without breaking your gamepad buttons.</p>





```input1
7 3
1 5 16 18 7 2 10
baaaaca
```




```input2
5 5
2 4 1 3 1000
aaaaa
```




```input3
5 4
2 4 1 3 1000
aaaaa
```




```input4
8 1
10 15 2 1 4 8 15 16
qqwweerr
```




```input5
6 3
14 18 9 19 2 15
cccccc
```




```input6
2 1
10 10
qq
```




```output1
54
```




```output2
1010
```




```output3
1009
```




```output4
41
```




```output5
52
```




```output6
10
```



## Note

<p>In the first example you can choose hits with numbers $[1, 3, 4, 5, 6, 7]$ with the total damage $1 + 16 + 18 + 7 + 2 + 10 = 54$.</p><p>In the second example you can choose all hits so the total damage is $2 + 4 + 1 + 3 + 1000 = 1010$.</p><p>In the third example you can choose all hits expect the third one so the total damage is $2 + 4 + 3 + 1000 = 1009$.</p><p>In the fourth example you can choose hits with numbers $[2, 3, 6, 8]$. Only this way you can reach the maximum total damage $15 + 2 + 8 + 16 = 41$.</p><p>In the fifth example you can choose only hits with numbers $[2, 4, 6]$ with the total damage $18 + 19 + 15 = 52$.</p><p>In the sixth example you can change either first hit or the second hit (it does not matter) with the total damage $10$.</p>
