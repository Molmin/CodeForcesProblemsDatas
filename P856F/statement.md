## Description

<div><p>Vasya and Petya are playing an online game. As most online games, it has hero progress system that allows players to gain experience that make their heroes stronger. Of course, Vasya would like to get as many experience points as possible. After careful study of experience points allocation, he found out that if he plays the game alone, he gets one experience point each second. However, if two players are playing together, and their current experience values differ by at most <span class="tex-span"><i>C</i></span> points, they can boost their progress, and each of them gets 2 experience points each second.</p><p>Since Vasya and Petya are middle school students, their parents don't allow them to play all the day around. Each of the friends has his own schedule: Vasya can only play during intervals <span class="tex-span">[<i>a</i><sub class="lower-index">1</sub>;<i>b</i><sub class="lower-index">1</sub>], [<i>a</i><sub class="lower-index">2</sub>;<i>b</i><sub class="lower-index">2</sub>], ..., [<i>a</i><sub class="lower-index"><i>n</i></sub>;<i>b</i><sub class="lower-index"><i>n</i></sub>]</span>, and Petya can only play during intervals <span class="tex-span">[<i>c</i><sub class="lower-index">1</sub>;<i>d</i><sub class="lower-index">1</sub>], [<i>c</i><sub class="lower-index">2</sub>;<i>d</i><sub class="lower-index">2</sub>], ..., [<i>c</i><sub class="lower-index"><i>m</i></sub>;<i>d</i><sub class="lower-index"><i>m</i></sub>]</span>. All time periods are given in seconds from the current moment. Vasya is good in math, so he has noticed that sometimes it can be profitable not to play alone, because experience difference could become too big, and progress would not be boosted even when played together.</p><p>Now they would like to create such schedule of playing that Vasya's final experience was greatest possible. The current players experience is the same. Petya is not so concerned about his experience, so he is ready to cooperate and play when needed to maximize Vasya's experience.</p></div><div class="input-specification"><p>The first line of input data contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>C</i></span> — the number of intervals when Vasya can play, the number of intervals when Petya can play, and the maximal difference in experience level when playing together still gives a progress boost (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>C</i> ≤ 10<sup class="upper-index">18</sup></span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain two integers each: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— intervals when Vasya can play (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain two integers each: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— intervals when Petya can play (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> &lt; <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximal experience that Vasya can have in the end, if both players try to maximize this value.</p></div>

## Input

<p>The first line of input data contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>C</i></span> — the number of intervals when Vasya can play, the number of intervals when Petya can play, and the maximal difference in experience level when playing together still gives a progress boost (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>C</i> ≤ 10<sup class="upper-index">18</sup></span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain two integers each: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— intervals when Vasya can play (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain two integers each: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— intervals when Petya can play (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> &lt; <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p>

## Output

<p>Output one integer&nbsp;— the maximal experience that Vasya can have in the end, if both players try to maximize this value.</p>





```input1
2 1 5
1 7
10 20
10 20

```




```input2
1 2 5
0 100
20 60
85 90

```




```output1
25

```




```output2
125

```


