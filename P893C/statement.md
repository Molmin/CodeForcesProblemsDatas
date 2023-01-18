## Description

<div><p>Vova promised himself that he would never play computer games... But recently Firestorm — a well-known game developing company — published their newest game, World of Farcraft, and it became really popular. Of course, Vova started playing it.</p><p>Now he tries to solve a quest. The task is to come to a settlement named Overcity and spread a rumor in it.</p><p>Vova knows that there are <span class="tex-span"><i>n</i></span> characters in Overcity. Some characters are friends to each other, and they share information they got. Also Vova knows that he can bribe each character so he or she starts spreading the rumor; <span class="tex-span"><i>i</i></span>-th character wants <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> gold in exchange for spreading the rumor. When a character hears the rumor, he tells it to all his friends, and they start spreading the rumor to their friends (for free), and so on.</p><p>The quest is finished when all <span class="tex-span"><i>n</i></span> characters know the rumor. What is the minimum amount of gold Vova needs to spend in order to finish the quest?</p><p>Take a look at the notes if you think you haven't understood the problem completely.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of characters in Overcity and the number of pairs of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the amount of gold <span class="tex-span"><i>i</i></span>-th character asks to start spreading the rumor.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each containing a pair of numbers (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span>) which represent that characters <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are friends (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that each pair is listed at most once.</p></div><div class="output-specification"><p>Print one number — the minimum amount of gold Vova has to spend in order to finish the quest.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of characters in Overcity and the number of pairs of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the amount of gold <span class="tex-span"><i>i</i></span>-th character asks to start spreading the rumor.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each containing a pair of numbers (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span>) which represent that characters <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are friends (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that each pair is listed at most once.</p>

## Output

<p>Print one number — the minimum amount of gold Vova has to spend in order to finish the quest.</p>





```input1
5 2
2 5 3 4 8
1 4
4 5

```




```input2
10 0
1 2 3 4 5 6 7 8 9 10

```




```input3
10 5
1 6 2 7 3 8 4 9 5 10
1 2
3 4
5 6
7 8
9 10

```




```output1
10

```




```output2
55

```




```output3
15

```



## Note

<p>In the first example the best decision is to bribe the first character (he will spread the rumor to fourth character, and the fourth one will spread it to fifth). Also Vova has to bribe the second and the third characters, so they know the rumor.</p><p>In the second example Vova has to bribe everyone.</p><p>In the third example the optimal decision is to bribe the first, the third, the fifth, the seventh and the ninth characters.</p>
