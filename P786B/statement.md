## Description

<div><p>Rick and his co-workers have made a new radioactive formula and a lot of bad guys are after them. So Rick wants to give his legacy to Morty before bad guys catch them. </p><p>There are <span class="tex-span"><i>n</i></span> planets in their universe numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Rick is in planet number <span class="tex-span"><i>s</i></span> (the earth) and he doesn't know where Morty is. As we all know, Rick owns a portal gun. With this gun he can open one-way portal from a planet he is in to any other planet (including that planet). But there are limits on this gun because he's still using its free trial.</p><center> <img class="tex-graphics" src="file://lQacinHy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>By default he can not open any portal by this gun. There are <span class="tex-span"><i>q</i></span> plans in the website that sells these guns. Every time you purchase a plan you can only use it once but you can purchase it again if you want to use it more.</p><p>Plans on the website have three types:</p><ol> <li> With a plan of this type you can open a portal from planet <span class="tex-span"><i>v</i></span> to planet <span class="tex-span"><i>u</i></span>. </li><li> With a plan of this type you can open a portal from planet <span class="tex-span"><i>v</i></span> to any planet with index in range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. </li><li> With a plan of this type you can open a portal from any planet with index in range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> to planet <span class="tex-span"><i>v</i></span>. </li></ol><p>Rick doesn't known where Morty is, but Unity is going to inform him and he wants to be prepared for when he finds and start his journey immediately. So for each planet (including earth itself) he wants to know the minimum amount of money he needs to get from earth to that planet.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — number of planets, number of plans and index of earth respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the plans. Each line starts with a number <span class="tex-span"><i>t</i></span>, type of that plan (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>). If <span class="tex-span"><i>t</i> = 1</span> then it is followed by three integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>w</i></span> where <span class="tex-span"><i>w</i></span> is the cost of that plan (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>). Otherwise it is followed by four integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>w</i></span> where <span class="tex-span"><i>w</i></span> is the cost of that plan (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first and only line of output print <span class="tex-span"><i>n</i></span> integers separated by spaces. <span class="tex-span"><i>i</i></span>-th of them should be minimum money to get from earth to <span class="tex-span"><i>i</i></span>-th planet, or <span class="tex-span"> - 1</span> if it's impossible to get to that planet.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — number of planets, number of plans and index of earth respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the plans. Each line starts with a number <span class="tex-span"><i>t</i></span>, type of that plan (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>). If <span class="tex-span"><i>t</i> = 1</span> then it is followed by three integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>w</i></span> where <span class="tex-span"><i>w</i></span> is the cost of that plan (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>). Otherwise it is followed by four integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>w</i></span> where <span class="tex-span"><i>w</i></span> is the cost of that plan (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first and only line of output print <span class="tex-span"><i>n</i></span> integers separated by spaces. <span class="tex-span"><i>i</i></span>-th of them should be minimum money to get from earth to <span class="tex-span"><i>i</i></span>-th planet, or <span class="tex-span"> - 1</span> if it's impossible to get to that planet.</p>





```input1
3 5 1
2 3 2 3 17
2 3 2 2 16
2 2 2 3 3
3 3 1 1 12
1 3 3 17

```




```input2
4 3 1
3 4 1 3 12
2 2 3 4 10
1 2 4 16

```




```output1
0 28 12 

```




```output2
0 -1 -1 12 

```



## Note

<p>In the first sample testcase, Rick can purchase <span class="tex-span">4</span>th plan once and then <span class="tex-span">2</span>nd plan in order to get to get to planet number <span class="tex-span">2</span>.</p>
