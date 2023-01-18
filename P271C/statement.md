## Description

<div><p>The Greatest Secret Ever consists of <span class="tex-span"><i>n</i></span> words, indexed by positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The secret needs dividing between <span class="tex-span"><i>k</i></span> Keepers (let's index them by positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>), the <span class="tex-span"><i>i</i></span>-th Keeper gets a <span class="tex-font-style-bf">non-empty</span> set of words with numbers from the set <span class="tex-span"><i>U</i><sub class="lower-index"><i>i</i></sub> = (<i>u</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>u</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>u</i><sub class="lower-index"><i>i</i>, |<i>U</i><sub class="lower-index"><i>i</i></sub>|</sub>)</span>. Here and below we'll presuppose that the set elements are written in the increasing order.</p><p>We'll say that the <span class="tex-font-style-it">secret is safe</span> if the following conditions are hold:</p><ul> <li> for any two indexes <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>k</i></span>) the intersection of sets <span class="tex-span"><i>U</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>U</i><sub class="lower-index"><i>j</i></sub></span> is an empty set; </li><li> the union of sets <span class="tex-span"><i>U</i><sub class="lower-index">1</sub>, <i>U</i><sub class="lower-index">2</sub>, ..., <i>U</i><sub class="lower-index"><i>k</i></sub></span> is set <span class="tex-span">(1, 2, ..., <i>n</i>)</span>; </li><li> in each set <span class="tex-span"><i>U</i><sub class="lower-index"><i>i</i></sub></span>, its elements <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>u</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>u</i><sub class="lower-index"><i>i</i>, |<i>U</i><sub class="lower-index"><i>i</i></sub>|</sub></span> <span class="tex-font-style-bf">do not form</span> an arithmetic progression (in particular, <span class="tex-span">|<i>U</i><sub class="lower-index"><i>i</i></sub>| ≥ 3</span> should hold). </li></ul><p>Let us remind you that the elements of set <span class="tex-span">(<i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>s</i></sub>)</span> form an arithmetic progression if there is such number <span class="tex-span"><i>d</i></span>, that for all <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>s</i></span>) fulfills <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> + <i>d</i> = <i>u</i><sub class="lower-index"><i>i</i> + 1</sub></span>. For example, the elements of sets <span class="tex-span">(5)</span>, <span class="tex-span">(1, 10)</span> and <span class="tex-span">(1, 5, 9)</span> form arithmetic progressions and the elements of sets <span class="tex-span">(1, 2, 4)</span> and <span class="tex-span">(3, 6, 8)</span> don't.</p><p>Your task is to find any partition of the set of words into subsets <span class="tex-span"><i>U</i><sub class="lower-index">1</sub>, <i>U</i><sub class="lower-index">2</sub>, ..., <i>U</i><sub class="lower-index"><i>k</i></sub></span> so that the secret is safe. Otherwise indicate that there's no such partition.</p></div><div class="input-specification"><p>The input consists of a single line which contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of words in the secret and the number of the Keepers. The numbers are separated by a single space.</p></div><div class="output-specification"><p>If there is no way to keep the secret safe, print a single integer "-1" (without the quotes). Otherwise, print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them representing the number of the Keeper who's got the <span class="tex-span"><i>i</i></span>-th word of the secret.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The input consists of a single line which contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of words in the secret and the number of the Keepers. The numbers are separated by a single space.</p>

## Output

<p>If there is no way to keep the secret safe, print a single integer "-1" (without the quotes). Otherwise, print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them representing the number of the Keeper who's got the <span class="tex-span"><i>i</i></span>-th word of the secret.</p><p>If there are multiple solutions, print any of them.</p>





```input1
11 3

```




```input2
5 2

```




```output1
3 1 2 1 1 2 3 2 2 3 1

```




```output2
-1

```


