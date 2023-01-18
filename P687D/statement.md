## Description

<div><p>Long time ago, there was a great kingdom and it was being ruled by The Great Arya and Pari The Great. These two had some problems about the numbers they like, so they decided to divide the great kingdom between themselves.</p><p>The great kingdom consisted of <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> bidirectional roads between these cities, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. The <span class="tex-span"><i>i</i></span>-th road had length equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The Great Arya and Pari The Great were discussing about destructing some prefix (all road with numbers less than some <span class="tex-span"><i>x</i></span>) and suffix (all roads with numbers greater than some <span class="tex-span"><i>x</i></span>) of the roads so there will remain only the roads with numbers <span class="tex-span"><i>l</i>, <i>l</i> + 1, ..., <i>r</i> - 1</span> and <span class="tex-span"><i>r</i></span>.</p><p>After that they will divide the great kingdom into two pieces (with each city belonging to exactly one piece) such that the <span class="tex-font-style-it">hardness</span> of the division is <span class="tex-font-style-bf">minimized</span>. The hardness of a division is the <span class="tex-font-style-bf">maximum length</span> of a road such that its both endpoints are in the same piece of the kingdom. In case there is no such road, the hardness of the division is considered to be equal to <span class="tex-span"> - 1</span>.</p><p>Historians found the map of the great kingdom, and they have <span class="tex-span"><i>q</i></span> guesses about the <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> chosen by those great rulers. Given these data, for each guess <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> print the minimum possible hardness of the division of the kingdom.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 1000</span>, <img align="middle" class="tex-formula" src="file://Q2xP3X9h.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and roads in the great kingdom, and the number of guesses, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th line of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i>, 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the road number <span class="tex-span"><i>i</i></span> connects cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and its length is equal <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that no road connects the city to itself and no pair of cities is connected by more than one road.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— a guess from the historians about the remaining roads in the kingdom.</p></div><div class="output-specification"><p>For each guess print the minimum possible hardness of the division in described scenario.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 1000</span>, <img align="middle" class="tex-formula" src="file://Q2xP3X9h.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and roads in the great kingdom, and the number of guesses, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th line of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i>, 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the road number <span class="tex-span"><i>i</i></span> connects cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and its length is equal <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that no road connects the city to itself and no pair of cities is connected by more than one road.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— a guess from the historians about the remaining roads in the kingdom.</p>

## Output

<p>For each guess print the minimum possible hardness of the division in described scenario.</p>





```input1
5 6 5
5 4 86
5 1 0
1 3 38
2 1 33
2 4 28
2 3 40
3 5
2 6
1 3
2 3
1 6

```




```output1
-1
33
-1
-1
33

```


