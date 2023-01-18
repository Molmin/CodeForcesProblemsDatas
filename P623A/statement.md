## Description

<div><p>One day student Vasya was sitting on a lecture and mentioned a string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span>, consisting of letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" that was written on his desk. As the lecture was boring, Vasya decided to complete the picture by composing a graph <span class="tex-span"><i>G</i></span> with the following properties: </p><ul> <li> <span class="tex-span"><i>G</i></span> has exactly <span class="tex-span"><i>n</i></span> vertices, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </li><li> For all pairs of vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, where <span class="tex-span"><i>i</i> ≠ <i>j</i></span>, there is an edge connecting them <span class="tex-font-style-bf">if and only if</span> characters <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> are either equal or neighbouring in the alphabet. That is, letters in pairs "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">b</span>"-"<span class="tex-font-style-tt">c</span>" are neighbouring, while letters "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">c</span>" are not. </li></ul><p>Vasya painted the resulting graph near the string and then erased the string. Next day Vasya's friend Petya came to a lecture and found some graph at his desk. He had heard of Vasya's adventure and now he wants to find out whether it could be the original graph <span class="tex-span"><i>G</i></span>, painted by Vasya. In order to verify this, Petya needs to know whether there exists a string <span class="tex-span"><i>s</i></span>, such that if Vasya used this <span class="tex-span"><i>s</i></span> he would produce the given graph <span class="tex-span"><i>G</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://cuJbyX7A.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the number of vertices and edges in the graph found by Petya, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>&nbsp;— the edges of the graph <span class="tex-span"><i>G</i></span>. It is guaranteed, that there are no multiple edges, that is any pair of vertexes appear in this list no more than once.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the string <span class="tex-span"><i>s</i></span> Petya is interested in really exists and "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise.</p><p>If the string <span class="tex-span"><i>s</i></span> exists, then print it on the second line of the output. The length of <span class="tex-span"><i>s</i></span> must be exactly <span class="tex-span"><i>n</i></span>, it must consist of only letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" only, and the graph built using this string must coincide with <span class="tex-span"><i>G</i></span>. If there are multiple possible answers, you may print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://cuJbyX7A.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the number of vertices and edges in the graph found by Petya, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>&nbsp;— the edges of the graph <span class="tex-span"><i>G</i></span>. It is guaranteed, that there are no multiple edges, that is any pair of vertexes appear in this list no more than once.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the string <span class="tex-span"><i>s</i></span> Petya is interested in really exists and "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise.</p><p>If the string <span class="tex-span"><i>s</i></span> exists, then print it on the second line of the output. The length of <span class="tex-span"><i>s</i></span> must be exactly <span class="tex-span"><i>n</i></span>, it must consist of only letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" only, and the graph built using this string must coincide with <span class="tex-span"><i>G</i></span>. If there are multiple possible answers, you may print any of them.</p>





```input1
2 1
1 2

```




```input2
4 3
1 2
1 3
1 4

```




```output1
Yes
aa

```




```output2
No

```



## Note

<p>In the first sample you are given a graph made of two vertices with an edge between them. So, these vertices can correspond to both the same and adjacent letters. Any of the following strings <span class="tex-font-style-tt">"</span>aa<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>ab<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>ba<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>bb<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>bc<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>cb<span class="tex-font-style-tt">"</span>, <span class="tex-font-style-tt">"</span>cc<span class="tex-font-style-tt">"</span> meets the graph's conditions. </p><p>In the second sample the first vertex is connected to all three other vertices, but these three vertices are not connected with each other. That means that they must correspond to distinct letters that are not adjacent, but that is impossible as there are only two such letters: a and c.</p>
