## Description

<div><p>You already know that Valery's favorite sport is biathlon. Due to your help, he learned to shoot without missing, and his skills are unmatched at the shooting range. But now a smaller task is to be performed, he should learn to complete the path fastest.</p><p>The track's map is represented by a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> in size divided into squares. Each square is marked with a lowercase Latin letter (which means the type of the plot), with the exception of the starting square (it is marked with a capital Latin letters <span class="tex-span"><i>S</i></span>) and the terminating square (it is marked with a capital Latin letter <span class="tex-span"><i>T</i></span>). The time of movement from one square to another is equal to <span class="tex-span">1</span> minute. The time of movement within the cell can be neglected. We can move from the cell only to side-adjacent ones, but it is forbidden to go beyond the map edges. Also the following restriction is imposed on the path: it is not allowed to visit more than <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">different types</span> of squares (squares of one type can be visited an infinite number of times). Squares marked with <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> have no type, so they are not counted. But <span class="tex-span"><i>S</i></span> must be visited exactly once — at the very beginning, and <span class="tex-span"><i>T</i></span> must be visited exactly once — at the very end.</p><p>Your task is to find the path from the square <span class="tex-span"><i>S</i></span> to the square <span class="tex-span"><i>T</i></span> that takes minimum time. Among all shortest paths you should choose the <span class="tex-font-style-bf">lexicographically minimal</span> one. When comparing paths you should lexicographically represent them as a sequence of characters, that is, of plot types.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50, <i>n</i>·<i>m</i> ≥ 2, 1 ≤ <i>k</i> ≤ 4</span>). Then <span class="tex-span"><i>n</i></span> lines contain the map. Each line has the length of exactly <span class="tex-span"><i>m</i></span> characters and consists of lowercase Latin letters and characters <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>. It is guaranteed that the map contains exactly one character <span class="tex-span"><i>S</i></span> and exactly one character <span class="tex-span"><i>T</i></span>.</p><p>Pretest 12 is one of the maximal tests for this problem.</p></div><div class="output-specification"><p>If there is a path that satisfies the condition, print it as a sequence of letters — the plot types. Otherwise, print "-1" (without quotes). <span class="tex-font-style-bf">You shouldn't print the character <span class="tex-span"><i>S</i></span> in the beginning and <span class="tex-span"><i>T</i></span> in the end</span>.</p><p><span class="tex-font-style-bf">Note that this sequence may be empty.</span> This case is present in pretests. You can just print nothing or print one "End of line"-character. Both will be accepted.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50, <i>n</i>·<i>m</i> ≥ 2, 1 ≤ <i>k</i> ≤ 4</span>). Then <span class="tex-span"><i>n</i></span> lines contain the map. Each line has the length of exactly <span class="tex-span"><i>m</i></span> characters and consists of lowercase Latin letters and characters <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>. It is guaranteed that the map contains exactly one character <span class="tex-span"><i>S</i></span> and exactly one character <span class="tex-span"><i>T</i></span>.</p><p>Pretest 12 is one of the maximal tests for this problem.</p>

## Output

<p>If there is a path that satisfies the condition, print it as a sequence of letters — the plot types. Otherwise, print "-1" (without quotes). <span class="tex-font-style-bf">You shouldn't print the character <span class="tex-span"><i>S</i></span> in the beginning and <span class="tex-span"><i>T</i></span> in the end</span>.</p><p><span class="tex-font-style-bf">Note that this sequence may be empty.</span> This case is present in pretests. You can just print nothing or print one "End of line"-character. Both will be accepted.</p>





```input1
5 3 2
Sba
ccc
aac
ccc
abT

```




```input2
3 4 1
Sxyy
yxxx
yyyT

```




```input3
1 3 3
TyS

```




```input4
1 4 1
SxyT

```




```output1
bcccc

```




```output2
xxxx

```




```output3
y

```




```output4
-1

```


