## Description

<div><p>Ilya is working for the company that constructs robots. Ilya writes programs for entertainment robots, and his current project is "Bob", a new-generation game robot. Ilya's boss wants to know his progress so far. Especially he is interested if Bob is better at playing different games than the previous model, "Alice". </p><p>So now Ilya wants to compare his robots' performance in a simple game called "1-2-3". This game is similar to the "Rock-Paper-Scissors" game: both robots secretly choose a number from the set <span class="tex-span">{1, 2, 3}</span> and say it at the same moment. If both robots choose the same number, then it's a draw and noone gets any points. But if chosen numbers are different, then one of the robots gets a point: <span class="tex-span">3</span> beats <span class="tex-span">2</span>, <span class="tex-span">2</span> beats <span class="tex-span">1</span> and <span class="tex-span">1</span> beats <span class="tex-span">3</span>. </p><p>Both robots' programs make them choose their numbers in such a way that their choice in <span class="tex-span">(<i>i</i> + 1)</span>-th game depends only on the numbers chosen by them in <span class="tex-span"><i>i</i></span>-th game. </p><p>Ilya knows that the robots will play <span class="tex-span"><i>k</i></span> games, Alice will choose number <span class="tex-span"><i>a</i></span> in the first game, and Bob will choose <span class="tex-span"><i>b</i></span> in the first game. He also knows both robots' programs and can tell what each robot will choose depending on their choices in previous game. Ilya doesn't want to wait until robots play all <span class="tex-span"><i>k</i></span> games, so he asks you to predict the number of points they will have after the final game. </p></div><div class="input-specification"><p>The first line contains three numbers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 3</span>). </p><p>Then <span class="tex-span">3</span> lines follow, <span class="tex-span"><i>i</i></span>-th of them containing <span class="tex-span">3</span> numbers <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 2</sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 3</sub></span>, where <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> represents Alice's choice in the game if Alice chose <span class="tex-span"><i>i</i></span> in previous game and Bob chose <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 3</span>). </p><p>Then <span class="tex-span">3</span> lines follow, <span class="tex-span"><i>i</i></span>-th of them containing <span class="tex-span">3</span> numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 2</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 3</sub></span>, where <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> represents Bob's choice in the game if Alice chose <span class="tex-span"><i>i</i></span> in previous game and Bob chose <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>B</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 3</span>). </p></div><div class="output-specification"><p>Print two numbers. First of them has to be equal to the number of points Alice will have, and second of them must be Bob's score after <span class="tex-span"><i>k</i></span> games.</p></div>

## Input

<p>The first line contains three numbers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 3</span>). </p><p>Then <span class="tex-span">3</span> lines follow, <span class="tex-span"><i>i</i></span>-th of them containing <span class="tex-span">3</span> numbers <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 2</sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, 3</sub></span>, where <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> represents Alice's choice in the game if Alice chose <span class="tex-span"><i>i</i></span> in previous game and Bob chose <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 3</span>). </p><p>Then <span class="tex-span">3</span> lines follow, <span class="tex-span"><i>i</i></span>-th of them containing <span class="tex-span">3</span> numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 2</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, 3</sub></span>, where <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> represents Bob's choice in the game if Alice chose <span class="tex-span"><i>i</i></span> in previous game and Bob chose <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>B</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 3</span>). </p>

## Output

<p>Print two numbers. First of them has to be equal to the number of points Alice will have, and second of them must be Bob's score after <span class="tex-span"><i>k</i></span> games.</p>





```input1
10 2 1
1 1 1
1 1 1
1 1 1
2 2 2
2 2 2
2 2 2

```




```input2
8 1 1
2 2 1
3 3 1
3 1 3
1 1 1
2 1 1
1 2 3

```




```input3
5 1 1
1 2 2
2 2 2
2 2 2
1 2 2
2 2 2
2 2 2

```




```output1
1 9

```




```output2
5 2

```




```output3
0 0

```



## Note

<p>In the second example game goes like this:</p><p><img align="middle" class="tex-formula" src="file://sYskMLvu.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The fourth and the seventh game are won by Bob, the first game is draw and the rest are won by Alice.</p>
