## Description

<div><p>The marmots need to prepare <span class="tex-span"><i>k</i></span> problems for HC<span class="tex-span"><sup class="upper-index">2</sup></span> over <span class="tex-span"><i>n</i></span> days. Each problem, once prepared, also has to be printed.</p><p>The preparation of a problem on day <span class="tex-span"><i>i</i></span> (at most one per day) costs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> CHF, and the printing of a problem on day <span class="tex-span"><i>i</i></span> (also at most one per day) costs <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> CHF. Of course, a problem cannot be printed before it has been prepared (but doing both on the same day is fine).</p><p>What is the minimum cost of preparation and printing?</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2200</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://AZI5gEtC.png" style="max-width: 100.0%;max-height: 100.0%;">) — the preparation costs. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://sGxofX5B.png" style="max-width: 100.0%;max-height: 100.0%;">) — the printing costs.</p></div><div class="output-specification"><p>Output the minimum cost of preparation and printing <span class="tex-span"><i>k</i></span> problems — that is, the minimum possible sum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub> + <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub> + ... + <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub> + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index">1</sub></sub> + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index">2</sub></sub> + ... + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index"><i>k</i></sub></sub></span>, where <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i><sub class="lower-index">1</sub> &lt; <i>j</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>j</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span> and <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> ≤ <i>j</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>i</i><sub class="lower-index">2</sub> ≤ <i>j</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i><sub class="lower-index"><i>k</i></sub></span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2200</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://AZI5gEtC.png" style="max-width: 100.0%;max-height: 100.0%;">) — the preparation costs. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://sGxofX5B.png" style="max-width: 100.0%;max-height: 100.0%;">) — the printing costs.</p>

## Output

<p>Output the minimum cost of preparation and printing <span class="tex-span"><i>k</i></span> problems — that is, the minimum possible sum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub> + <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub> + ... + <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub> + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index">1</sub></sub> + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index">2</sub></sub> + ... + <i>b</i><sub class="lower-index"><i>j</i><sub class="lower-index"><i>k</i></sub></sub></span>, where <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i><sub class="lower-index">1</sub> &lt; <i>j</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>j</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span> and <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> ≤ <i>j</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>i</i><sub class="lower-index">2</sub> ≤ <i>j</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i><sub class="lower-index"><i>k</i></sub></span>.</p>





```input1
8 4
3 8 7 9 9 4 6 8
2 5 9 4 3 8 9 1

```




```output1
32
```



## Note

<p>In the sample testcase, one optimum solution is to prepare the first problem on day <span class="tex-span">1</span> and print it on day <span class="tex-span">1</span>, prepare the second problem on day <span class="tex-span">2</span> and print it on day <span class="tex-span">4</span>, prepare the third problem on day <span class="tex-span">3</span> and print it on day <span class="tex-span">5</span>, and prepare the fourth problem on day <span class="tex-span">6</span> and print it on day <span class="tex-span">8</span>.</p>
