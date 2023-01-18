## Description

<div><p>Limak is a little grizzly bear. He will once attack Deerland but now he can only destroy trees in role-playing games. Limak starts with a tree with one vertex. The only vertex has index <span class="tex-span">1</span> and is a root of the tree.</p><p>Sometimes, a game chooses a subtree and allows Limak to attack it. When a subtree is attacked then each of its edges is destroyed with probability <img align="middle" class="tex-formula" src="file://M4N6InJ9.png" style="max-width: 100.0%;max-height: 100.0%;">, independently of other edges. Then, Limak gets the penalty&nbsp;— an integer equal to the height of the subtree after the attack. The height is defined as the maximum number of edges on the path between the root of the subtree and any vertex in the subtree.</p><p>You must handle queries of two types.</p><ul> <li> <span class="tex-font-style-tt">1 v</span> denotes a query of the first type. A new vertex appears and its parent is <span class="tex-span"><i>v</i></span>. A new vertex has the next available index (so, new vertices will be numbered <span class="tex-span">2, 3, ...</span>). </li><li> <span class="tex-font-style-tt">2 v</span> denotes a query of the second type. For a moment let's assume that the game allows Limak to attack a subtree rooted in <span class="tex-span"><i>v</i></span>. Then, what would be the expected value of the penalty Limak gets after the attack? </li></ul><p>In a query of the second type, Limak doesn't actually attack the subtree and thus the query doesn't affect next queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500 000</span>)&nbsp;— the number of queries.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> denotes a parent of a new vertex, while if <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span> then you should print the answer for a subtree rooted in <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It's guaranteed that there will be at least <span class="tex-span">1</span> query of the second type, that is, the output won't be empty.</p><p>It's guaranteed that just before the <span class="tex-span"><i>i</i></span>-th query a vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> already exists.</p></div><div class="output-specification"><p>For each query of the second type print one real number&nbsp;—the expected value of the penalty if Limak attacks the given subtree. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://ZAnk5EXA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500 000</span>)&nbsp;— the number of queries.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> denotes a parent of a new vertex, while if <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span> then you should print the answer for a subtree rooted in <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It's guaranteed that there will be at least <span class="tex-span">1</span> query of the second type, that is, the output won't be empty.</p><p>It's guaranteed that just before the <span class="tex-span"><i>i</i></span>-th query a vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> already exists.</p>

## Output

<p>For each query of the second type print one real number&nbsp;—the expected value of the penalty if Limak attacks the given subtree. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://ZAnk5EXA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
7
1 1
1 1
2 1
1 2
1 3
2 2
2 1

```




```input2
8
2 1
1 1
1 2
1 3
1 4
2 1
1 4
2 1

```




```output1
0.7500000000
0.5000000000
1.1875000000

```




```output2
0.0000000000
0.9375000000
0.9687500000

```



## Note

<p>Below, you can see the drawing for the first sample. Red circles denote queries of the second type.</p><center> <img class="tex-graphics" src="file://k7f9RVNz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
