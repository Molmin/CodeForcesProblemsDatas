## Description

<div><p>Berland scientists noticed long ago that the world around them depends on Berland population. Due to persistent research in this area the scientists managed to find out that the Berland chronology starts from the moment when the first two people came to that land (it is considered to have happened in the first year). After one Berland year after the start of the chronology the population had already equaled 13 people (the second year). However, tracing the population number during the following years was an ultimately difficult task, still it was found out that if <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of people in Berland in the year of <span class="tex-span"><i>i</i></span>, then either <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> = 12<i>d</i><sub class="lower-index"><i>i</i> - 2</sub></span>, or <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> = 13<i>d</i><sub class="lower-index"><i>i</i> - 1</sub> - 12<i>d</i><sub class="lower-index"><i>i</i> - 2</sub></span>. Of course no one knows how many people are living in Berland at the moment, but now we can tell if there could possibly be a year in which the country population equaled <span class="tex-span"><i>A</i></span>. That's what we ask you to determine. Also, if possible, you have to find out in which years it could be (from the beginning of Berland chronology). Let's suppose that it could be in the years of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. Then you have to define how many residents could be in the country during those years apart from the <span class="tex-span"><i>A</i></span> variant. Look at the examples for further explanation.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> &lt; 10<sup class="upper-index">300</sup></span>). It is guaranteed that the number doesn't contain leading zeros.</p></div><div class="output-specification"><p>On the first output line print <span class="tex-font-style-tt">YES</span>, if there could be a year in which the total population of the country equaled <span class="tex-span"><i>A</i></span>, otherwise print <span class="tex-font-style-tt">NO</span>. </p><p>If the answer is <span class="tex-font-style-tt">YES</span>, then you also have to print number <span class="tex-span"><i>k</i></span> — the number of years in which the population could equal <span class="tex-span"><i>A</i></span>. On the next line you have to output precisely <span class="tex-span"><i>k</i></span> space-separated numbers — <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. Those numbers have to be output in the increasing order.</p><p>On the next line you should output number <span class="tex-span"><i>p</i></span> — how many variants of the number of people could be in the years of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, apart from the <span class="tex-span"><i>A</i></span> variant. On each of the next <span class="tex-span"><i>p</i></span> lines you have to print one number — the sought number of residents. Those number also have to go in the increasing order. </p><p>If any number (or both of them) <span class="tex-span"><i>k</i></span> or <span class="tex-span"><i>p</i></span> exceeds <span class="tex-span">1000</span>, then you have to print <span class="tex-span">1000</span> instead of it and only the first <span class="tex-span">1000</span> possible answers in the increasing order.</p><p>The numbers should have no leading zeros.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> &lt; 10<sup class="upper-index">300</sup></span>). It is guaranteed that the number doesn't contain leading zeros.</p>

## Output

<p>On the first output line print <span class="tex-font-style-tt">YES</span>, if there could be a year in which the total population of the country equaled <span class="tex-span"><i>A</i></span>, otherwise print <span class="tex-font-style-tt">NO</span>. </p><p>If the answer is <span class="tex-font-style-tt">YES</span>, then you also have to print number <span class="tex-span"><i>k</i></span> — the number of years in which the population could equal <span class="tex-span"><i>A</i></span>. On the next line you have to output precisely <span class="tex-span"><i>k</i></span> space-separated numbers — <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. Those numbers have to be output in the increasing order.</p><p>On the next line you should output number <span class="tex-span"><i>p</i></span> — how many variants of the number of people could be in the years of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, apart from the <span class="tex-span"><i>A</i></span> variant. On each of the next <span class="tex-span"><i>p</i></span> lines you have to print one number — the sought number of residents. Those number also have to go in the increasing order. </p><p>If any number (or both of them) <span class="tex-span"><i>k</i></span> or <span class="tex-span"><i>p</i></span> exceeds <span class="tex-span">1000</span>, then you have to print <span class="tex-span">1000</span> instead of it and only the first <span class="tex-span">1000</span> possible answers in the increasing order.</p><p>The numbers should have no leading zeros.</p>





```input1
2

```




```input2
3

```




```input3
13

```




```input4
1729

```




```output1
YES
1
1
0

```




```output2
NO

```




```output3
YES
1
2
0

```




```output4
YES
1
4
1
156

```


