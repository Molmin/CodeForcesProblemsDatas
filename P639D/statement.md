## Description

<div><p>Codeforces is a wonderful platform and one its feature shows how much someone contributes to the community. Every registered user has <span class="tex-font-style-it">contribution</span>&nbsp;— an integer number, not necessarily positive. There are <span class="tex-span"><i>n</i></span> registered users and the <span class="tex-span"><i>i</i></span>-th of them has contribution <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Limak is a little polar bear and he's new into competitive programming. He doesn't even have an account in Codeforces but he is able to upvote existing blogs and comments. We assume that every registered user has infinitely many blogs and comments.</p><ul> <li> Limak can spend <span class="tex-span"><i>b</i></span> minutes to read one blog and upvote it. Author's contribution will be increased by <span class="tex-span">5</span>. </li><li> Limak can spend <span class="tex-span"><i>c</i></span> minutes to read one comment and upvote it. Author's contribution will be increased by <span class="tex-span">1</span>. </li></ul><p>Note that it's possible that Limak reads blogs faster than comments.</p><p>Limak likes ties. He thinks it would be awesome to see a tie between at least <span class="tex-span"><i>k</i></span> registered users. To make it happen he is going to spend some time on reading and upvoting. After that, there should exist an integer value <span class="tex-span"><i>x</i></span> that at least <span class="tex-span"><i>k</i></span> registered users have contribution exactly <span class="tex-span"><i>x</i></span>.</p><p>How much time does Limak need to achieve his goal?</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>b</i>, <i>c</i> ≤ 1000</span>)&nbsp;— the number of registered users, the required minimum number of users with the same contribution, time needed to read and upvote a blog, and time needed to read and upvote a comment, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>t</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes contribution of the <span class="tex-span"><i>i</i></span>-th registered user.</p></div><div class="output-specification"><p>Print the minimum number of minutes Limak will spend to get a tie between at least <span class="tex-span"><i>k</i></span> registered users.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>b</i>, <i>c</i> ≤ 1000</span>)&nbsp;— the number of registered users, the required minimum number of users with the same contribution, time needed to read and upvote a blog, and time needed to read and upvote a comment, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>t</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes contribution of the <span class="tex-span"><i>i</i></span>-th registered user.</p>

## Output

<p>Print the minimum number of minutes Limak will spend to get a tie between at least <span class="tex-span"><i>k</i></span> registered users.</p>





```input1
4 3 100 30
12 2 6 1

```




```input2
4 3 30 100
12 2 6 1

```




```input3
6 2 987 789
-8 42 -4 -65 -8 -8

```




```output1
220

```




```output2
190

```




```output3
0

```



## Note

<p>In the first sample, there are <span class="tex-span">4</span> registered users and Limak wants a tie between at least <span class="tex-span">3</span> of them. Limak should behave as follows.</p><ul> <li> He spends <span class="tex-span">100</span> minutes to read one blog of the <span class="tex-span">4</span>-th user and increase his contribution from <span class="tex-span">1</span> to <span class="tex-span">6</span>. </li><li> Then he spends <span class="tex-span">4·30 = 120</span> minutes to read four comments of the <span class="tex-span">2</span>-nd user and increase his contribution from <span class="tex-span">2</span> to <span class="tex-span">6</span> (four times it was increaded by <span class="tex-span">1</span>). </li></ul><p>In the given scenario, Limak spends <span class="tex-span">100 + 4·30 = 220</span> minutes and after that each of users <span class="tex-span">2, 3, 4</span> has contribution <span class="tex-span">6</span>.</p><p>In the second sample, Limak needs <span class="tex-span">30</span> minutes to read a blog and <span class="tex-span">100</span> minutes to read a comment. This time he can get <span class="tex-span">3</span> users with contribution equal to <span class="tex-span">12</span> by spending <span class="tex-span">100 + 3·30 = 190</span> minutes:</p><ul> <li> Spend <span class="tex-span">2·30 = 60</span> minutes to read two blogs of the <span class="tex-span">1</span>-st user to increase his contribution from <span class="tex-span">2</span> to <span class="tex-span">12</span>. </li><li> Spend <span class="tex-span">30 + 100</span> minutes to read one blog and one comment of the <span class="tex-span">3</span>-rd user. His contribution will change from <span class="tex-span">6</span> to <span class="tex-span">6 + 5 + 1 = 12</span>. </li></ul>
