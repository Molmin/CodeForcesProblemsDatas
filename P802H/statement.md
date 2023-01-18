## Description

<div><p>Thanks to your help, Heidi is confident that no one can fool her. She has now decided to post some fake news on the HC<span class="tex-span"><sup class="upper-index">2</sup></span> Facebook page. However, she wants to be able to communicate to the HC<span class="tex-span"><sup class="upper-index">2</sup></span> committee that the post is fake, using some secret phrase hidden in the post as a subsequence. To make this method foolproof, she wants the phrase to appear <span class="tex-span"><i>n</i></span> times in the post. She is asking you to design a post (string) <span class="tex-span"><i>s</i></span> and a hidden phrase <span class="tex-span"><i>p</i></span> such that <span class="tex-span"><i>p</i></span> appears in <span class="tex-span"><i>s</i></span> as a subsequence exactly <span class="tex-span"><i>n</i></span> times.</p></div><div class="input-specification"><p>The first and only line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>).</p></div><div class="output-specification"><p>The output should contain two nonempty strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>p</i></span> separated by a single space. Each string should be composed of letters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span> and <span class="tex-font-style-tt">A</span>-<span class="tex-font-style-tt">Z</span>: both lowercase and uppercase are allowed) and have length at most <span class="tex-span">200</span>. The number of occurrences of <span class="tex-span"><i>p</i></span> in <span class="tex-span"><i>s</i></span> as a subsequence should be exactly <span class="tex-span"><i>n</i></span>. If there are many possible solutions, output any of them. It is guaranteed that at least one solution exists.</p></div>

## Input

<p>The first and only line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>).</p>

## Output

<p>The output should contain two nonempty strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>p</i></span> separated by a single space. Each string should be composed of letters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span> and <span class="tex-font-style-tt">A</span>-<span class="tex-font-style-tt">Z</span>: both lowercase and uppercase are allowed) and have length at most <span class="tex-span">200</span>. The number of occurrences of <span class="tex-span"><i>p</i></span> in <span class="tex-span"><i>s</i></span> as a subsequence should be exactly <span class="tex-span"><i>n</i></span>. If there are many possible solutions, output any of them. It is guaranteed that at least one solution exists.</p>





```input1
2

```




```input2
4

```




```input3
6

```




```output1
hHheidi Hei
```




```output2
bbbba ba
```




```output3
aaabb ab
```



## Note

<p>An occurrence of <span class="tex-span"><i>p</i></span> as a subsequence in <span class="tex-span"><i>s</i></span> should be thought of as a set of positions in <span class="tex-span"><i>s</i></span> such that the letters at these positions, in order, form <span class="tex-span"><i>p</i></span>. The number of occurences is thus the number of such sets. For example, <span class="tex-font-style-tt">ab</span> appears 6 times as a subsequence in <span class="tex-font-style-tt">aaabb</span>, for the following sets of positions: <span class="tex-span">{1, 4}, {1, 5}, {2, 4}, {2, 5}, {3, 4}, {3, 5}</span> (that is, we should choose one of the <span class="tex-font-style-tt">a</span>'s and one of the <span class="tex-font-style-tt">b</span>'s).</p>
