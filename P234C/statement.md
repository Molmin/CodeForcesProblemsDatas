## Description

<div><p>Scientists say a lot about the problems of global warming and cooling of the Earth. Indeed, such natural phenomena strongly influence all life on our planet.</p><p>Our hero Vasya is quite concerned about the problems. He decided to try a little experiment and observe how outside daily temperature changes. He hung out a thermometer on the balcony every morning and recorded the temperature. He had been measuring the temperature for the last <span class="tex-span"><i>n</i></span> days. Thus, he got a sequence of numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where the <span class="tex-span"><i>i</i></span>-th number is the temperature on the <span class="tex-span"><i>i</i></span>-th day.</p><p>Vasya analyzed the temperature statistics in other cities, and came to the conclusion that the city has no environmental problems, if first the temperature outside is negative for some non-zero number of days, and then the temperature is positive for some non-zero number of days. More formally, there must be a positive integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) such that <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> &lt; 0, <i>t</i><sub class="lower-index">2</sub> &lt; 0, ..., <i>t</i><sub class="lower-index"><i>k</i></sub> &lt; 0</span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>k</i> + 1</sub> &gt; 0, <i>t</i><sub class="lower-index"><i>k</i> + 2</sub> &gt; 0, ..., <i>t</i><sub class="lower-index"><i>n</i></sub> &gt; 0</span>. In particular, the temperature should never be zero. If this condition is not met, Vasya decides that his city has environmental problems, and gets upset.</p><p>You do not want to upset Vasya. Therefore, you want to select multiple values of temperature and modify them to satisfy Vasya's condition. You need to know what the least number of temperature values needs to be changed for that.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of days for which Vasya has been measuring the temperature. </p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>t</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the sequence of temperature values. Numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are separated by single spaces.</p></div><div class="output-specification"><p>Print a single integer — the answer to the given task.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of days for which Vasya has been measuring the temperature. </p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>t</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the sequence of temperature values. Numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are separated by single spaces.</p>

## Output

<p>Print a single integer — the answer to the given task.</p>





```input1
4
-1 1 -2 1

```




```input2
5
0 -1 1 2 -5

```




```output1
1

```




```output2
2

```



## Note

<p>Note to the first sample: there are two ways to change exactly one number so that the sequence met Vasya's condition. You can either replace the first number <span class="tex-font-style-tt">1</span> by any negative number or replace the number <span class="tex-font-style-tt">-2</span> by any positive number.</p>
