## Description

<div><p>To stay woke and attentive during classes, Karen needs some coffee!</p><center> <img class="tex-graphics" src="file://fvIMYFZZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Karen, a coffee aficionado, wants to know the optimal temperature for brewing the perfect cup of coffee. Indeed, she has spent some time reading several recipe books, including the universally acclaimed "The Art of the Covfefe".</p><p>She knows <span class="tex-span"><i>n</i></span> coffee recipes. The <span class="tex-span"><i>i</i></span>-th recipe suggests that coffee should be brewed between <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> degrees, inclusive, to achieve the optimal taste.</p><p>Karen thinks that a temperature is <span class="tex-font-style-it">admissible</span> if at least <span class="tex-span"><i>k</i></span> recipes recommend it.</p><p>Karen has a rather fickle mind, and so she asks <span class="tex-span"><i>q</i></span> questions. In each question, given that she only wants to prepare coffee with a temperature between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, inclusive, can you tell her how many admissible integer temperatures fall within the range?</p></div><div class="input-specification"><p>The first line of input contains three integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200000</span>), and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>), the number of recipes, the minimum number of recipes a certain temperature must be recommended by to be admissible, and the number of questions Karen has, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the recipes. Specifically, the <span class="tex-span"><i>i</i></span>-th line among these contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>), describing that the <span class="tex-span"><i>i</i></span>-th recipe suggests that the coffee be brewed between <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> degrees, inclusive.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the questions. Each of these lines contains <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 200000</span>), describing that she wants to know the number of admissible integer temperatures between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> degrees, inclusive.</p></div><div class="output-specification"><p>For each question, output a single integer on a line by itself, the number of admissible integer temperatures between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> degrees, inclusive.</p></div>

## Input

<p>The first line of input contains three integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200000</span>), and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>), the number of recipes, the minimum number of recipes a certain temperature must be recommended by to be admissible, and the number of questions Karen has, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the recipes. Specifically, the <span class="tex-span"><i>i</i></span>-th line among these contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>), describing that the <span class="tex-span"><i>i</i></span>-th recipe suggests that the coffee be brewed between <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> degrees, inclusive.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the questions. Each of these lines contains <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 200000</span>), describing that she wants to know the number of admissible integer temperatures between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> degrees, inclusive.</p>

## Output

<p>For each question, output a single integer on a line by itself, the number of admissible integer temperatures between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> degrees, inclusive.</p>





```input1
3 2 4
91 94
92 97
97 99
92 94
93 97
95 96
90 100

```




```input2
2 1 1
1 1
200000 200000
90 100

```




```output1
3
3
0
4

```




```output2
0

```



## Note

<p>In the first test case, Karen knows <span class="tex-span">3</span> recipes.</p><ol> <li> The first one recommends brewing the coffee between <span class="tex-span">91</span> and <span class="tex-span">94</span> degrees, inclusive. </li><li> The second one recommends brewing the coffee between <span class="tex-span">92</span> and <span class="tex-span">97</span> degrees, inclusive. </li><li> The third one recommends brewing the coffee between <span class="tex-span">97</span> and <span class="tex-span">99</span> degrees, inclusive. </li></ol><p>A temperature is <span class="tex-font-style-it">admissible</span> if at least <span class="tex-span">2</span> recipes recommend it.</p><p>She asks <span class="tex-span">4</span> questions.</p><p>In her first question, she wants to know the number of admissible integer temperatures between <span class="tex-span">92</span> and <span class="tex-span">94</span> degrees, inclusive. There are <span class="tex-span">3</span>: <span class="tex-span">92</span>, <span class="tex-span">93</span> and <span class="tex-span">94</span> degrees are all admissible.</p><p>In her second question, she wants to know the number of admissible integer temperatures between <span class="tex-span">93</span> and <span class="tex-span">97</span> degrees, inclusive. There are <span class="tex-span">3</span>: <span class="tex-span">93</span>, <span class="tex-span">94</span> and <span class="tex-span">97</span> degrees are all admissible.</p><p>In her third question, she wants to know the number of admissible integer temperatures between <span class="tex-span">95</span> and <span class="tex-span">96</span> degrees, inclusive. There are none.</p><p>In her final question, she wants to know the number of admissible integer temperatures between <span class="tex-span">90</span> and <span class="tex-span">100</span> degrees, inclusive. There are <span class="tex-span">4</span>: <span class="tex-span">92</span>, <span class="tex-span">93</span>, <span class="tex-span">94</span> and <span class="tex-span">97</span> degrees are all admissible.</p><p>In the second test case, Karen knows <span class="tex-span">2</span> recipes.</p><ol> <li> The first one, "wikiHow to make Cold Brew Coffee", recommends brewing the coffee at exactly <span class="tex-span">1</span> degree. </li><li> The second one, "What good is coffee that isn't brewed at at least <span class="tex-span">36.3306</span> times the temperature of the surface of the sun?", recommends brewing the coffee at exactly <span class="tex-span">200000</span> degrees. </li></ol><p>A temperature is <span class="tex-font-style-it">admissible</span> if at least <span class="tex-span">1</span> recipe recommends it.</p><p>In her first and only question, she wants to know the number of admissible integer temperatures that are actually reasonable. There are none.</p>
