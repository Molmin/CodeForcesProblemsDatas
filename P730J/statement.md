## Description

<div><p>Nick has <span class="tex-span"><i>n</i></span> bottles of soda left after his birthday. Each bottle is described by two values: remaining amount of soda <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and bottle volume <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Nick has decided to pour all remaining soda into minimal number of bottles, moreover he has to do it as soon as possible. Nick spends <span class="tex-span"><i>x</i></span> seconds to pour <span class="tex-span"><i>x</i></span> units of soda from one bottle to another.</p><p>Nick asks you to help him to determine <span class="tex-span"><i>k</i></span> — the minimal number of bottles to store all remaining soda and <span class="tex-span"><i>t</i></span> — the minimal time to pour soda into <span class="tex-span"><i>k</i></span> bottles. A bottle can't store more soda than its volume. All remaining soda should be saved.</p></div><div class="input-specification"><p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of bottles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the amount of soda remaining in the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the volume of the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span> for any <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>The only line should contain two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span>, where <span class="tex-span"><i>k</i></span> is the minimal number of bottles that can store all the soda and <span class="tex-span"><i>t</i></span> is the minimal time to pour the soda into <span class="tex-span"><i>k</i></span> bottles.</p></div>

## Input

<p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of bottles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the amount of soda remaining in the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the volume of the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span> for any <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>The only line should contain two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span>, where <span class="tex-span"><i>k</i></span> is the minimal number of bottles that can store all the soda and <span class="tex-span"><i>t</i></span> is the minimal time to pour the soda into <span class="tex-span"><i>k</i></span> bottles.</p>





```input1
4
3 3 4 3
4 7 6 5

```




```input2
2
1 1
100 100

```




```input3
5
10 30 5 6 24
10 41 7 8 24

```




```output1
2 6

```




```output2
1 1

```




```output3
3 11

```



## Note

<p>In the first example Nick can pour soda from the first bottle to the second bottle. It will take 3 seconds. After it the second bottle will contain <span class="tex-span">3 + 3 = 6</span> units of soda. Then he can pour soda from the fourth bottle to the second bottle and to the third bottle: one unit to the second and two units to the third. It will take <span class="tex-span">1 + 2 = 3</span> seconds. So, all the soda will be in two bottles and he will spend <span class="tex-span">3 + 3 = 6</span> seconds to do it.</p>
