## Description

<div><p>The programmers from the R2 company love playing 2048. One day, they decided to invent their own simplified version of this game — <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> on a stripe.</p><p>Imagine an infinite in one direction stripe, consisting of unit squares (the side of each square is equal to the height of the stripe). Each square can either be empty or contain some number.</p><p>Initially, all squares are empty. Then at infinity one of the unit squares number 2 or 4 appears. Then the player presses a button once, and the appeared number begins to move towards the beginning of the stripe. Let's assume that some number <span class="tex-span"><i>x</i></span> moves to the beginning of the stripe, then it will stop if:</p><ol> <li> it either gets in the first square of the stripe; </li><li> or it is in the square that is preceded by a square with number <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>y</i> ≠ <i>x</i>)</span>. But if number <span class="tex-span"><i>x</i></span> at some point of time gets to the square with the same number then both numbers add to each other and result in <span class="tex-span">2<i>x</i></span>. The new number <span class="tex-span">2<i>x</i></span> continues moving to the beginning of the stripe by the same rules. </li></ol><p>After the final stop of the number moving process, the infinity gets a new number 2 or 4 and the process repeats. Read the notes to the test samples to better understand the moving strategy.</p><p>I guess you've understood that the game progress fully depends on the order in which numbers 2 and 4 appear. Let's look at some sequence of numbers 2 and 4 in the game. We assume that the sequence is <span class="tex-font-style-it">winning</span> if it results in at least one square getting the number greater or equal than <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span>. </p><p>The goal of the game is to make up a winning sequence of <span class="tex-span"><i>n</i></span> numbers. But not everything is so simple, some numbers in the sequence are identified beforehand. You are given a sequence consisting of numbers 0, 2, 4. Count how many ways there are to replace each 0 of the sequence with 2 or 4 to get a winning sequence.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000;&nbsp;3 ≤ <i>k</i> ≤ 11)</span>. The next line contains sequence of <span class="tex-span"><i>n</i></span> integers, each of them is either 0, or 2, or 4.</p></div><div class="output-specification"><p>Print a single integer — the number of ways to replace zeroes by numbers 2 or 4 to get a winning sequence. As this number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000;&nbsp;3 ≤ <i>k</i> ≤ 11)</span>. The next line contains sequence of <span class="tex-span"><i>n</i></span> integers, each of them is either 0, or 2, or 4.</p>

## Output

<p>Print a single integer — the number of ways to replace zeroes by numbers 2 or 4 to get a winning sequence. As this number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
7 4
2 2 4 2 2 2 2

```




```input2
1 3
0

```




```input3
2 3
0 4

```




```input4
5 4
2 0 0 4 4

```




```output1
1

```




```output2
0

```




```output3
1

```




```output4
2

```



## Note

<p>Consider the first example. The beginning of the strip will look as follows: </p><p><span class="tex-font-style-tt">2</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">4</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">8</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">8 2</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">8 4</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">8 4 2</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">16</span>.</p><p>To better understand the game, you can see the original game on <span class="tex-font-style-tt">http://gabrielecirulli.github.io/2048/</span>. Please note that the game that is described on the strip is slightly different from the original game (when the two numbers add up in the original game, they do not keep moving). Be careful, the game is addictive, there isn't much time for the contest!</p>
