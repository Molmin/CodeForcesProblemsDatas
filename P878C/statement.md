## Description

<div><p>Recently a tournament in <span class="tex-span"><i>k</i></span> kinds of sports has begun in Berland. Vasya wants to make money on the bets.</p><p>The scheme of the tournament is very mysterious and not fully disclosed. Competitions are held back to back, each of them involves two sportsmen who have not left the tournament yet. Each match can be held in any of the <span class="tex-span"><i>k</i></span> kinds of sport. Loser leaves the tournament. The last remaining sportsman becomes the winner. Apart of this, the scheme can be arbitrary, it is not disclosed in advance.</p><p>Vasya knows powers of sportsmen in each kind of sport. He believes that the sportsmen with higher power always wins.</p><p>The tournament is held every year, and each year one new participant joins it. In the first tournament, only one sportsman has participated, in the second there were two sportsmen, and so on. Vasya has been watching the tournament for the last <span class="tex-span"><i>n</i></span> years. Help him to find the number of possible winners for each of the <span class="tex-span"><i>n</i></span> tournaments.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>) — the number of tournaments and the number of kinds of sport, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>1</sub>, <i>s</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>s</i><sub class="lower-index"><i>ik</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>ij</i></sub></span> is the power of the <span class="tex-span"><i>i</i></span>-th sportsman in the <span class="tex-span"><i>j</i></span>-th kind of sport. The sportsman with higher powers always wins. It's guaranteed that for any kind of sport all of these powers are distinct.</p></div><div class="output-specification"><p>For each of the <span class="tex-span"><i>n</i></span> tournaments output the number of contenders who can win.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>) — the number of tournaments and the number of kinds of sport, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>1</sub>, <i>s</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>s</i><sub class="lower-index"><i>ik</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>ij</i></sub></span> is the power of the <span class="tex-span"><i>i</i></span>-th sportsman in the <span class="tex-span"><i>j</i></span>-th kind of sport. The sportsman with higher powers always wins. It's guaranteed that for any kind of sport all of these powers are distinct.</p>

## Output

<p>For each of the <span class="tex-span"><i>n</i></span> tournaments output the number of contenders who can win.</p>





```input1
3 2
1 5
5 1
10 10

```




```input2
3 2
2 2
3 3
1 10

```




```input3
3 2
2 3
1 1
3 2

```




```output1
1
2
1

```




```output2
1
1
3

```




```output3
1
1
2

```



## Note

<p>In the first sample:</p><p>In the first tournament there is only one sportsman, and he is the winner.</p><p>In the second tournament, there are two sportsmen, and everyone can defeat another, depending on kind of sports.</p><p>In the third tournament, the third sportsman in the strongest in both kinds of sports, so he is the winner regardless of the scheme.</p>
