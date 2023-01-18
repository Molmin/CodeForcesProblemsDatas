## Description

<div><p>In the capital city of Berland, Bertown, demonstrations are against the recent election of the King of Berland. Berland opposition, led by Mr. Ovalny, believes that the elections were not fair enough and wants to organize a demonstration at one of the squares.</p><p>Bertown has <span class="tex-span"><i>n</i></span> squares, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, they are numbered in the order of increasing distance between them and the city center. That is, square number <span class="tex-span">1</span> is central, and square number <span class="tex-span"><i>n</i></span> is the farthest from the center. Naturally, the opposition wants to hold a meeting as close to the city center as possible (that is, they want an square with the minimum number).</p><p>There are exactly <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &lt; <i>n</i>)</span> days left before the demonstration. Now all squares are free. But the Bertown city administration never sleeps, and the approval of an application for the demonstration threatens to become a very complex process. The process of approval lasts several days, but every day the following procedure takes place:</p><ul> <li> The opposition shall apply to hold a demonstration at a free square (the one which isn't used by the administration). </li><li> The administration tries to move the demonstration to the worst free square left. To do this, the administration organizes some long-term activities on the square, which is specified in the application of opposition. In other words, the administration starts using the square and it is no longer free. Then the administration proposes to move the opposition demonstration to the worst free square. If the opposition has applied for the worst free square <span class="tex-font-style-bf">then request is accepted and administration doesn't spend money</span>. If the administration does not have enough money to organize an event on the square in question, the opposition's application is accepted. If administration doesn't have enough money to organize activity, then rest of administration's money spends and application is accepted </li><li> If the application is not accepted, then the opposition can agree to the administration's proposal (that is, take the worst free square), or withdraw the current application and submit another one the next day. If there are no more days left before the meeting, the opposition has no choice but to agree to the proposal of City Hall. If application is accepted opposition can reject it. It means than opposition still can submit more applications later, <span class="tex-font-style-bf">but square remains free</span>. </li></ul><p>In order to organize an event on the square <span class="tex-span"><i>i</i></span>, the administration needs to spend <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bourles. Because of the crisis the administration has only <span class="tex-span"><i>b</i></span> bourles to confront the opposition. What is the best square that the opposition can take, if the administration will keep trying to occupy the square in question each time? Note that the administration's actions always depend only on the actions of the opposition.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number of squares and days left before the meeting, correspondingly (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>b</i></span> — the number of bourles the administration has (<span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the sum of money, needed to organise an event on square <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single number — the minimum number of the square where the opposition can organize the demonstration.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number of squares and days left before the meeting, correspondingly (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>b</i></span> — the number of bourles the administration has (<span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the sum of money, needed to organise an event on square <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single number — the minimum number of the square where the opposition can organize the demonstration.</p>





```input1
5 2
8
2 4 5 3 1

```




```input2
5 2
8
3 2 4 1 5

```




```input3
5 4
1000000000000000
5 4 3 2 1

```




```output1
2

```




```output2
5

```




```output3
5

```



## Note

<p>In the first sample the opposition can act like this. On day one it applies for square 3. The administration has to organize an event there and end up with 3 bourles. If on the second day the opposition applies for square 2, the administration won't have the money to intervene.</p><p>In the second sample the opposition has only the chance for the last square. If its first move occupies one of the first four squares, the administration is left with at least 4 bourles, which means that next day it can use its next move to move the opposition from any square to the last one.</p><p>In the third sample administration has a lot of money, so opposition can occupy only last square.</p>
