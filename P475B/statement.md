## Description

<div><p>Imagine a city with <span class="tex-span"><i>n</i></span> horizontal streets crossing <span class="tex-span"><i>m</i></span> vertical streets, forming an <span class="tex-span">(<i>n</i> - 1) × (<i>m</i> - 1)</span> grid. In order to increase the traffic flow, mayor of the city has decided to make each street one way. This means in each horizontal street, the traffic moves only from west to east or only from east to west. Also, traffic moves only from north to south or only from south to north in each vertical street. It is possible to enter a horizontal street from a vertical street, or vice versa, at their intersection.</p><center> <img class="tex-graphics" src="file://BdbNaoC2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The mayor has received some street direction patterns. Your task is to check whether it is possible to reach any junction from any other junction in the proposed street direction pattern.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 20</span>), denoting the number of horizontal streets and the number of vertical streets.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>, made of characters '<span class="tex-font-style-tt">&lt;</span>' and '<span class="tex-font-style-tt">&gt;</span>', denoting direction of each horizontal street. If the <span class="tex-span"><i>i</i></span>-th character is equal to '<span class="tex-font-style-tt">&lt;</span>', the street is directed from east to west otherwise, the street is directed from west to east. Streets are listed in order from north to south.</p><p>The third line contains a string of length <span class="tex-span"><i>m</i></span>, made of characters '<span class="tex-font-style-tt">^</span>' and '<span class="tex-font-style-tt">v</span>', denoting direction of each vertical street. If the <span class="tex-span"><i>i</i></span>-th character is equal to '<span class="tex-font-style-tt">^</span>', the street is directed from south to north, otherwise the street is directed from north to south. Streets are listed in order from west to east.</p></div><div class="output-specification"><p>If the given pattern meets the mayor's criteria, print a single line containing "<span class="tex-font-style-tt">YES</span>", otherwise print a single line containing "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 20</span>), denoting the number of horizontal streets and the number of vertical streets.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>, made of characters '<span class="tex-font-style-tt">&lt;</span>' and '<span class="tex-font-style-tt">&gt;</span>', denoting direction of each horizontal street. If the <span class="tex-span"><i>i</i></span>-th character is equal to '<span class="tex-font-style-tt">&lt;</span>', the street is directed from east to west otherwise, the street is directed from west to east. Streets are listed in order from north to south.</p><p>The third line contains a string of length <span class="tex-span"><i>m</i></span>, made of characters '<span class="tex-font-style-tt">^</span>' and '<span class="tex-font-style-tt">v</span>', denoting direction of each vertical street. If the <span class="tex-span"><i>i</i></span>-th character is equal to '<span class="tex-font-style-tt">^</span>', the street is directed from south to north, otherwise the street is directed from north to south. Streets are listed in order from west to east.</p>

## Output

<p>If the given pattern meets the mayor's criteria, print a single line containing "<span class="tex-font-style-tt">YES</span>", otherwise print a single line containing "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3 3
&gt;&lt;&gt;
v^v

```




```input2
4 6
&lt;&gt;&lt;&gt;
v^v^v^

```




```output1
NO

```




```output2
YES

```



## Note

<p>The figure above shows street directions in the second sample test case.</p>
