## Description

<div><p>Vitaly has an array of <span class="tex-span"><i>n</i></span> distinct integers. Vitaly wants to divide this array into three <span class="tex-font-style-bf">non-empty</span> sets so as the following conditions hold: </p><ol> <li> The product of all numbers in the first set is less than zero <span class="tex-span">( &lt; 0)</span>. </li><li> The product of all numbers in the second set is greater than zero <span class="tex-span">( &gt; 0)</span>. </li><li> The product of all numbers in the third set is equal to zero. </li><li> Each number from the initial array must occur in exactly one set. </li></ol><p>Help Vitaly. Divide the given array.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>)</span> — the array elements.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">1</sub> &gt; 0)</span> — the number of elements in the first set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> numbers — the elements that got to the first set.</p><p>In the next line print integer <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">2</sub> &gt; 0)</span> — the number of elements in the second set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> numbers — the elements that got to the second set.</p><p>In the next line print integer <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">3</sub> &gt; 0)</span> — the number of elements in the third set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> numbers — the elements that got to the third set.</p><p>The printed sets must meet the described conditions. It is guaranteed that the solution exists. If there are several solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>)</span> — the array elements.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">1</sub> &gt; 0)</span> — the number of elements in the first set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> numbers — the elements that got to the first set.</p><p>In the next line print integer <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">2</sub> &gt; 0)</span> — the number of elements in the second set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> numbers — the elements that got to the second set.</p><p>In the next line print integer <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> <span class="tex-span">(<i>n</i><sub class="lower-index">3</sub> &gt; 0)</span> — the number of elements in the third set. Then print <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> numbers — the elements that got to the third set.</p><p>The printed sets must meet the described conditions. It is guaranteed that the solution exists. If there are several solutions, you are allowed to print any of them.</p>





```input1
3
-1 2 0

```




```input2
4
-1 -2 -3 0

```




```output1
1 -1
1 2
1 0

```




```output2
1 -1
2 -3 -2
1 0

```


