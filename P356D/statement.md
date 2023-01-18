## Description

<div><p>When you were a child you must have been told a puzzle of bags and coins. Anyway, here's one of its versions: </p><p><span class="tex-font-style-it">A horse has three bags. The first bag has one coin, the second bag has one coin and the third bag has three coins. In total, the horse has three coins in the bags. How is that possible?</span> </p><p>The answer is quite simple. The third bag contains a coin and two other bags. </p><p>This problem is a generalization of the childhood puzzle. You have <span class="tex-span"><i>n</i></span> bags. You know that the first bag contains <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> coins, the second bag contains <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> coins, ..., the <span class="tex-span"><i>n</i></span>-th bag contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> coins. In total, there are <span class="tex-span"><i>s</i></span> coins. Find the way to arrange the bags and coins so that they match the described scenario or else state that it is impossible to do.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>s</i> ≤ 70000)</span> — the number of bags and the total number of coins. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 70000)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows the number of coins in the <span class="tex-span"><i>i</i></span>-th bag.</p></div><div class="output-specification"><p>If the answer doesn't exist, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print the contents of the <span class="tex-span"><i>i</i></span>-th bag. The first number in the line, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>, must represent the number of coins lying directly in the <span class="tex-span"><i>i</i></span>-th bag (the coins in the bags that are in the <span class="tex-span"><i>i</i></span>-th bag are not taken into consideration). The second number in the line, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i>)</span> must represent the number of bags that lie directly in the <span class="tex-span"><i>i</i></span>-th bag (the bags that are inside the bags lying in the <span class="tex-span"><i>i</i></span>-th bag are not taken into consideration). Next, the line must contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> integers — the numbers of the bags that are lying directly in the <span class="tex-span"><i>i</i></span>-th bag.</p><p>The total number of coins in the solution must equal <span class="tex-span"><i>s</i></span>. If we count the total number of coins the <span class="tex-span"><i>i</i></span>-th bag in the solution has, we should get <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>No bag can directly lie in more than one bag. The bags can be nested in more than one level (see the second test case). If there are multiple correct answers, you can print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>s</i> ≤ 70000)</span> — the number of bags and the total number of coins. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 70000)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows the number of coins in the <span class="tex-span"><i>i</i></span>-th bag.</p>

## Output

<p>If the answer doesn't exist, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print the contents of the <span class="tex-span"><i>i</i></span>-th bag. The first number in the line, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>, must represent the number of coins lying directly in the <span class="tex-span"><i>i</i></span>-th bag (the coins in the bags that are in the <span class="tex-span"><i>i</i></span>-th bag are not taken into consideration). The second number in the line, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i>)</span> must represent the number of bags that lie directly in the <span class="tex-span"><i>i</i></span>-th bag (the bags that are inside the bags lying in the <span class="tex-span"><i>i</i></span>-th bag are not taken into consideration). Next, the line must contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> integers — the numbers of the bags that are lying directly in the <span class="tex-span"><i>i</i></span>-th bag.</p><p>The total number of coins in the solution must equal <span class="tex-span"><i>s</i></span>. If we count the total number of coins the <span class="tex-span"><i>i</i></span>-th bag in the solution has, we should get <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>No bag can directly lie in more than one bag. The bags can be nested in more than one level (see the second test case). If there are multiple correct answers, you can print any of them.</p>





```input1
3 3
1 3 1

```




```input2
3 3
1 3 1

```




```input3
1 2
1

```




```input4
8 10
2 7 3 4 1 3 1 2

```




```output1
1 0
1 2 3 1
1 0

```




```output2
1 0
2 1 3
0 1 1

```




```output3
-1

```




```output4
2 0
1 2 1 4
0 2 7 8
0 2 5 6
1 0
3 0
1 0
2 0

```



## Note

<p>The pictures below show two possible ways to solve one test case from the statement. The left picture corresponds to the first test case, the right picture corresponds to the second one.</p><center> <img class="tex-graphics" src="file://PwtFT3UV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
