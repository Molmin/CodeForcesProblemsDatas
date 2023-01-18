## Description

<div><p>Santa Claus has <span class="tex-span"><i>n</i></span> tangerines, and the <span class="tex-span"><i>i</i></span>-th of them consists of exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> slices. Santa Claus came to a school which has <span class="tex-span"><i>k</i></span> pupils. Santa decided to treat them with tangerines.</p><p>However, there can be too few tangerines to present at least one tangerine to each pupil. So Santa decided to divide tangerines into parts so that no one will be offended. In order to do this, he can divide a tangerine or any existing part into two smaller equal parts. If the number of slices in the part he wants to split is odd, then one of the resulting parts will have one slice more than the other. It's forbidden to divide a part consisting of only one slice.</p><p><span class="tex-font-style-bf">Santa Claus wants to present to everyone either a whole tangerine or exactly one part of it</span> (that also means that everyone must get a positive number of slices). One or several tangerines or their parts may stay with Santa.</p><p>Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> be the number of slices the <span class="tex-span"><i>i</i></span>-th pupil has in the end. Let Santa's <span class="tex-font-style-it">joy</span> be the minimum among all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>'s.</p><p>Your task is to find the maximum possible <span class="tex-font-style-it">joy</span> Santa can have after he treats everyone with tangerines (or their parts).</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>) denoting the number of tangerines and the number of pupils, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of slices the <span class="tex-span"><i>i</i></span>-th tangerine consists of.</p></div><div class="output-specification"><p>If there's no way to present a tangerine or a part of tangerine to everyone, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the maximum possible <span class="tex-font-style-it">joy</span> that Santa can have.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>) denoting the number of tangerines and the number of pupils, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of slices the <span class="tex-span"><i>i</i></span>-th tangerine consists of.</p>

## Output

<p>If there's no way to present a tangerine or a part of tangerine to everyone, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the maximum possible <span class="tex-font-style-it">joy</span> that Santa can have.</p>





```input1
3 2
5 9 3

```




```input2
2 4
12 14

```




```input3
2 3
1 1

```




```output1
5

```




```output2
6

```




```output3
-1

```



## Note

<p>In the first example Santa should divide the second tangerine into two parts with <span class="tex-span">5</span> and <span class="tex-span">4</span> slices. After that he can present the part with <span class="tex-span">5</span> slices to the first pupil and the whole first tangerine (with <span class="tex-span">5</span> slices, too) to the second pupil.</p><p>In the second example Santa should divide both tangerines, so that he'll be able to present two parts with <span class="tex-span">6</span> slices and two parts with <span class="tex-span">7</span> slices.</p><p>In the third example Santa Claus can't present <span class="tex-span">2</span> slices to <span class="tex-span">3</span> pupils in such a way that everyone will have anything.</p>
