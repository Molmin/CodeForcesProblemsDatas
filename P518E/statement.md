## Description

<div><p>After bracket sequences Arthur took up number theory. He has got a new favorite sequence of length <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>, consisting of integers and integer <span class="tex-span"><i>k</i></span>, not exceeding <span class="tex-span"><i>n</i></span>.</p><p>This sequence had the following property: if you write out the sums of all its segments consisting of <span class="tex-span"><i>k</i></span> consecutive elements <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>&nbsp; + &nbsp;<i>a</i><sub class="lower-index">2</sub>&nbsp;...&nbsp; + &nbsp;<i>a</i><sub class="lower-index"><i>k</i></sub>, &nbsp;<i>a</i><sub class="lower-index">2</sub>&nbsp; + &nbsp;<i>a</i><sub class="lower-index">3</sub>&nbsp; + &nbsp;...&nbsp; + &nbsp;<i>a</i><sub class="lower-index"><i>k</i> + 1</sub>, &nbsp;..., &nbsp;<i>a</i><sub class="lower-index"><i>n</i> - <i>k</i> + 1</sub>&nbsp; + &nbsp;<i>a</i><sub class="lower-index"><i>n</i> - <i>k</i> + 2</sub>&nbsp; + &nbsp;...&nbsp; + &nbsp;<i>a</i><sub class="lower-index"><i>n</i></sub>)</span>, then those numbers will form strictly increasing sequence.</p><p>For example, for the following sample: <span class="tex-span"><i>n</i> = 5, &nbsp;<i>k</i> = 3, &nbsp;<i>a</i> = (1, &nbsp;2, &nbsp;4, &nbsp;5, &nbsp;6)</span> the sequence of numbers will look as follows: (<span class="tex-span">1&nbsp; + &nbsp;2&nbsp; + &nbsp;4, &nbsp;2&nbsp; + &nbsp;4&nbsp; + &nbsp;5, &nbsp;4&nbsp; + &nbsp;5&nbsp; + &nbsp;6</span>)&nbsp;=&nbsp;(<span class="tex-span">7, &nbsp;11, &nbsp;15</span>), that means that sequence <span class="tex-span"><i>a</i></span> meets the described property. </p><p>Obviously the sequence of sums will have <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> elements.</p><p>Somebody (we won't say who) replaced some numbers in Arthur's sequence by question marks (if this number is replaced, it is replaced by exactly one question mark). We need to restore the sequence so that it meets the required property and also minimize the sum <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span>, where <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span> is the absolute value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers are in Arthur's sequence and the lengths of segments respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p><p>If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp; = &nbsp;?</span>, then the <span class="tex-span"><i>i</i></span>-th element of Arthur's sequence was replaced by a question mark. </p><p>Otherwise, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is the <span class="tex-span"><i>i</i></span>-th element of Arthur's sequence.</p></div><div class="output-specification"><p>If Arthur is wrong at some point and there is no sequence that could fit the given information, print a single string "<span class="tex-font-style-tt">Incorrect sequence</span>" (without the quotes).</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> integers — Arthur's favorite sequence. If there are multiple such sequences, print the sequence with the minimum sum <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span>, where <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span> is the absolute value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If there are still several such sequences, you are allowed to print any of them. Print the elements of the sequence without leading zeroes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers are in Arthur's sequence and the lengths of segments respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p><p>If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp; = &nbsp;?</span>, then the <span class="tex-span"><i>i</i></span>-th element of Arthur's sequence was replaced by a question mark. </p><p>Otherwise, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is the <span class="tex-span"><i>i</i></span>-th element of Arthur's sequence.</p>

## Output

<p>If Arthur is wrong at some point and there is no sequence that could fit the given information, print a single string "<span class="tex-font-style-tt">Incorrect sequence</span>" (without the quotes).</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> integers — Arthur's favorite sequence. If there are multiple such sequences, print the sequence with the minimum sum <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span>, where <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|</span> is the absolute value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If there are still several such sequences, you are allowed to print any of them. Print the elements of the sequence without leading zeroes.</p>





```input1
3 2
? 1 2

```




```input2
5 1
-10 -9 ? -7 -6

```




```input3
5 3
4 6 7 2 9

```




```output1
0 1 2 

```




```output2
-10 -9 -8 -7 -6 

```




```output3
Incorrect sequence

```


