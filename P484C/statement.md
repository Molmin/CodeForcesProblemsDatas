## Description

<div><p>How many specific orders do you know? Ascending order, descending order, order of ascending length, order of ascending polar angle... Let's have a look at another specific order: <span class="tex-font-style-underline"><span class="tex-span"><i>d</i></span>-sorting</span>. This sorting is applied to the strings of length at least <span class="tex-span"><i>d</i></span>, where <span class="tex-span"><i>d</i></span> is some positive integer. The characters of the string are sorted in following manner: first come all the 0-th characters of the initial string, then the 1-st ones, then the 2-nd ones and so on, in the end go all the <span class="tex-span">(<i>d</i> - 1)</span>-th characters of the initial string. By the <span class="tex-span"><i>i</i></span>-th characters we mean all the character whose positions are exactly <span class="tex-span"><i>i</i></span> modulo <span class="tex-span"><i>d</i></span>. If two characters stand on the positions with the same remainder of integer division by <span class="tex-span"><i>d</i></span>, their relative order after the sorting shouldn't be changed. The string is zero-indexed. For example, for string '<span class="tex-font-style-tt">qwerty</span>':</p><p>Its 1-sorting is the string '<span class="tex-font-style-tt">qwerty</span>' (all characters stand on 0 positions),</p><p>Its 2-sorting is the string '<span class="tex-font-style-tt">qetwry</span>' (characters '<span class="tex-font-style-tt">q</span>', '<span class="tex-font-style-tt">e</span>' and '<span class="tex-font-style-tt">t</span>' stand on 0 positions and characters '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">r</span>' and '<span class="tex-font-style-tt">y</span>' are on 1 positions),</p><p>Its 3-sorting is the string '<span class="tex-font-style-tt">qrwtey</span>' (characters '<span class="tex-font-style-tt">q</span>' and '<span class="tex-font-style-tt">r</span>' stand on 0 positions, characters '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">t</span>' stand on 1 positions and characters '<span class="tex-font-style-tt">e</span>' and '<span class="tex-font-style-tt">y</span>' stand on 2 positions),</p><p>Its 4-sorting is the string '<span class="tex-font-style-tt">qtwyer</span>',</p><p>Its 5-sorting is the string '<span class="tex-font-style-tt">qywert</span>'.</p><p>You are given string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-font-style-underline">shuffling</span> operations of this string. Each <span class="tex-font-style-underline">shuffling</span> operation accepts two integer arguments <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> and transforms string <span class="tex-span"><i>S</i></span> as follows. For each <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - <i>k</i></span> in the increasing order we apply the operation of <span class="tex-span"><i>d</i></span>-sorting to the substring <span class="tex-span"><i>S</i>[<i>i</i>..<i>i</i> + <i>k</i> - 1]</span>. Here <span class="tex-span"><i>S</i>[<i>a</i>..<i>b</i>]</span> represents a substring that consists of characters on positions from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> inclusive.</p><p>After each <span class="tex-font-style-underline">shuffling</span> operation you need to print string <span class="tex-span"><i>S</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains a non-empty string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase and uppercase English letters and digits from 0 to 9. </p><p>The second line of the input contains integer <span class="tex-span"><i>m</i></span>&nbsp;– the number of <span class="tex-font-style-underline">shuffling</span> operations (<span class="tex-span">1 ≤ <i>m</i>·<i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). </p><p>Following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the operations consisting of two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ <i>k</i> ≤ <i>n</i></span>). </p></div><div class="output-specification"><p>After each operation print the current state of string <span class="tex-span"><i>S</i></span>.</p></div>

## Input

<p>The first line of the input contains a non-empty string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase and uppercase English letters and digits from 0 to 9. </p><p>The second line of the input contains integer <span class="tex-span"><i>m</i></span>&nbsp;– the number of <span class="tex-font-style-underline">shuffling</span> operations (<span class="tex-span">1 ≤ <i>m</i>·<i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). </p><p>Following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the operations consisting of two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ <i>k</i> ≤ <i>n</i></span>). </p>

## Output

<p>After each operation print the current state of string <span class="tex-span"><i>S</i></span>.</p>





```input1
qwerty
3
4 2
6 3
5 2

```




```output1
qertwy
qtewry
qetyrw

```



## Note

<p>Here is detailed explanation of the sample. The first modification is executed with arguments <span class="tex-span"><i>k</i> = 4</span>, <span class="tex-span"><i>d</i> = 2</span>. That means that you need to apply 2-sorting for each substring of length 4 one by one moving from the left to the right. The string will transform in the following manner:</p><p><span class="tex-font-style-tt">qwerty</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt"><span class="tex-font-style-bf">qewr</span>ty</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">q<span class="tex-font-style-bf">erwt</span>y</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">qe<span class="tex-font-style-bf">rtwy</span></span></p><p>Thus, string <span class="tex-span"><i>S</i></span> equals '<span class="tex-font-style-tt">qertwy</span>' at the end of first query.</p><p>The second modification is executed with arguments <span class="tex-span"><i>k</i> = 6</span>, <span class="tex-span"><i>d</i> = 3</span>. As a result of this operation the whole string <span class="tex-span"><i>S</i></span> is replaced by its 3-sorting: </p><p><span class="tex-font-style-tt">qertwy</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt"><span class="tex-font-style-bf">qtewry</span></span></p><p>The third modification is executed with arguments <span class="tex-span"><i>k</i> = 5</span>, <span class="tex-span"><i>d</i> = 2</span>. </p><p><span class="tex-font-style-tt">qtewry</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt"><span class="tex-font-style-bf">qertw</span>y</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">q<span class="tex-font-style-bf">etyrw</span></span></p>
