## Description

<div><p>There is an old tradition of keeping <span class="tex-span">4</span> boxes of candies in the house in Cyberland. The numbers of candies are <span class="tex-font-style-underline">special</span> if their <span class="tex-font-style-underline">arithmetic mean</span>, their <span class="tex-font-style-underline">median</span> and their <span class="tex-font-style-underline">range</span> are all equal. By definition, for a set <span class="tex-span">{<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>}</span> (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>x</i><sub class="lower-index">3</sub> ≤ <i>x</i><sub class="lower-index">4</sub></span>) <span class="tex-font-style-underline">arithmetic mean</span> is <img align="middle" class="tex-formula" src="file://4n0kYpTC.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-font-style-underline">median</span> is <img align="middle" class="tex-formula" src="file://jZLHoZ4U.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-font-style-underline">range</span> is <span class="tex-span"><i>x</i><sub class="lower-index">4</sub> - <i>x</i><sub class="lower-index">1</sub></span>. <span class="tex-font-style-bf">The arithmetic mean and median are not necessary integer.</span> It is well-known that if those three numbers are same, boxes will create a "debugging field" and codes in the field will have no bugs.</p><p>For example, <span class="tex-span">1, 1, 3, 3</span> is the example of <span class="tex-span">4</span> numbers meeting the condition because their mean, median and range are all equal to <span class="tex-span">2</span>.</p><p>Jeff has <span class="tex-span">4</span> special boxes of candies. However, something bad has happened! Some of the boxes could have been lost and now there are only <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 4</span>) boxes remaining. The <span class="tex-span"><i>i</i></span>-th remaining box contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> candies.</p><p>Now Jeff wants to know: is there a possible way to find the number of candies of the <span class="tex-span">4 - <i>n</i></span> missing boxes, meeting the condition above (the mean, median and range are equal)?</p></div><div class="input-specification"><p>The first line of input contains an only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 4</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, denoting the number of candies in the <span class="tex-span"><i>i</i></span>-th box (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>).</p></div><div class="output-specification"><p>In the first output line, print "<span class="tex-font-style-tt">YES</span>" if a solution exists, or print "<span class="tex-font-style-tt">NO</span>" if there is no solution.</p><p>If a solution exists, you should output <span class="tex-span">4 - <i>n</i></span> more lines, each line containing an integer <span class="tex-span"><i>b</i></span>, denoting the number of candies in a missing box.</p><p>All your numbers <span class="tex-span"><i>b</i></span> must satisfy inequality <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>. It is guaranteed that if there exists a positive integer solution, you can always find such <span class="tex-span"><i>b</i></span>'s meeting the condition. If there are multiple answers, you are allowed to print any of them.</p><p><span class="tex-font-style-bf">Given numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may follow in any order in the input, not necessary in non-decreasing.</span></p><p><span class="tex-font-style-bf"><span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may have stood at any positions in the original set, not necessary on lowest <span class="tex-span"><i>n</i></span> first positions</span>.</p></div>

## Input

<p>The first line of input contains an only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 4</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, denoting the number of candies in the <span class="tex-span"><i>i</i></span>-th box (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>).</p>

## Output

<p>In the first output line, print "<span class="tex-font-style-tt">YES</span>" if a solution exists, or print "<span class="tex-font-style-tt">NO</span>" if there is no solution.</p><p>If a solution exists, you should output <span class="tex-span">4 - <i>n</i></span> more lines, each line containing an integer <span class="tex-span"><i>b</i></span>, denoting the number of candies in a missing box.</p><p>All your numbers <span class="tex-span"><i>b</i></span> must satisfy inequality <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>. It is guaranteed that if there exists a positive integer solution, you can always find such <span class="tex-span"><i>b</i></span>'s meeting the condition. If there are multiple answers, you are allowed to print any of them.</p><p><span class="tex-font-style-bf">Given numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may follow in any order in the input, not necessary in non-decreasing.</span></p><p><span class="tex-font-style-bf"><span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may have stood at any positions in the original set, not necessary on lowest <span class="tex-span"><i>n</i></span> first positions</span>.</p>





```input1
2
1
1

```




```input2
3
1
1
1

```




```input3
4
1
2
2
3

```




```output1
YES
3
3

```




```output2
NO

```




```output3
YES

```



## Note

<p>For the first sample, the numbers of candies in <span class="tex-span">4</span> boxes can be <span class="tex-span">1, 1, 3, 3</span>. The arithmetic mean, the median and the range of them are all <span class="tex-span">2</span>.</p><p>For the second sample, it's impossible to find the missing number of candies.</p><p>In the third example no box has been lost and numbers satisfy the condition.</p><p><span class="tex-font-style-bf">You may output <span class="tex-span"><i>b</i></span> in any order.</span></p>
