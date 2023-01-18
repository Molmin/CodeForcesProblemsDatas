## Description

<div><p>Barney lives in country USC (United States of Charzeh). USC has <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>n</i> - 1</span> roads between them. Cities and roads of USC form a rooted tree (Barney's not sure why it is rooted). Root of the tree is the city number <span class="tex-span">1</span>. Thus if one will start his journey from city <span class="tex-span">1</span>, he can visit any city he wants by following roads.</p><center> <img class="tex-graphics" src="file://K5egXefK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Some girl has stolen Barney's heart, and Barney wants to find her. He starts looking for in the root of the tree and (since he is Barney Stinson not a random guy), he uses a <span class="tex-font-style-it">random DFS</span> to search in the cities. A pseudo code of this algorithm is as follows:</p><pre class="verbatim"><br>let starting_time be an array of length n<br>current_time = 0<br>dfs(v):<br>	current_time = current_time + 1<br>	starting_time[v] = current_time<br>	shuffle children[v] randomly (each permutation with equal possibility)<br>	// children[v] is vector of children cities of city v<br>	for u in children[v]:<br>		dfs(u)<br></pre><p>As told before, Barney will start his journey in the root of the tree (equivalent to call <span class="tex-font-style-tt">dfs(1)</span>).</p><p>Now Barney needs to pack a backpack and so he wants to know more about his upcoming journey: for every city <span class="tex-span"><i>i</i></span>, Barney wants to know the expected value of <span class="tex-font-style-tt">starting_time[i]</span>. He's a friend of Jon Snow and knows nothing, that's why he asked for your help.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities in USC.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number of the parent city of city number <span class="tex-span"><i>i</i></span> in the tree, meaning there is a road between cities numbered <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>i</i></span> in USC.</p></div><div class="output-specification"><p>In the first and only line of output print <span class="tex-span"><i>n</i></span> numbers, where <span class="tex-span"><i>i</i></span>-th number is the expected value of <span class="tex-font-style-tt">starting_time[i]</span>.</p><p>Your answer for each city will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities in USC.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number of the parent city of city number <span class="tex-span"><i>i</i></span> in the tree, meaning there is a road between cities numbered <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>i</i></span> in USC.</p>

## Output

<p>In the first and only line of output print <span class="tex-span"><i>n</i></span> numbers, where <span class="tex-span"><i>i</i></span>-th number is the expected value of <span class="tex-font-style-tt">starting_time[i]</span>.</p><p>Your answer for each city will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
7
1 2 1 1 4 4

```




```input2
12
1 1 2 2 4 4 3 3 1 10 8

```




```output1
1.0 4.0 5.0 3.5 4.5 5.0 5.0 

```




```output2
1.0 5.0 5.5 6.5 7.5 8.0 8.0 7.0 7.5 6.5 7.5 8.0 

```


