## Description

<div><p>Mary has just graduated from one well-known University and is now attending celebration party. Students like to dream of a beautiful life, so they used champagne glasses to construct a small pyramid. The height of the pyramid is <span class="tex-span"><i>n</i></span>. The top level consists of only <span class="tex-span">1</span> glass, that stands on <span class="tex-span">2</span> glasses on the second level (counting from the top), then <span class="tex-span">3</span> glasses on the third level and so on.The bottom level consists of <span class="tex-span"><i>n</i></span> glasses.</p><p>Vlad has seen in the movies many times how the champagne beautifully flows from top levels to bottom ones, filling all the glasses simultaneously. So he took a bottle and started to pour it in the glass located at the top of the pyramid.</p><p>Each second, Vlad pours to the top glass the amount of champagne equal to the size of exactly one glass. If the glass is already full, but there is some champagne flowing in it, then it pours over the edge of the glass and is equally distributed over two glasses standing under. If the overflowed glass is at the bottom level, then the champagne pours on the table. For the purpose of this problem we consider that champagne is distributed among pyramid glasses immediately. Vlad is interested in the number of completely full glasses if he stops pouring champagne in <span class="tex-span"><i>t</i></span> seconds.</p><p>Pictures below illustrate the pyramid consisting of three levels.</p><center> <img class="tex-graphics" src="file://Y89rwOEQ.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://cvaF8AsK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10, 0 ≤ <i>t</i> ≤ 10 000</span>)&nbsp;— the height of the pyramid and the number of seconds Vlad will be pouring champagne from the bottle.</p></div><div class="output-specification"><p>Print the single integer&nbsp;— the number of completely full glasses after <span class="tex-span"><i>t</i></span> seconds.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10, 0 ≤ <i>t</i> ≤ 10 000</span>)&nbsp;— the height of the pyramid and the number of seconds Vlad will be pouring champagne from the bottle.</p>

## Output

<p>Print the single integer&nbsp;— the number of completely full glasses after <span class="tex-span"><i>t</i></span> seconds.</p>





```input1
3 5

```




```input2
4 8

```




```output1
4

```




```output2
6

```



## Note

<p>In the first sample, the glasses full after <span class="tex-span">5</span> seconds are: the top glass, both glasses on the second level and the middle glass at the bottom level. Left and right glasses of the bottom level will be half-empty.</p>
