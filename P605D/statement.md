## Description

<div><p>You are playing a board card game. In this game the player has two characteristics, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— the white magic skill and the black magic skill, respectively. There are <span class="tex-span"><i>n</i></span> spell cards lying on the table, each of them has four characteristics, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. In one move a player can pick one of the cards and cast the spell written on it, but only if first two of it's characteristics meet the requirement <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i></span>, i.e. if the player has enough magic skill to cast this spell. However, after casting the spell the characteristics of a player change and become equal to <span class="tex-span"><i>x</i> = <i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i> = <i>d</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>At the beginning of the game both characteristics of a player are equal to zero. The goal of the game is to cast the <span class="tex-span"><i>n</i></span>-th spell. Your task is to make it in as few moves as possible. You are allowed to use spell in any order and any number of times (for example, you may not use some spells at all).</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cards on the table.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the characteristics of the corresponding card.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of moves needed to cast the <span class="tex-span"><i>n</i></span>-th spell and in the second line print <span class="tex-span"><i>k</i></span> numbers&nbsp;— the indices of the cards in the order in which you should cast them. In case there are multiple possible solutions, print any of them.</p><p>If it is impossible to cast the <span class="tex-span"><i>n</i></span>-th spell, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cards on the table.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the characteristics of the corresponding card.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of moves needed to cast the <span class="tex-span"><i>n</i></span>-th spell and in the second line print <span class="tex-span"><i>k</i></span> numbers&nbsp;— the indices of the cards in the order in which you should cast them. In case there are multiple possible solutions, print any of them.</p><p>If it is impossible to cast the <span class="tex-span"><i>n</i></span>-th spell, print <span class="tex-span"> - 1</span>.</p>





```input1
4
0 0 3 4
2 2 5 3
4 1 1 7
5 3 8 8

```




```input2
2
0 0 4 6
5 1 1000000000 1000000000

```




```output1
3
1 2 4

```




```output2
-1

```


