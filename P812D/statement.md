## Description

<div><p>Sagheer is working at a kindergarten. There are <span class="tex-span"><i>n</i></span> children and <span class="tex-span"><i>m</i></span> different toys. These children use well-defined protocols for playing with the toys:</p><ul> <li> Each child has a lovely set of toys that he loves to play with. He requests the toys one after another at distinct moments of time. A child starts playing if and only if he is granted all the toys in his lovely set.</li><li> If a child starts playing, then sooner or later he gives the toys back. No child keeps the toys forever.</li><li> Children request toys at distinct moments of time. No two children request a toy at the same time.</li><li> If a child is granted a toy, he never gives it back until he finishes playing with his lovely set.</li><li> If a child is not granted a toy, he waits until he is granted this toy. He can't request another toy while waiting.</li><li> If two children are waiting for the same toy, then the child who requested it first will take the toy first.</li></ul><p>Children don't like to play with each other. That's why they never share toys. When a child requests a toy, then granting the toy to this child depends on whether the toy is free or not. If the toy is free, Sagheer will give it to the child. Otherwise, the child has to wait for it and can't request another toy.</p><p>Children are smart and can detect if they have to wait forever before they get the toys they want. In such case they start crying. In other words, a crying set is a set of children in which each child is waiting for a toy that is kept by another child in the set.</p><p>Now, we have reached a scenario where all the children made all the requests for their lovely sets, except for one child <span class="tex-span"><i>x</i></span> that still has one last request for his lovely set. Some children are playing while others are waiting for a toy, but no child is crying, and no one has yet finished playing. If the child <span class="tex-span"><i>x</i></span> is currently waiting for some toy, he makes his last request just after getting that toy. Otherwise, he makes the request right away. When child <span class="tex-span"><i>x</i></span> will make his last request, how many children will start crying?</p><p>You will be given the scenario and <span class="tex-span"><i>q</i></span> <span class="tex-font-style-bf">independent</span> queries. Each query will be of the form <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> meaning that the last request of the child <span class="tex-span"><i>x</i></span> is for the toy <span class="tex-span"><i>y</i></span>. Your task is to help Sagheer find the size of the <span class="tex-font-style-bf">maximal</span> crying set when child <span class="tex-span"><i>x</i></span> makes his last request.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of children, toys, scenario requests and queries.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i></span>)&nbsp;— a scenario request meaning child <span class="tex-span"><i>a</i></span> requests toy <span class="tex-span"><i>b</i></span>. The requests are given in the order they are made by children.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>)&nbsp;— the request to be added to the scenario meaning child <span class="tex-span"><i>x</i></span> will request toy <span class="tex-span"><i>y</i></span> just after getting the toy he is waiting for (if any).</p><p>It is guaranteed that the scenario requests are consistent and no child is initially crying. All the scenario requests are distinct and no query coincides with a scenario request.</p></div><div class="output-specification"><p>For each query, print on a single line the number of children who will start crying when child <span class="tex-span"><i>x</i></span> makes his last request for toy <span class="tex-span"><i>y</i></span>. Please answer all queries independent of each other.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of children, toys, scenario requests and queries.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i></span>)&nbsp;— a scenario request meaning child <span class="tex-span"><i>a</i></span> requests toy <span class="tex-span"><i>b</i></span>. The requests are given in the order they are made by children.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>)&nbsp;— the request to be added to the scenario meaning child <span class="tex-span"><i>x</i></span> will request toy <span class="tex-span"><i>y</i></span> just after getting the toy he is waiting for (if any).</p><p>It is guaranteed that the scenario requests are consistent and no child is initially crying. All the scenario requests are distinct and no query coincides with a scenario request.</p>

## Output

<p>For each query, print on a single line the number of children who will start crying when child <span class="tex-span"><i>x</i></span> makes his last request for toy <span class="tex-span"><i>y</i></span>. Please answer all queries independent of each other.</p>





```input1
3 3 5 1
1 1
2 2
3 3
1 2
2 3
3 1

```




```input2
5 4 7 2
1 1
2 2
2 1
5 1
3 3
4 4
4 1
5 3
5 4

```




```output1
3

```




```output2
0
2

```



## Note

<p>In the first example, child <span class="tex-span">1</span> is waiting for toy <span class="tex-span">2</span>, which child <span class="tex-span">2</span> has, while child <span class="tex-span">2</span> is waiting for top <span class="tex-span">3</span>, which child <span class="tex-span">3</span> has. When child <span class="tex-span">3</span> makes his last request, the toy he requests is held by child <span class="tex-span">1</span>. Each of the three children is waiting for a toy held by another child and no one is playing, so all the three will start crying.</p><p>In the second example, at the beginning, child <span class="tex-span"><i>i</i></span> is holding toy <span class="tex-span"><i>i</i></span> for <span class="tex-span">1 ≤ <i>i</i> ≤ 4</span>. Children <span class="tex-span">1</span> and <span class="tex-span">3</span> have completed their lovely sets. After they finish playing, toy <span class="tex-span">3</span> will be free while toy <span class="tex-span">1</span> will be taken by child <span class="tex-span">2</span> who has just completed his lovely set. After he finishes, toys <span class="tex-span">1</span> and <span class="tex-span">2</span> will be free and child <span class="tex-span">5</span> will take toy <span class="tex-span">1</span>. Now:</p><ul> <li> In the first query, child <span class="tex-span">5</span> will take toy <span class="tex-span">3</span> and after he finishes playing, child <span class="tex-span">4</span> can play.</li><li> In the second query, child <span class="tex-span">5</span> will request toy <span class="tex-span">4</span> which is held by child <span class="tex-span">4</span>. At the same time, child <span class="tex-span">4</span> is waiting for toy <span class="tex-span">1</span> which is now held by child <span class="tex-span">5</span>. None of them can play and they will start crying. </li></ul>
