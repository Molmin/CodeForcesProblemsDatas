## Description

<div><p>Polycarp has an array $a$ consisting of $n$ integers.</p><p>He wants to play a game with this array. The game consists of several moves. On the first move he chooses any element and deletes it (after the first move the array contains $n-1$ elements). For each of the next moves he chooses any element with the only restriction: its parity should differ from the parity of the element deleted on the previous move. In other words, he alternates parities (even-odd-even-odd-... or odd-even-odd-even-...) of the removed elements. Polycarp stops if he can't make a move.</p><p>Formally: </p><ul> <li> If it is the first move, he chooses any element and deletes it; </li><li> If it is the second or any next move: <ul> <li> if the last deleted element was <span class="tex-font-style-bf">odd</span>, Polycarp chooses any <span class="tex-font-style-bf">even</span> element and deletes it; </li><li> if the last deleted element was <span class="tex-font-style-bf">even</span>, Polycarp chooses any <span class="tex-font-style-bf">odd</span> element and deletes it. </li></ul> </li><li> If after some move Polycarp cannot make a move, the game ends. </li></ul><p>Polycarp's goal is to <span class="tex-font-style-bf">minimize</span> the sum of <span class="tex-font-style-bf">non-deleted</span> elements of the array after end of the game. If Polycarp can delete the whole array, then the sum of <span class="tex-font-style-bf">non-deleted</span> elements is zero.</p><p>Help Polycarp find this value.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2000$) — the number of elements of $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^6$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>Print one integer — the <span class="tex-font-style-bf">minimum</span> possible sum of <span class="tex-font-style-bf">non-deleted</span> elements of the array after end of the game.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2000$) — the number of elements of $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^6$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>Print one integer — the <span class="tex-font-style-bf">minimum</span> possible sum of <span class="tex-font-style-bf">non-deleted</span> elements of the array after end of the game.</p>





```input1
5
1 5 7 8 2
```




```input2
6
5 1 2 4 6 3
```




```input3
2
1000000 1000000
```




```output1
0
```




```output2
0
```




```output3
1000000
```


