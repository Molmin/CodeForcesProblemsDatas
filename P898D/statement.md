## Description

<div><p>Every evening Vitalya sets <span class="tex-span"><i>n</i></span> alarm clocks to wake up tomorrow. Every alarm clock rings during exactly one minute and is characterized by one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— number of minute after midnight in which it rings. Every alarm clock begins ringing at the beginning of the minute and rings during whole minute. </p><p>Vitalya will definitely wake up if during some <span class="tex-span"><i>m</i></span> consecutive minutes at least <span class="tex-span"><i>k</i></span> alarm clocks will begin ringing. Pay attention that Vitalya considers only alarm clocks which begin ringing during given period of time. He doesn't consider alarm clocks which started ringing before given period of time and continues ringing during given period of time.</p><p>Vitalya is so tired that he wants to sleep all day long and not to wake up. Find out minimal number of alarm clocks Vitalya should turn off to sleep all next day. Now all alarm clocks are turned on. </p></div><div class="input-specification"><p>First line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— number of alarm clocks, and conditions of Vitalya's waking up. </p><p>Second line contains sequence of <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) in which <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals minute on which <span class="tex-span"><i>i</i></span>-th alarm clock will ring. Numbers are given in arbitrary order. Vitalya lives in a Berland in which day lasts for <span class="tex-span">10<sup class="upper-index">6</sup></span> minutes. </p></div><div class="output-specification"><p>Output minimal number of alarm clocks that Vitalya should turn off to sleep all next day long.</p></div>

## Input

<p>First line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— number of alarm clocks, and conditions of Vitalya's waking up. </p><p>Second line contains sequence of <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) in which <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals minute on which <span class="tex-span"><i>i</i></span>-th alarm clock will ring. Numbers are given in arbitrary order. Vitalya lives in a Berland in which day lasts for <span class="tex-span">10<sup class="upper-index">6</sup></span> minutes. </p>

## Output

<p>Output minimal number of alarm clocks that Vitalya should turn off to sleep all next day long.</p>





```input1
3 3 2
3 5 1

```




```input2
5 10 3
12 8 18 25 1

```




```input3
7 7 2
7 3 4 1 6 5 2

```




```input4
2 2 2
1 3

```




```output1
1

```




```output2
0

```




```output3
6

```




```output4
0

```



## Note

<p>In first example Vitalya should turn off first alarm clock which rings at minute <span class="tex-span">3</span>.</p><p>In second example Vitalya shouldn't turn off any alarm clock because there are no interval of <span class="tex-span">10</span> consequence minutes in which <span class="tex-span">3</span> alarm clocks will ring.</p><p>In third example Vitalya should turn off any <span class="tex-span">6</span> alarm clocks.</p>
