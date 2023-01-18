## Description

<div><p>While Patrick was gone shopping, Spongebob decided to play a little trick on his friend. The naughty Sponge browsed through Patrick's personal stuff and found a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> of length <span class="tex-span"><i>m</i></span>, consisting of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, not necessarily distinct. Then he picked some sequence <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span> and for each number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> got number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>f</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub></span>. To finish the prank he erased the initial sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It's hard to express how sad Patrick was when he returned home from shopping! We will just say that Spongebob immediately got really sorry about what he has done and he is now trying to restore the original sequence. Help him do this or determine that this is impossible.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the lengths of sequences <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, determining sequence <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>The last line contains <span class="tex-span"><i>m</i></span> integers, determining sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Possible</span>" if there is exactly one sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, such that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>f</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Then print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>If there are multiple suitable sequences <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, print "<span class="tex-font-style-tt">Ambiguity</span>".</p><p>If Spongebob has made a mistake in his calculations and no suitable sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> exists, print "<span class="tex-font-style-tt">Impossible</span>".</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the lengths of sequences <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, determining sequence <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>The last line contains <span class="tex-span"><i>m</i></span> integers, determining sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Possible</span>" if there is exactly one sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, such that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>f</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Then print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>If there are multiple suitable sequences <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, print "<span class="tex-font-style-tt">Ambiguity</span>".</p><p>If Spongebob has made a mistake in his calculations and no suitable sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> exists, print "<span class="tex-font-style-tt">Impossible</span>".</p>





```input1
3 3
3 2 1
1 2 3

```




```input2
3 3
1 1 1
1 1 1

```




```input3
3 3
1 2 1
3 3 3

```




```output1
Possible
3 2 1 

```




```output2
Ambiguity

```




```output3
Impossible

```



## Note

<p>In the first sample <span class="tex-span">3</span> is replaced by <span class="tex-span">1</span> and vice versa, while <span class="tex-span">2</span> never changes. The answer exists and is unique.</p><p>In the second sample all numbers are replaced by <span class="tex-span">1</span>, so it is impossible to unambiguously restore the original sequence.</p><p>In the third sample <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> ≠ 3</span> for all <span class="tex-span"><i>i</i></span>, so no sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> transforms into such <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and we can say for sure that Spongebob has made a mistake.</p>
