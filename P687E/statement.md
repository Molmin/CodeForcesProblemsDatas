## Description

<div><p>Today Pari gave Arya a cool graph problem. Arya wrote a non-optimal solution for it, because he believes in his ability to optimize non-optimal solutions. In addition to being non-optimal, his code was buggy and he tried a lot to optimize it, so the code also became dirty! He keeps getting Time Limit Exceeds and he is disappointed. Suddenly a bright idea came to his mind!</p><p>Here is how his dirty code looks like:</p><pre class="verbatim"><br>dfs(v)<br>{<br>     set count[v] = count[v] + 1<br>     if(count[v] &lt; 1000)<br>     {<br>          foreach u in neighbors[v]<br>          {<br>               if(visited[u] is equal to false)<br>               {<br>                    dfs(u)<br>               }<br>               break<br>          }<br>     }<br>     set visited[v] = true<br>}<br><br>main()<br>{<br>     input the digraph()<br>     TOF()<br>     foreach 1&lt;=i&lt;=n<br>     {<br>          set count[i] = 0 , visited[i] = false<br>     }<br>     foreach 1 &lt;= v &lt;= n<br>     {<br>          if(visited[v] is equal to false)<br>          {<br>               dfs(v)<br>          }<br>     }<br>     ... // And do something cool and magical but we can't tell you what!<br>}<br></pre><p>He asks you to write the <span class="tex-font-style-underline">TOF</span> function in order to optimize the running time of the code with minimizing the number of calls of the <span class="tex-font-style-underline">dfs</span> function. The input is a directed graph and in the <span class="tex-font-style-underline">TOF</span> function you have to rearrange the edges of the graph in the list <span class="tex-font-style-underline">neighbors</span> for each vertex. The number of calls of <span class="tex-font-style-underline">dfs</span> function depends on the arrangement of <span class="tex-font-style-underline">neighbors</span> of each vertex.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>)&nbsp;— the number of vertices and then number of directed edges in the input graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>), meaning there is a directed <img align="middle" class="tex-formula" src="file://FydDHPB2.png" style="max-width: 100.0%;max-height: 100.0%;"> edge in the input graph. </p><p>You may assume that the graph won't contain any self-loops and there is at most one edge between any unordered pair of vertices.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum possible number of <span class="tex-font-style-underline">dfs</span> calls that can be achieved with permuting the edges.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>)&nbsp;— the number of vertices and then number of directed edges in the input graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>), meaning there is a directed <img align="middle" class="tex-formula" src="file://FydDHPB2.png" style="max-width: 100.0%;max-height: 100.0%;"> edge in the input graph. </p><p>You may assume that the graph won't contain any self-loops and there is at most one edge between any unordered pair of vertices.</p>

## Output

<p>Print a single integer&nbsp;— the minimum possible number of <span class="tex-font-style-underline">dfs</span> calls that can be achieved with permuting the edges.</p>





```input1
3 3
1 2
2 3
3 1

```




```input2
6 7
1 2
2 3
3 1
3 4
4 5
5 6
6 4

```




```output1
2998

```




```output2
3001

```


