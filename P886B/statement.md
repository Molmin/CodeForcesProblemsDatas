## Description

<div><p>Vlad likes to eat in cafes very much. During his life, he has visited cafes <span class="tex-span"><i>n</i></span> times. Unfortunately, Vlad started to feel that his last visits are not any different from each other. To fix that Vlad had a small research.</p><p>First of all, Vlad assigned individual indices to all cafes. Then, he wrote down indices of cafes he visited in a row, in order of visiting them. Now, Vlad wants to find such a cafe that his last visit to that cafe was before his last visits to every other cafe. In other words, he wants to find such a cafe that he hasn't been there for as long as possible. Help Vlad to find that cafe.</p></div><div class="input-specification"><p>In first line there is one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— number of cafes indices written by Vlad.</p><p>In second line, <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>) are written&nbsp;— indices of cafes in order of being visited by Vlad. Vlad could visit some cafes more than once. Note that in numeration, some indices could be omitted.</p></div><div class="output-specification"><p>Print one integer&nbsp;— index of the cafe that Vlad hasn't visited for as long as possible.</p></div>

## Input

<p>In first line there is one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— number of cafes indices written by Vlad.</p><p>In second line, <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>) are written&nbsp;— indices of cafes in order of being visited by Vlad. Vlad could visit some cafes more than once. Note that in numeration, some indices could be omitted.</p>

## Output

<p>Print one integer&nbsp;— index of the cafe that Vlad hasn't visited for as long as possible.</p>





```input1
5
1 3 2 1 2

```




```input2
6
2 1 2 2 4 1

```




```output1
3

```




```output2
2

```



## Note

<p>In first test, there are three cafes, and the last visits to cafes with indices <span class="tex-span">1</span> and <span class="tex-span">2</span> were after the last visit to cafe with index <span class="tex-span">3</span>; so this cafe is the answer. </p><p>In second test case, there are also three cafes, but with indices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>. Cafes with indices <span class="tex-span">1</span> and <span class="tex-span">4</span> were visited after the last visit of cafe with index <span class="tex-span">2</span>, so the answer is <span class="tex-span">2</span>. Note that Vlad could omit some numbers while numerating the cafes.</p>
