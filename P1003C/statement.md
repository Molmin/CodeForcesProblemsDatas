## Description

<div><p>The heat during the last few days has been really intense. Scientists from all over the Berland study how the temperatures and weather change, and they claim that this summer is abnormally hot. But any scientific claim sounds a lot more reasonable if there are some numbers involved, so they have decided to actually calculate some value which would represent how high the temperatures are.</p><p>Mathematicians of Berland State University came up with a special <span class="tex-font-style-it">heat intensity value</span>. This value is calculated as follows:</p><p>Suppose we want to analyze the segment of $n$ consecutive days. We have measured the temperatures during these $n$ days; the temperature during $i$-th day equals $a_i$.</p><p>We denote the <span class="tex-font-style-it">average temperature</span> of a segment of some consecutive days as the arithmetic mean of the temperature measures during this segment of days. So, if we want to analyze the <span class="tex-font-style-it">average temperature</span> from day $x$ to day $y$, we calculate it as $\frac{\sum \limits_{i = x}^{y} a_i}{y - x + 1}$ (note that division is performed without any rounding). The <span class="tex-font-style-it">heat intensity value</span> is the maximum of <span class="tex-font-style-it">average temperatures</span> over all segments of not less than $k$ consecutive days. For example, if analyzing the measures $[3, 4, 1, 2]$ and $k = 3$, we are interested in segments $[3, 4, 1]$, $[4, 1, 2]$ and $[3, 4, 1, 2]$ (we want to find the maximum value of <span class="tex-font-style-it">average temperature</span> over these segments).</p><p>You have been hired by Berland State University to write a program that would compute the <span class="tex-font-style-it">heat intensity value</span> of a given period of days. Are you up to this task?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the number of days in the given period, and the minimum number of days in a segment we consider when calculating <span class="tex-font-style-it">heat intensity value</span>, respectively.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 5000$) — the temperature measures during given $n$ days.</p></div><div class="output-specification"><p>Print one real number — the <span class="tex-font-style-it">heat intensity value</span>, i. e., the maximum of <span class="tex-font-style-it">average temperatures</span> over all segments of not less than $k$ consecutive days.</p><p>Your answer will be considered correct if the following condition holds: $|res - res_0| &lt; 10^{-6}$, where $res$ is your answer, and $res_0$ is the answer given by the jury's solution.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the number of days in the given period, and the minimum number of days in a segment we consider when calculating <span class="tex-font-style-it">heat intensity value</span>, respectively.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 5000$) — the temperature measures during given $n$ days.</p>

## Output

<p>Print one real number — the <span class="tex-font-style-it">heat intensity value</span>, i. e., the maximum of <span class="tex-font-style-it">average temperatures</span> over all segments of not less than $k$ consecutive days.</p><p>Your answer will be considered correct if the following condition holds: $|res - res_0| &lt; 10^{-6}$, where $res$ is your answer, and $res_0$ is the answer given by the jury's solution.</p>





```input1
4 3
3 4 1 2

```




```output1
2.666666666666667

```


