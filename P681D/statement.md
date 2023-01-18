## Description

<div><p>Sasha lives in a big happy family. At the Man's Day all the men of the family gather to celebrate it following their own traditions. There are <span class="tex-span"><i>n</i></span> men in Sasha's family, so let's number them with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Each man has at most one father but may have arbitrary number of sons.</p><p>Man number <span class="tex-span"><i>A</i></span> is considered to be the <span class="tex-font-style-it">ancestor</span> of the man number <span class="tex-span"><i>B</i></span> if at least one of the following conditions is satisfied: </p><ul> <li> <span class="tex-span"><i>A</i> = <i>B</i></span>; </li><li> the man number <span class="tex-span"><i>A</i></span> is the father of the man number <span class="tex-span"><i>B</i></span>; </li><li> there is a man number <span class="tex-span"><i>C</i></span>, such that the man number <span class="tex-span"><i>A</i></span> is his ancestor and the man number <span class="tex-span"><i>C</i></span> is the father of the man number <span class="tex-span"><i>B</i></span>. </li></ul><p>Of course, if the man number <span class="tex-span"><i>A</i></span> is an ancestor of the man number <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>A</i> ≠ <i>B</i></span>, then the man number <span class="tex-span"><i>B</i></span> is not an ancestor of the man number <span class="tex-span"><i>A</i></span>.</p><p>The tradition of the Sasha's family is to give gifts at the Man's Day. Because giving gifts in a normal way is boring, each year the following happens.</p><ol> <li> A list of candidates is prepared, containing some (possibly all) of the <span class="tex-span"><i>n</i></span> men in some order. </li><li> Each of the <span class="tex-span"><i>n</i></span> men decides to give a gift. </li><li> In order to choose a person to give a gift to, man <span class="tex-span"><i>A</i></span> looks through the list and picks the first man <span class="tex-span"><i>B</i></span> in the list, such that <span class="tex-span"><i>B</i></span> is an ancestor of <span class="tex-span"><i>A</i></span> and gives him a gift. Note that according to definition it may happen that a person gives a gift to himself. </li><li> If there is no ancestor of a person in the list, he becomes sad and leaves the celebration without giving a gift to anyone. </li></ol><p>This year you have decided to help in organizing celebration and asked each of the <span class="tex-span"><i>n</i></span> men, who do they want to give presents to (this person is chosen only among ancestors). Are you able to make a list of candidates, such that all the wishes will be satisfied if they give gifts according to the process described above?</p></div><div class="input-specification"><p>In the first line of the input two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i> ≤ 100 000</span>) are given&nbsp;— the number of the men in the Sasha's family and the number of family relations in it respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe family relations: the <span class="tex-span">(<i>i</i> + 1)<sup class="upper-index"><i>th</i></sup></span> line consists of pair of integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>q</i><sub class="lower-index"><i>i</i></sub></span>) meaning that the man numbered <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the father of the man numbered <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that every pair of numbers appears at most once, that among every pair of two different men at least one of them is not an ancestor of another and that every man has at most one father.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of which means that the man numbered <span class="tex-span"><i>i</i></span> wants to give a gift to the man numbered <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span> the man numbered <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an ancestor of the man numbered <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i>)</span>&nbsp;— the number of the men in the list of candidates, in the first line.</p><p>Print then <span class="tex-span"><i>k</i></span> pairwise different positive integers not exceeding <span class="tex-span"><i>n</i></span> — the numbers of the men in the list in an order satisfying every of the men's wishes, one per line.</p><p>If there are more than one appropriate lists, print any of them. If there is no appropriate list print <span class="tex-span"> - 1</span> in the only line.</p></div>

## Input

<p>In the first line of the input two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i> ≤ 100 000</span>) are given&nbsp;— the number of the men in the Sasha's family and the number of family relations in it respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe family relations: the <span class="tex-span">(<i>i</i> + 1)<sup class="upper-index"><i>th</i></sup></span> line consists of pair of integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>q</i><sub class="lower-index"><i>i</i></sub></span>) meaning that the man numbered <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the father of the man numbered <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that every pair of numbers appears at most once, that among every pair of two different men at least one of them is not an ancestor of another and that every man has at most one father.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of which means that the man numbered <span class="tex-span"><i>i</i></span> wants to give a gift to the man numbered <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span> the man numbered <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an ancestor of the man numbered <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i>)</span>&nbsp;— the number of the men in the list of candidates, in the first line.</p><p>Print then <span class="tex-span"><i>k</i></span> pairwise different positive integers not exceeding <span class="tex-span"><i>n</i></span> — the numbers of the men in the list in an order satisfying every of the men's wishes, one per line.</p><p>If there are more than one appropriate lists, print any of them. If there is no appropriate list print <span class="tex-span"> - 1</span> in the only line.</p>





```input1
3 2
1 2
2 3
1 2 1

```




```input2
4 2
1 2
3 4
1 2 3 3

```




```output1
-1
```




```output2
3
2
1
3

```



## Note

<p>The first sample explanation: </p><ul> <li> if there would be no <span class="tex-span">1</span> in the list then the first and the third man's wishes would not be satisfied <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub> = <i>a</i><sub class="lower-index">3</sub> = 1)</span>; </li><li> if there would be no <span class="tex-span">2</span> in the list then the second man wish would not be satisfied <span class="tex-span">(<i>a</i><sub class="lower-index">2</sub> = 2)</span>; </li><li> if <span class="tex-span">1</span> would stay before <span class="tex-span">2</span> in the answer then the second man would have to give his gift to the first man, but he wants to give it to himself <span class="tex-span">(<i>a</i><sub class="lower-index">2</sub> = 2)</span>. </li><li> if, at the other hand, the man numbered <span class="tex-span">2</span> would stay before the man numbered <span class="tex-span">1</span>, then the third man would have to give his gift to the second man, but not to the first <span class="tex-span">(<i>a</i><sub class="lower-index">3</sub> = 1)</span>. </li></ul>
