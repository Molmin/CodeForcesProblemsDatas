## Description

<div><p>The Red Kingdom is attacked by the White King and the Black King!</p><p>The Kingdom is guarded by $n$ castles, the $i$-th castle is defended by $a_i$ soldiers. To conquer the Red Kingdom, the Kings have to eliminate all the defenders. </p><p>Each day the White King launches an attack on one of the castles. Then, at night, the forces of the Black King attack a castle (possibly the same one). Then the White King attacks a castle, then the Black King, and so on. The first attack is performed by the White King.</p><p>Each attack must target a castle with <span class="tex-font-style-bf">at least one</span> alive defender in it. There are three types of attacks:</p><ul> <li> a <span class="tex-font-style-it">mixed attack</span> decreases the number of defenders in the targeted castle by $x$ (or sets it to $0$ if there are already less than $x$ defenders); </li><li> an <span class="tex-font-style-it">infantry attack</span> decreases the number of defenders in the targeted castle by $y$ (or sets it to $0$ if there are already less than $y$ defenders); </li><li> a <span class="tex-font-style-it">cavalry attack</span> decreases the number of defenders in the targeted castle by $z$ (or sets it to $0$ if there are already less than $z$ defenders). </li></ul><p>The <span class="tex-font-style-it">mixed attack</span> can be launched at any valid target (at any castle with at least one soldier). However, the <span class="tex-font-style-it">infantry attack</span> cannot be launched if the <span class="tex-font-style-bf">previous attack on the targeted castle</span> had the same type, no matter when and by whom it was launched. The same applies to the <span class="tex-font-style-it">cavalry attack</span>. A castle that was not attacked at all can be targeted by any type of attack.</p><p>The King who launches the last attack will be glorified as the conqueror of the Red Kingdom, so both Kings want to launch the last attack (and they are wise enough to find a strategy that allows them to do it no matter what are the actions of their opponent, if such strategy exists). The White King is leading his first attack, and you are responsible for planning it. Can you calculate the number of possible options for the first attack that allow the White King to launch the last attack? Each option for the first attack is represented by the targeted castle and the type of attack, and two options are different if the targeted castles or the types of attack are different.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Then, the test cases follow. Each test case is represented by two lines. </p><p>The first line contains four integers $n$, $x$, $y$ and $z$ ($1 \le n \le 3 \cdot 10^5$, $1 \le x, y, z \le 5$). </p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^{18}$).</p><p>It is guaranteed that the sum of values of $n$ over all test cases in the input does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the answer to it: the number of possible options for the first attack of the White King (or $0$, if the Black King can launch the last attack no matter how the White King acts).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Then, the test cases follow. Each test case is represented by two lines. </p><p>The first line contains four integers $n$, $x$, $y$ and $z$ ($1 \le n \le 3 \cdot 10^5$, $1 \le x, y, z \le 5$). </p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^{18}$).</p><p>It is guaranteed that the sum of values of $n$ over all test cases in the input does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print the answer to it: the number of possible options for the first attack of the White King (or $0$, if the Black King can launch the last attack no matter how the White King acts).</p>





```input1
3
2 1 3 4
7 6
1 1 2 3
1
1 1 2 2
3
```




```input2
10
6 5 4 5
2 3 2 3 1 3
1 5 2 3
10
4 4 2 3
8 10 8 5
2 2 1 4
8 5
3 5 3 5
9 2 10
4 5 5 5
2 10 4 2
2 3 1 4
1 10
3 1 5 3
9 8 7
2 5 4 5
8 8
3 5 1 4
5 5 10
```




```output1
2
3
0
```




```output2
0
2
1
2
5
12
5
0
0
2
```


