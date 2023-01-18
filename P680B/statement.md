## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in Bearland, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Cities are arranged in one long row. The distance between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is equal to <span class="tex-span">|<i>i</i> - <i>j</i>|</span>.</p><p>Limak is a police officer. He lives in a city <span class="tex-span"><i>a</i></span>. His job is to catch criminals. It's hard because he doesn't know in which cities criminals are. Though, he knows that there is <span class="tex-font-style-bf">at most one</span> criminal in each city.</p><p>Limak is going to use a BCD (Bear Criminal Detector). The BCD will tell Limak how many criminals there are for every distance from a city <span class="tex-span"><i>a</i></span>. After that, Limak can catch a criminal in each city for which he <span class="tex-font-style-bf">is sure</span> that there must be a criminal.</p><p>You know in which cities criminals are. Count the number of criminals Limak will catch, after he uses the BCD.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cities and the index of city where Limak lives.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). There are <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> criminals in the <span class="tex-span"><i>i</i></span>-th city.</p></div><div class="output-specification"><p>Print the number of criminals Limak will catch.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cities and the index of city where Limak lives.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). There are <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> criminals in the <span class="tex-span"><i>i</i></span>-th city.</p>

## Output

<p>Print the number of criminals Limak will catch.</p>





```input1
6 3
1 1 1 0 1 0

```




```input2
5 2
0 0 0 1 0

```




```output1
3

```




```output2
1

```



## Note

<p>In the first sample, there are six cities and Limak lives in the third one (blue arrow below). Criminals are in cities marked red.</p><center> <img class="tex-graphics" src="file://ilbUSE7P.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Using the BCD gives Limak the following information:</p><ul> <li> There is one criminal at distance <span class="tex-span">0</span> from the third city&nbsp;— Limak is sure that this criminal is exactly in the third city. </li><li> There is one criminal at distance <span class="tex-span">1</span> from the third city&nbsp;— Limak doesn't know if a criminal is in the second or fourth city. </li><li> There are two criminals at distance <span class="tex-span">2</span> from the third city&nbsp;— Limak is sure that there is one criminal in the first city and one in the fifth city. </li><li> There are zero criminals for every greater distance. </li></ul><p>So, Limak will catch criminals in cities <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">5</span>, that is <span class="tex-span">3</span> criminals in total.</p><p>In the second sample (drawing below), the BCD gives Limak the information that there is one criminal at distance <span class="tex-span">2</span> from Limak's city. There is only one city at distance <span class="tex-span">2</span> so Limak is sure where a criminal is.</p><center> <img class="tex-graphics" src="file://b0qUAMhb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
