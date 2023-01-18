## Description

<div><p>It is now 125 years later, but humanity is still on the run from a humanoid-cyborg race determined to destroy it. Or perhaps we are getting some stories mixed up here... In any case, the fleet is now smaller. However, in a recent upgrade, all the navigation systems have been outfitted with higher-dimensional, linear-algebraic jump processors.</p><p>Now, in order to make a jump, a ship's captain needs to specify a <span class="tex-font-style-it">subspace</span> of the <span class="tex-span"><i>d</i></span>-dimensional space in which the events are taking place. She does so by providing a generating set of vectors for that subspace.</p><p>Princess Heidi has received such a set from the captain of each of <span class="tex-span"><i>m</i></span> ships. Again, she would like to group up those ships whose hyperspace jump subspaces are equal. To do so, she wants to assign a group number between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span> to each of the ships, so that two ships have the same group number if and only if their corresponding subspaces are equal (even though they might be given using different sets of vectors).</p><p>Help Heidi!</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 5</span>) – the number of ships and the dimension of the full underlying vector space, respectively. Next, the <span class="tex-span"><i>m</i></span> subspaces are described, one after another. The <span class="tex-span"><i>i</i></span>-th subspace, which corresponds to the <span class="tex-span"><i>i</i></span>-th ship, is described as follows:</p><p>The first line contains one integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i></span>). Then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> lines follow, the <span class="tex-span"><i>j</i></span>-th of them describing the <span class="tex-span"><i>j</i></span>-th vector sent by the <span class="tex-span"><i>i</i></span>-th ship. Each of the <span class="tex-span"><i>j</i></span> lines consists of <span class="tex-span"><i>d</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>j</i> = 1, ..., <i>d</i></span>, that describe the vector <img align="middle" class="tex-formula" src="file://Ooge2Yp2.png" style="max-width: 100.0%;max-height: 100.0%;">; it holds that <span class="tex-span">|<i>a</i><sub class="lower-index"><i>j</i></sub>| ≤ 250</span>. The <span class="tex-span"><i>i</i></span>-th subspace is the linear span of these <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> vectors.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, ..., <i>g</i><sub class="lower-index"><i>m</i></sub></span>, where <img align="middle" class="tex-formula" src="file://bphNGitt.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the group number assigned to the <span class="tex-span"><i>i</i></span>-th ship. That is, for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>m</i></span>, the following should hold: <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = <i>g</i><sub class="lower-index"><i>j</i></sub></span> if and only if the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th subspaces are equal. In addition, the sequence <span class="tex-span">(<i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>m</i></sub>)</span> should be lexicographically minimal among all sequences with that property.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 5</span>) – the number of ships and the dimension of the full underlying vector space, respectively. Next, the <span class="tex-span"><i>m</i></span> subspaces are described, one after another. The <span class="tex-span"><i>i</i></span>-th subspace, which corresponds to the <span class="tex-span"><i>i</i></span>-th ship, is described as follows:</p><p>The first line contains one integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i></span>). Then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> lines follow, the <span class="tex-span"><i>j</i></span>-th of them describing the <span class="tex-span"><i>j</i></span>-th vector sent by the <span class="tex-span"><i>i</i></span>-th ship. Each of the <span class="tex-span"><i>j</i></span> lines consists of <span class="tex-span"><i>d</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>j</i> = 1, ..., <i>d</i></span>, that describe the vector <img align="middle" class="tex-formula" src="file://Ooge2Yp2.png" style="max-width: 100.0%;max-height: 100.0%;">; it holds that <span class="tex-span">|<i>a</i><sub class="lower-index"><i>j</i></sub>| ≤ 250</span>. The <span class="tex-span"><i>i</i></span>-th subspace is the linear span of these <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> vectors.</p>

## Output

<p>Output <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, ..., <i>g</i><sub class="lower-index"><i>m</i></sub></span>, where <img align="middle" class="tex-formula" src="file://bphNGitt.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the group number assigned to the <span class="tex-span"><i>i</i></span>-th ship. That is, for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>m</i></span>, the following should hold: <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = <i>g</i><sub class="lower-index"><i>j</i></sub></span> if and only if the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th subspaces are equal. In addition, the sequence <span class="tex-span">(<i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>m</i></sub>)</span> should be lexicographically minimal among all sequences with that property.</p>





```input1
8 2
1
5 0
1
0 1
1
0 1
2
0 6
0 1
2
0 1
1 0
2
-5 -5
4 3
2
1 1
0 1
2
1 0
1 0

```




```output1
1 2 2 2 3 3 3 1
```



## Note

<p>In the sample testcase, the first and the last subspace are equal, subspaces 2 to 4 are equal, and subspaces 5 to 7 are equal.</p><p>Recall that two subspaces, one given as the span of vectors <img align="middle" class="tex-formula" src="file://sVbTyMOs.png" style="max-width: 100.0%;max-height: 100.0%;"> and another given as the span of vectors <img align="middle" class="tex-formula" src="file://4tHu0L1y.png" style="max-width: 100.0%;max-height: 100.0%;">, are equal if each vector <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> can be written as a linear combination of vectors <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>k</i></sub></span> (that is, there exist coefficients <img align="middle" class="tex-formula" src="file://tmSpEbE8.png" style="max-width: 100.0%;max-height: 100.0%;"> such that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = α<sub class="lower-index">1</sub><i>w</i><sub class="lower-index">1</sub> + ... + α<sub class="lower-index"><i>k</i></sub><i>w</i><sub class="lower-index"><i>k</i></sub></span>) and, similarly, each vector <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> can be written as a linear combination of vectors <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Recall that a sequence <span class="tex-span">(<i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>m</i></sub>)</span> is lexicographically smaller than a sequence <span class="tex-span">(<i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>m</i></sub>)</span> if there exists an index <span class="tex-span"><i>i</i></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>, such that <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> &lt; <i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub> = <i>h</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>j</i> &lt; <i>i</i></span>.</p>
