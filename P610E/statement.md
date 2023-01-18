## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of first <span class="tex-span"><i>k</i></span> lowercase English letters.</p><p>We define a <span class="tex-font-style-it"><span class="tex-span"><i>c</i></span>-repeat</span> of some string <span class="tex-span"><i>q</i></span> as a string, consisting of <span class="tex-span"><i>c</i></span> copies of the string <span class="tex-span"><i>q</i></span>. For example, string "<span class="tex-font-style-tt">acbacbacbacb</span>" is a <span class="tex-span">4</span>-repeat of the string "<span class="tex-font-style-tt">acb</span>".</p><p>Let's say that string <span class="tex-span"><i>a</i></span> contains string <span class="tex-span"><i>b</i></span> as a subsequence, if string <span class="tex-span"><i>b</i></span> can be obtained from <span class="tex-span"><i>a</i></span> by erasing some symbols.</p><p>Let <span class="tex-span"><i>p</i></span> be a string that represents some permutation of the first <span class="tex-span"><i>k</i></span> lowercase English letters. We define function <span class="tex-span"><i>d</i>(<i>p</i>)</span> as the smallest integer such that a <span class="tex-span"><i>d</i>(<i>p</i>)</span>-repeat of the string <span class="tex-span"><i>p</i></span> contains string <span class="tex-span"><i>s</i></span> as a subsequence.</p><p>There are <span class="tex-span"><i>m</i></span> operations of one of two types that can be applied to string <span class="tex-span"><i>s</i></span>:</p><ol> <li> Replace all characters at positions from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> by a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> For the given <span class="tex-span"><i>p</i></span>, that is a permutation of first <span class="tex-span"><i>k</i></span> lowercase English letters, find the value of function <span class="tex-span"><i>d</i>(<i>p</i>)</span>. </li></ol><p>All operations are performed sequentially, in the order they appear in the input. Your task is to determine the values of function <span class="tex-span"><i>d</i>(<i>p</i>)</span> for all operations of the second type.</p></div><div class="input-specification"><p>The first line contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>m</i> ≤ 20000, 1 ≤ <i>k</i> ≤ 10</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>, the number of operations and the size of the alphabet respectively. The second line contains the string <span class="tex-span"><i>s</i></span> itself.</p><p>Each of the following lines <span class="tex-span"><i>m</i></span> contains a description of some operation: </p><ol> <li> Operation of the first type starts with <span class="tex-span">1</span> followed by a triple <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, that denotes replacement of all characters at positions from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> by character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is one of the first <span class="tex-span"><i>k</i></span> lowercase English letters). </li><li> Operation of the second type starts with <span class="tex-span">2</span> followed by a permutation of the first <span class="tex-span"><i>k</i></span> lowercase English letters.</li></ol></div><div class="output-specification"><p>For each query of the second type the value of function <span class="tex-span"><i>d</i>(<i>p</i>)</span>.</p></div>

## Input

<p>The first line contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>m</i> ≤ 20000, 1 ≤ <i>k</i> ≤ 10</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>, the number of operations and the size of the alphabet respectively. The second line contains the string <span class="tex-span"><i>s</i></span> itself.</p><p>Each of the following lines <span class="tex-span"><i>m</i></span> contains a description of some operation: </p><ol> <li> Operation of the first type starts with <span class="tex-span">1</span> followed by a triple <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, that denotes replacement of all characters at positions from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> by character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is one of the first <span class="tex-span"><i>k</i></span> lowercase English letters). </li><li> Operation of the second type starts with <span class="tex-span">2</span> followed by a permutation of the first <span class="tex-span"><i>k</i></span> lowercase English letters.</li></ol>

## Output

<p>For each query of the second type the value of function <span class="tex-span"><i>d</i>(<i>p</i>)</span>.</p>





```input1
7 4 3
abacaba
1 3 5 b
2 abc
1 4 4 c
2 cba

```




```output1
6
5

```



## Note

<p>After the first operation the string <span class="tex-span"><i>s</i></span> will be <span class="tex-font-style-tt">abbbbba</span>.</p><p>In the second operation the answer is <span class="tex-span">6</span>-repeat of <span class="tex-font-style-tt">abc</span>: <span class="tex-font-style-tt">ABcaBcaBcaBcaBcAbc</span>.</p><p>After the third operation the string <span class="tex-span"><i>s</i></span> will be <span class="tex-font-style-tt">abbcbba</span>.</p><p>In the fourth operation the answer is <span class="tex-span">5</span>-repeat of <span class="tex-font-style-tt">cba</span>: <span class="tex-font-style-tt">cbAcBacBaCBacBA</span>.</p><p>Uppercase letters means the occurrences of symbols from the string <span class="tex-span"><i>s</i></span>.</p>
