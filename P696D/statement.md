## Description

<div><p>Barney was hanging out with Nora for a while and now he thinks he may have feelings for her. Barney wants to send her a cheesy text message and wants to make her as happy as possible.</p><center> <img class="tex-graphics" src="file://MjbVELA4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially, happiness level of Nora is <span class="tex-span">0</span>. Nora loves some pickup lines like "I'm falling for you" and stuff. Totally, she knows <span class="tex-span"><i>n</i></span> pickup lines, each consisting only of lowercase English letters, also some of them may be equal (in writing, but different in pronouncing or meaning though). Every time Nora sees <span class="tex-span"><i>i</i></span>-th pickup line as a <span class="tex-font-style-bf">consecutive subsequence</span> of Barney's text message her happiness level increases by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. These substrings may overlap, for example, Nora will see the pickup line <span class="tex-font-style-tt">aa</span> twice and the pickup line <span class="tex-font-style-tt">ab</span> once in text message <span class="tex-font-style-tt">aaab</span>.</p><p>Due to texting app limits, Barney's text may have up to <span class="tex-span"><i>l</i></span> characters.</p><p>Barney asked you to help him make Nora as much happy as possible, it's gonna be legen...</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">14</sup></span>)&nbsp;— the number of pickup lines and the maximum length of Barney's text.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), meaning that Nora's happiness level increases by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> after every time seeing <span class="tex-span"><i>i</i></span>-th pickup line.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the pickup lines. <span class="tex-span"><i>i</i></span>-th of them contains a single string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of only English lowercase letter. Summary length of all pickup lines does not exceed <span class="tex-span">200</span>.</p><p><span class="tex-font-style-bf">All strings are not empty</span>.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the maximum possible value of Nora's happiness level after reading Barney's text.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">14</sup></span>)&nbsp;— the number of pickup lines and the maximum length of Barney's text.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), meaning that Nora's happiness level increases by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> after every time seeing <span class="tex-span"><i>i</i></span>-th pickup line.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the pickup lines. <span class="tex-span"><i>i</i></span>-th of them contains a single string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of only English lowercase letter. Summary length of all pickup lines does not exceed <span class="tex-span">200</span>.</p><p><span class="tex-font-style-bf">All strings are not empty</span>.</p>

## Output

<p>Print the only integer&nbsp;— the maximum possible value of Nora's happiness level after reading Barney's text.</p>





```input1
3 6
3 2 1
heart
earth
art

```




```input2
3 6
3 2 8
heart
earth
art

```




```output1
6

```




```output2
16

```



## Note

<p>An optimal answer for the first sample case is <span class="tex-font-style-tt">hearth</span> containing each pickup line exactly once.</p><p>An optimal answer for the second sample case is <span class="tex-font-style-tt">artart</span>.</p>
