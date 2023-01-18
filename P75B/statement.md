## Description

<div><p>Facetook is a well known social network website, and it will launch a new feature called Facetook Priority Wall. This feature will sort all posts from your friends according to the priority factor (it will be described).</p><p>This priority factor will be affected by three types of actions: </p><ul> <li> 1. "<span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span> posted on <span class="tex-span"><i>Y</i></span>'s wall</span>" (15 points), </li><li> 2. "<span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span> commented on <span class="tex-span"><i>Y</i></span>'s post</span>" (10 points), </li><li> 3. "<span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span> likes <span class="tex-span"><i>Y</i></span>'s post</span>" (5 points). </li></ul><p><span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> will be two distinct names. And each action will increase the priority factor between <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> (and vice versa) by the above value of points (the priority factor between <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> is the same as the priority factor between <span class="tex-span"><i>Y</i></span> and <span class="tex-span"><i>X</i></span>).</p><p>You will be given <span class="tex-span"><i>n</i></span> actions with the above format (without the action number and the number of points), and you have to print all the distinct names in these actions sorted according to the priority factor with you.</p></div><div class="input-specification"><p>The first line contains your name. The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of actions (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then <span class="tex-span"><i>n</i></span> lines follow, it is guaranteed that each one contains exactly 1 action in the format given above. There is exactly one space between each two words in a line, and there are no extra spaces. All the letters are lowercase. All names in the input will consist of at least 1 letter and at most 10 small Latin letters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, where <span class="tex-span"><i>m</i></span> is the number of distinct names in the input (excluding yourself). Each line should contain just 1 name. The names should be sorted according to the priority factor with you in the descending order (the highest priority factor should come first). If two or more names have the same priority factor, print them in the alphabetical (lexicographical) order.</p><p>Note, that you should output all the names that are present in the input data (excluding yourself), even if that person has a zero priority factor.</p><p>The lexicographical comparison is performed by the standard "<span class="tex-font-style-tt">&lt;</span>" operator in modern programming languages. The line <span class="tex-span"><i>a</i></span> is lexicographically smaller than the line <span class="tex-span"><i>b</i></span>, if either <span class="tex-span"><i>a</i></span> is the prefix of <span class="tex-span"><i>b</i></span>, or if exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>min</i>(|<i>a</i>|, |<i>b</i>|)</span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span">|<i>a</i>|</span> and <span class="tex-span">|<i>b</i>|</span> stand for the lengths of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondently.</p></div>

## Input

<p>The first line contains your name. The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of actions (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then <span class="tex-span"><i>n</i></span> lines follow, it is guaranteed that each one contains exactly 1 action in the format given above. There is exactly one space between each two words in a line, and there are no extra spaces. All the letters are lowercase. All names in the input will consist of at least 1 letter and at most 10 small Latin letters.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, where <span class="tex-span"><i>m</i></span> is the number of distinct names in the input (excluding yourself). Each line should contain just 1 name. The names should be sorted according to the priority factor with you in the descending order (the highest priority factor should come first). If two or more names have the same priority factor, print them in the alphabetical (lexicographical) order.</p><p>Note, that you should output all the names that are present in the input data (excluding yourself), even if that person has a zero priority factor.</p><p>The lexicographical comparison is performed by the standard "<span class="tex-font-style-tt">&lt;</span>" operator in modern programming languages. The line <span class="tex-span"><i>a</i></span> is lexicographically smaller than the line <span class="tex-span"><i>b</i></span>, if either <span class="tex-span"><i>a</i></span> is the prefix of <span class="tex-span"><i>b</i></span>, or if exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>min</i>(|<i>a</i>|, |<i>b</i>|)</span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span">|<i>a</i>|</span> and <span class="tex-span">|<i>b</i>|</span> stand for the lengths of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondently.</p>





```input1
ahmed
3
ahmed posted on fatma's wall
fatma commented on ahmed's post
mona likes ahmed's post

```




```input2
aba
1
likes likes posted's post

```




```output1
fatma
mona

```




```output2
likes
posted

```


