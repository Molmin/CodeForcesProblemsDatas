## Description

<div><p>During the "Russian Code Cup" programming competition, the testing system stores all sent solutions for each participant. We know that many participants use random numbers in their programs and are often sent several solutions with the same source code to check.</p><p>Each participant is identified by some unique positive integer <span class="tex-span"><i>k</i></span>, and each sent solution <span class="tex-span"><i>A</i></span> is characterized by two numbers: <span class="tex-span"><i>x</i></span>&nbsp;— the number of different solutions that are sent before the first solution identical to <span class="tex-span"><i>A</i></span>, and <span class="tex-span"><i>k</i></span> — the number of the participant, who is the author of the solution. Consequently, all identical solutions have the same <span class="tex-span"><i>x</i></span>.</p><p>It is known that the data in the testing system are stored in the chronological order, that is, if the testing system has a solution with number <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> &gt; 0)</span> of the participant with number <span class="tex-span"><i>k</i></span>, then the testing system has a solution with number <span class="tex-span"><i>x</i> - 1</span> of the same participant stored somewhere before.</p><p>During the competition the checking system crashed, but then the data of the submissions of all participants have been restored. Now the jury wants to verify that the recovered data is in chronological order. Help the jury to do so.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of solutions. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers separated by space <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of previous unique solutions and the identifier of the participant.</p></div><div class="output-specification"><p>A single line of the output should contain «<span class="tex-font-style-tt">YES</span>» if the data is in chronological order, and «<span class="tex-font-style-tt">NO</span>» otherwise.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of solutions. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers separated by space <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of previous unique solutions and the identifier of the participant.</p>

## Output

<p>A single line of the output should contain «<span class="tex-font-style-tt">YES</span>» if the data is in chronological order, and «<span class="tex-font-style-tt">NO</span>» otherwise.</p>





```input1
2
0 1
1 1

```




```input2
4
0 1
1 2
1 1
0 2

```




```input3
4
0 1
1 1
0 1
0 2

```




```output1
YES

```




```output2
NO

```




```output3
YES

```


