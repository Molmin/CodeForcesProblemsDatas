## Description

<div><p>Misha has an array of <span class="tex-span"><i>n</i></span> integers indexed by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Let's define <span class="tex-font-style-it">palindrome degree</span> of array <span class="tex-span"><i>a</i></span> as the number of such index pairs <span class="tex-span">(<i>l</i>, <i>r</i>)(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, that the elements from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th one inclusive can be rearranged in such a way that the <span class="tex-font-style-bf">whole</span> array will be a palindrome. In other words, pair <span class="tex-span">(<i>l</i>, <i>r</i>)</span> should meet the condition that after some rearranging of numbers on positions from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive (it is allowed not to rearrange the numbers at all), for any <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span> following condition holds: <span class="tex-span"><i>a</i>[<i>i</i>] = <i>a</i>[<i>n</i> - <i>i</i> + 1]</span>. </p><p>Your task is to find the <span class="tex-font-style-it">palindrome degree</span> of Misha's array.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i></span>), separated by spaces — the elements of Misha's array.</p></div><div class="output-specification"><p>In a single line print the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i></span>), separated by spaces — the elements of Misha's array.</p>

## Output

<p>In a single line print the answer to the problem.</p>





```input1
3
2 2 2

```




```input2
6
3 6 5 3 3 5

```




```input3
5
5 5 2 5 2

```




```output1
6

```




```output2
0

```




```output3
4

```



## Note

<p>In the first sample test any possible pair <span class="tex-span">(<i>l</i>, <i>r</i>)</span> meets the condition.</p><p>In the third sample test following pairs <span class="tex-span">(1, 3), (1, 4), (1, 5), (2, 5)</span> meet the condition.</p>
