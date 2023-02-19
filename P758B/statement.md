## Description

<div><p>Nothing is eternal in the world, Kostya understood it on the 7-th of January when he saw partially dead four-color garland.</p><p>Now he has a goal to replace dead light bulbs, however he doesn't know how many light bulbs for each color are required. It is guaranteed that for each of four colors at least one light is working.</p><p>It is known that the garland contains light bulbs of four colors: red, blue, yellow and green. The garland is made as follows: if you take any four consecutive light bulbs then there will not be light bulbs with the same color among them. For example, the garland can look like "<span class="tex-font-style-tt">RYBGRYBGRY</span>", "<span class="tex-font-style-tt">YBGRYBGRYBG</span>", "<span class="tex-font-style-tt">BGRYB</span>", but can not look like "<span class="tex-font-style-tt">BGRYG</span>", "<span class="tex-font-style-tt">YBGRYBYGR</span>" or "<span class="tex-font-style-tt">BGYBGY</span>". Letters denote colors: '<span class="tex-font-style-tt">R</span>'&nbsp;— red, '<span class="tex-font-style-tt">B</span>'&nbsp;— blue, '<span class="tex-font-style-tt">Y</span>'&nbsp;— yellow, '<span class="tex-font-style-tt">G</span>'&nbsp;— green.</p><p>Using the information that for each color at least one light bulb still works count the number of dead light bulbs of each four colors.</p></div><div class="input-specification"><p>The first and the only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">4 ≤ |<i>s</i>| ≤ 100</span>), which describes the garland, the <span class="tex-span"><i>i</i></span>-th symbol of which describes the color of the <span class="tex-span"><i>i</i></span>-th light bulb in the order from the beginning of garland: </p><ul> <li> '<span class="tex-font-style-tt">R</span>'&nbsp;— the light bulb is red, </li><li> '<span class="tex-font-style-tt">B</span>'&nbsp;— the light bulb is blue, </li><li> '<span class="tex-font-style-tt">Y</span>'&nbsp;— the light bulb is yellow, </li><li> '<span class="tex-font-style-tt">G</span>'&nbsp;— the light bulb is green, </li><li> '<span class="tex-font-style-tt">!</span>'&nbsp;— the light bulb is dead. </li></ul><p>The string <span class="tex-span"><i>s</i></span> can not contain other symbols except those five which were described. </p><p>It is guaranteed that in the given string at least once there is each of four letters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">Y</span>' and '<span class="tex-font-style-tt">G</span>'. </p><p>It is guaranteed that the string <span class="tex-span"><i>s</i></span> is correct garland with some blown light bulbs, it means that for example the line "<span class="tex-font-style-tt">GRBY!!!B</span>" can not be in the input data. </p></div><div class="output-specification"><p>In the only line print four integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>r</i></sub>, <i>k</i><sub class="lower-index"><i>b</i></sub>, <i>k</i><sub class="lower-index"><i>y</i></sub>, <i>k</i><sub class="lower-index"><i>g</i></sub></span>&nbsp;— the number of dead light bulbs of red, blue, yellow and green colors accordingly.</p></div>

## Input

<p>The first and the only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">4 ≤ |<i>s</i>| ≤ 100</span>), which describes the garland, the <span class="tex-span"><i>i</i></span>-th symbol of which describes the color of the <span class="tex-span"><i>i</i></span>-th light bulb in the order from the beginning of garland: </p><ul> <li> '<span class="tex-font-style-tt">R</span>'&nbsp;— the light bulb is red, </li><li> '<span class="tex-font-style-tt">B</span>'&nbsp;— the light bulb is blue, </li><li> '<span class="tex-font-style-tt">Y</span>'&nbsp;— the light bulb is yellow, </li><li> '<span class="tex-font-style-tt">G</span>'&nbsp;— the light bulb is green, </li><li> '<span class="tex-font-style-tt">!</span>'&nbsp;— the light bulb is dead. </li></ul><p>The string <span class="tex-span"><i>s</i></span> can not contain other symbols except those five which were described. </p><p>It is guaranteed that in the given string at least once there is each of four letters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">Y</span>' and '<span class="tex-font-style-tt">G</span>'. </p><p>It is guaranteed that the string <span class="tex-span"><i>s</i></span> is correct garland with some blown light bulbs, it means that for example the line "<span class="tex-font-style-tt">GRBY!!!B</span>" can not be in the input data. </p>

## Output

<p>In the only line print four integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>r</i></sub>, <i>k</i><sub class="lower-index"><i>b</i></sub>, <i>k</i><sub class="lower-index"><i>y</i></sub>, <i>k</i><sub class="lower-index"><i>g</i></sub></span>&nbsp;— the number of dead light bulbs of red, blue, yellow and green colors accordingly.</p>





```input1
RYBGRYBGR

```




```input2
!RGYB

```




```input3
!!!!YGRB

```




```input4
!GB!RG!Y!

```




```output1
0 0 0 0
```




```output2
0 1 0 0
```




```output3
1 1 1 1
```




```output4
2 1 1 0
```



## Note

<p>In the first example there are no dead light bulbs.</p><p>In the second example it is obvious that one blue bulb is blown, because it could not be light bulbs of other colors on its place according to the statements.</p>
