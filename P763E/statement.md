## Description

<div><p>After his birthday party, Timofey went to his favorite tree alley in a park. He wants to feed there his favorite birds&nbsp;— crows.</p><p>It's widely known that each tree is occupied by a single crow family. The trees in the alley form a row and are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some families are friends to each other. For some reasons, two families can be friends only if they live not too far from each other, more precisely, there is no more than <span class="tex-span"><i>k</i> - 1</span> trees between any pair of friend families. Formally, the family on the <span class="tex-span"><i>u</i></span>-th tree and the family on the <span class="tex-span"><i>v</i></span>-th tree can be friends only if <span class="tex-span">|<i>u</i> - <i>v</i>| ≤ <i>k</i></span> holds.</p><p>One of the friendship features is that if some family learns that Timofey is feeding crows somewhere, it notifies about this all friend families. Thus, after Timofey starts to feed crows under some tree, all the families that are friends to the family living on this tree, as well as their friends and so on, fly to the feeding place. Of course, the family living on the tree also comes to the feeding place.</p><p>Today Timofey came to the alley and noticed that all the families that live on trees with numbers strictly less than <span class="tex-span"><i>l</i></span> or strictly greater than <span class="tex-span"><i>r</i></span> have flown away. Thus, it is not possible to pass the information about feeding through them. Moreover, there is no need to feed them. Help Timofey to learn what is the minimum number of trees under which he has to feed crows so that all the families that have remained will get the information about feeding. You are given several situations, described by integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, you need to calculate the answer for all of them.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>), where <span class="tex-span"><i>n</i></span> is the number of trees, and <span class="tex-span"><i>k</i></span> is the maximum possible distance between friend families.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>·<i>k</i></span>)&nbsp;— the number of pair of friend families. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ 10<sup class="upper-index">5</sup></span>), that means that the families on trees <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends. It is guaranteed that <span class="tex-span"><i>u</i> ≠ <i>v</i></span> and <span class="tex-span">|<i>u</i> - <i>v</i>| ≤ <i>k</i></span>. All the given pairs are distinct.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of situations you need to calculate the answer in.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>), that means that in this situation families that have flown away lived on such trees <span class="tex-span"><i>x</i></span>, so that either <span class="tex-span"><i>x</i> &lt; <i>l</i></span> or <span class="tex-span"><i>x</i> &gt; <i>r</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. Line <span class="tex-span"><i>i</i></span> should contain single integer&nbsp;— the answer in the <span class="tex-span"><i>i</i></span>-th situation.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>), where <span class="tex-span"><i>n</i></span> is the number of trees, and <span class="tex-span"><i>k</i></span> is the maximum possible distance between friend families.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>·<i>k</i></span>)&nbsp;— the number of pair of friend families. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ 10<sup class="upper-index">5</sup></span>), that means that the families on trees <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends. It is guaranteed that <span class="tex-span"><i>u</i> ≠ <i>v</i></span> and <span class="tex-span">|<i>u</i> - <i>v</i>| ≤ <i>k</i></span>. All the given pairs are distinct.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of situations you need to calculate the answer in.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>), that means that in this situation families that have flown away lived on such trees <span class="tex-span"><i>x</i></span>, so that either <span class="tex-span"><i>x</i> &lt; <i>l</i></span> or <span class="tex-span"><i>x</i> &gt; <i>r</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. Line <span class="tex-span"><i>i</i></span> should contain single integer&nbsp;— the answer in the <span class="tex-span"><i>i</i></span>-th situation.</p>





```input1
5 3
3
1 3
2 3
4 5
5
1 1
1 2
2 3
1 3
1 5

```




```output1
1
2
1
1
2

```



## Note

<p>In the first example the following family pairs are friends: <span class="tex-span">(1, 3)</span>, <span class="tex-span">(2, 3)</span> and <span class="tex-span">(4, 5)</span>.</p><ul> <li> In the first situation only the first family has remained, so the answer is <span class="tex-span">1</span>. </li><li> In the second situation the first two families have remained, and they aren't friends, so the answer is <span class="tex-span">2</span>. </li><li> In the third situation the families <span class="tex-span">2</span> and <span class="tex-span">3</span> are friends, so it is enough to feed any of them, the answer is <span class="tex-span">1</span>. </li><li> In the fourth situation we can feed the first family, then the third family will get the information from the first family, and the second family will get the information from the third. The answer is <span class="tex-span">1</span>. </li><li> In the fifth situation we can feed the first and the fifth families, so the answer is <span class="tex-span">2</span>. </li></ul>
