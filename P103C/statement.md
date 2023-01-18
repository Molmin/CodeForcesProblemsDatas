## Description

<div><p>After all the events in Orlando we all know, Sasha and Roma decided to find out who is still the team's biggest loser. Thankfully, Masha found somewhere a revolver with a rotating cylinder of <span class="tex-span"><i>n</i></span> bullet slots able to contain exactly <span class="tex-span"><i>k</i></span> bullets, now the boys have a chance to resolve the problem once and for all. </p><p>Sasha selects any <span class="tex-span"><i>k</i></span> out of <span class="tex-span"><i>n</i></span> slots he wishes and puts bullets there. Roma spins the cylinder so that every of <span class="tex-span"><i>n</i></span> possible cylinder's shifts is equiprobable. Then the game starts, the players take turns, Sasha starts: he puts the gun to his head and shoots. If there was no bullet in front of the trigger, the cylinder shifts by one position and the weapon is given to Roma for make the same move. The game continues until someone is shot, the survivor is the winner. </p><p>Sasha does not want to lose, so he must choose slots for bullets in such a way as to minimize the probability of its own loss. Of all the possible variant he wants to select the lexicographically minimal one, where an empty slot is lexicographically less than a charged one. </p><p>More formally, the cylinder of <span class="tex-span"><i>n</i></span> bullet slots able to contain <span class="tex-span"><i>k</i></span> bullets can be represented as a string of <span class="tex-span"><i>n</i></span> characters. Exactly <span class="tex-span"><i>k</i></span> of them are "<span class="tex-font-style-tt">X</span>" (charged slots) and the others are "<span class="tex-font-style-tt">.</span>" (uncharged slots). </p><p>Let us describe the process of a shot. Suppose that the trigger is in front of the first character of the string (the first slot). If a shot doesn't kill anyone and the cylinder shifts, then the string shifts left. So the first character becomes the last one, the second character becomes the first one, and so on. But the trigger doesn't move. It will be in front of the first character of the resulting string.</p><p>Among all the strings that give the minimal probability of loss, Sasha choose the lexicographically minimal one. According to this very string, he charges the gun. You have to help Sasha to charge the gun. For that, each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> query must be answered: is there a bullet in the positions <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>k</i> ≤ <i>n</i>, 1 ≤ <i>p</i> ≤ 1000</span>) — the number of slots in the cylinder, the number of bullets and the number of queries. Then follow <span class="tex-span"><i>p</i></span> lines; they are the queries. Each line contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) the number of slot to describe.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p></div><div class="output-specification"><p>For each query print "<span class="tex-font-style-tt">.</span>" if the slot should be empty and "<span class="tex-font-style-tt">X</span>" if the slot should be charged.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>k</i> ≤ <i>n</i>, 1 ≤ <i>p</i> ≤ 1000</span>) — the number of slots in the cylinder, the number of bullets and the number of queries. Then follow <span class="tex-span"><i>p</i></span> lines; they are the queries. Each line contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) the number of slot to describe.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p>

## Output

<p>For each query print "<span class="tex-font-style-tt">.</span>" if the slot should be empty and "<span class="tex-font-style-tt">X</span>" if the slot should be charged.</p>





```input1
3 1 3
1
2
3

```




```input2
6 3 6
1
2
3
4
5
6

```




```input3
5 2 5
1
2
3
4
5

```




```output1
..X
```




```output2
.X.X.X
```




```output3
...XX
```



## Note

<p>The lexicographical comparison of is performed by the &lt; operator in modern programming languages. The <span class="tex-span"><i>a</i></span> string is lexicographically less that the <span class="tex-span"><i>b</i></span> string, if there exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p>
