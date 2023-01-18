## Description

<div><p>Harry, upon inquiring Helena Ravenclaw's ghost, came to know that she told Tom Riddle or You-know-who about Rowena Ravenclaw's diadem and that he stole it from her. </p><p>Harry thought that Riddle would have assumed that he was the only one to discover the Room of Requirement and thus, would have hidden it there. So Harry is trying to get inside the Room of Requirement to destroy the diadem as he knows that it is a horcrux.</p><p>But he has to answer a puzzle in order to enter the room. He is given <span class="tex-span"><i>n</i></span> objects, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some of the objects have a parent object, that has a lesser number. Formally, object <span class="tex-span"><i>i</i></span> may have a parent object <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span> such that <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>.</p><p>There is also a type associated with each parent relation, it can be either of type <span class="tex-span">1</span> or type <span class="tex-span">2</span>. Type <span class="tex-span">1</span> relation means that the child object is like a special case of the parent object. Type <span class="tex-span">2</span> relation means that the second object is <span class="tex-font-style-bf">always</span> a part of the first object and all its special cases.</p><p>Note that if an object <span class="tex-span"><i>b</i></span> is a special case of object <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>c</i></span> is a special case of object <span class="tex-span"><i>b</i></span>, then <span class="tex-span"><i>c</i></span> is considered to be a special case of object <span class="tex-span"><i>a</i></span> as well. The same holds for parts: if object <span class="tex-span"><i>b</i></span> is a part of <span class="tex-span"><i>a</i></span>, and object <span class="tex-span"><i>c</i></span> is a part of <span class="tex-span"><i>b</i></span>, then we say that object <span class="tex-span"><i>c</i></span> is a part of <span class="tex-span"><i>a</i></span>. Also note, that if object <span class="tex-span"><i>b</i></span> is a part of <span class="tex-span"><i>a</i></span>, and object <span class="tex-span"><i>c</i></span> is a special case of <span class="tex-span"><i>a</i></span>, then <span class="tex-span"><i>b</i></span> is a part of <span class="tex-span"><i>c</i></span> as well.</p><p>An object is considered to be neither a part of itself nor a special case of itself.</p><p>Now, Harry has to answer two type of queries:</p><ul> <li> <span class="tex-font-style-tt">1 u v</span>: he needs to tell if object <span class="tex-span"><i>v</i></span> is a special case of object <span class="tex-span"><i>u</i></span>. </li><li> <span class="tex-font-style-tt">2 u v</span>: he needs to tell if object <span class="tex-span"><i>v</i></span> is a part of object <span class="tex-span"><i>u</i></span>. </li></ul></div><div class="input-specification"><p>First line of input contains the number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of objects. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integer <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>parent</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span> <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>, <span class="tex-span"> - 1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), implying that the <span class="tex-span"><i>i</i></span>-th object has the parent <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>. (If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 0</span>, this implies that the object <span class="tex-span"><i>i</i></span> is a special case of object <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span>, this implies that the object <span class="tex-span"><i>i</i></span> is a part of object <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>). In case the <span class="tex-span"><i>i</i></span>-th object has no parent, both <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-tt">-1</span>.</p><p>Next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of queries. </p><p>Next <span class="tex-span"><i>q</i></span> lines each represent a query having three space separated integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Output will contain <span class="tex-span"><i>q</i></span> lines, each containing the answer for the corresponding query as "<span class="tex-font-style-tt">YES</span>" (affirmative) or "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can output each letter in any case (upper or lower).</p></div>

## Input

<p>First line of input contains the number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of objects. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integer <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>parent</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span> <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>, <span class="tex-span"> - 1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), implying that the <span class="tex-span"><i>i</i></span>-th object has the parent <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>. (If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 0</span>, this implies that the object <span class="tex-span"><i>i</i></span> is a special case of object <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span>, this implies that the object <span class="tex-span"><i>i</i></span> is a part of object <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span>). In case the <span class="tex-span"><i>i</i></span>-th object has no parent, both <span class="tex-span"><i>parent</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-tt">-1</span>.</p><p>Next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of queries. </p><p>Next <span class="tex-span"><i>q</i></span> lines each represent a query having three space separated integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>).</p>

## Output

<p>Output will contain <span class="tex-span"><i>q</i></span> lines, each containing the answer for the corresponding query as "<span class="tex-font-style-tt">YES</span>" (affirmative) or "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can output each letter in any case (upper or lower).</p>





```input1
3
-1 -1
1 0
2 0
2
1 1 3
2 1 3

```




```input2
3
-1 -1
1 0
1 1
2
2 2 3
2 3 2

```




```output1
YES
NO

```




```output2
YES
NO

```



## Note

<p>In test case <span class="tex-span">1</span>, as object <span class="tex-span">2</span> is a special case of object <span class="tex-span">1</span> and object <span class="tex-span">3</span> is a special case of object <span class="tex-span">2</span>, this makes object <span class="tex-span">3</span> a special case of object <span class="tex-span">1</span>.</p><p>In test case <span class="tex-span">2</span>, as object <span class="tex-span">2</span> is a special case of object <span class="tex-span">1</span> and object <span class="tex-span">1</span> has object <span class="tex-span">3</span>, this will mean that object <span class="tex-span">2</span> will also have object <span class="tex-span">3</span>. This is because when a general case (object <span class="tex-span">1</span>) has object <span class="tex-span">3</span>, its special case (object <span class="tex-span">2</span>) will definitely have object <span class="tex-span">3</span>.</p>
