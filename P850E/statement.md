## Description

<div><p>The presidential election is coming in Bearland next year! Everybody is so excited about this!</p><p>So far, there are three candidates, Alice, Bob, and Charlie. </p><p>There are <span class="tex-span"><i>n</i></span> citizens in Bearland. The election result will determine the life of all citizens of Bearland for many years. Because of this great responsibility, each of <span class="tex-span"><i>n</i></span> citizens will choose one of six orders of preference between Alice, Bob and Charlie uniformly at random, independently from other voters.</p><p>The government of Bearland has devised a function to help determine the outcome of the election given the voters preferences. More specifically, the function is <img align="middle" class="tex-formula" src="file://QYNvpJpN.png" style="max-width: 100.0%;max-height: 100.0%;"> (takes <span class="tex-span"><i>n</i></span> boolean numbers and returns a boolean number). The function also obeys the following property: <span class="tex-span"><i>f</i>(1 - <i>x</i><sub class="lower-index">1</sub>, 1 - <i>x</i><sub class="lower-index">2</sub>, ..., 1 - <i>x</i><sub class="lower-index"><i>n</i></sub>) = 1 - <i>f</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>)</span>.</p><p>Three rounds will be run between each pair of candidates: Alice and Bob, Bob and Charlie, Charlie and Alice. In each round, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will be equal to <span class="tex-span">1</span>, if <span class="tex-span"><i>i</i></span>-th citizen prefers the first candidate to second in this round, and <span class="tex-span">0</span> otherwise. After this, <span class="tex-span"><i>y</i> = <i>f</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>)</span> will be calculated. If <span class="tex-span"><i>y</i> = 1</span>, the first candidate will be declared as winner in this round. If <span class="tex-span"><i>y</i> = 0</span>, the second will be the winner, respectively.</p><p>Define the probability that there is a candidate who won two rounds as <span class="tex-span"><i>p</i></span>. <span class="tex-span"><i>p</i>·6<sup class="upper-index"><i>n</i></sup></span> is always an integer. Print the value of this integer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7 = 1 000 000 007</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>).</p><p>The next line contains a string of length <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> of zeros and ones, representing function <span class="tex-span"><i>f</i></span>. Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub>(<i>x</i>)</span> the <span class="tex-span"><i>k</i></span>-th bit in binary representation of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>i</i></span>-th (0-based) digit of this string shows the return value of <span class="tex-span"><i>f</i>(<i>b</i><sub class="lower-index">1</sub>(<i>i</i>), <i>b</i><sub class="lower-index">2</sub>(<i>i</i>), ..., <i>b</i><sub class="lower-index"><i>n</i></sub>(<i>i</i>))</span>.</p><p>It is guaranteed that <span class="tex-span"><i>f</i>(1 - <i>x</i><sub class="lower-index">1</sub>, 1 - <i>x</i><sub class="lower-index">2</sub>, ..., 1 - <i>x</i><sub class="lower-index"><i>n</i></sub>) = 1 - <i>f</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>)</span> for any values of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>ldots</i>, <i>x</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="output-specification"><p>Output one integer — answer to the problem.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>).</p><p>The next line contains a string of length <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> of zeros and ones, representing function <span class="tex-span"><i>f</i></span>. Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub>(<i>x</i>)</span> the <span class="tex-span"><i>k</i></span>-th bit in binary representation of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>i</i></span>-th (0-based) digit of this string shows the return value of <span class="tex-span"><i>f</i>(<i>b</i><sub class="lower-index">1</sub>(<i>i</i>), <i>b</i><sub class="lower-index">2</sub>(<i>i</i>), ..., <i>b</i><sub class="lower-index"><i>n</i></sub>(<i>i</i>))</span>.</p><p>It is guaranteed that <span class="tex-span"><i>f</i>(1 - <i>x</i><sub class="lower-index">1</sub>, 1 - <i>x</i><sub class="lower-index">2</sub>, ..., 1 - <i>x</i><sub class="lower-index"><i>n</i></sub>) = 1 - <i>f</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>)</span> for any values of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>ldots</i>, <i>x</i><sub class="lower-index"><i>n</i></sub></span>.</p>

## Output

<p>Output one integer — answer to the problem.</p>





```input1
3
01010101

```




```input2
3
01101001

```




```output1
216

```




```output2
168

```



## Note

<p>In first sample, result is always fully determined by the first voter. In other words, <span class="tex-span"><i>f</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>) = <i>x</i><sub class="lower-index">1</sub></span>. Thus, any no matter what happens, there will be a candidate who won two rounds (more specifically, the candidate who is at the top of voter 1's preference list), so <span class="tex-span"><i>p</i> = 1</span>, and we print <span class="tex-span">1·6<sup class="upper-index">3</sup> = 216</span>.</p>
