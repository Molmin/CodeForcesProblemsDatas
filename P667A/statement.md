## Description

<div><p>A lot of people in Berland hates rain, but you do not. Rain pacifies, puts your thoughts in order. By these years you have developed a good tradition — when it rains, you go on the street and stay silent for a moment, contemplate all around you, enjoy freshness, think about big deeds you have to do. </p><p>Today everything had changed quietly. You went on the street with a cup contained water, your favorite drink. In a moment when you were drinking a water you noticed that the process became quite long: the cup still contained water because of rain. You decided to make a formal model of what was happening and to find if it was possible to drink all water in that situation. </p><p>Thus, your cup is a cylinder with diameter equals <span class="tex-span"><i>d</i></span> centimeters. Initial level of water in cup equals <span class="tex-span"><i>h</i></span> centimeters from the bottom. </p><center> <img class="tex-graphics" src="file://ulNEwKyF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You drink a water with a speed equals <span class="tex-span"><i>v</i></span> milliliters per second. But rain goes with such speed that if you do not drink a water from the cup, the level of water increases on <span class="tex-span"><i>e</i></span> centimeters per second. The process of drinking water from the cup and the addition of rain to the cup goes evenly and continuously. </p><p>Find the time needed to make the cup empty or find that it will never happen. It is guaranteed that if it is possible to drink all water, it will happen not later than after <span class="tex-span">10<sup class="upper-index">4</sup></span> seconds.</p><p>Note one milliliter equals to one cubic centimeter.</p></div><div class="input-specification"><p>The only line of the input contains four integer numbers <span class="tex-span"><i>d</i>, <i>h</i>, <i>v</i>, <i>e</i></span> (<span class="tex-span">1 ≤ <i>d</i>, <i>h</i>, <i>v</i>, <i>e</i> ≤ 10<sup class="upper-index">4</sup></span>), where:</p><ul> <li> <span class="tex-span"><i>d</i></span> — the diameter of your cylindrical cup, </li><li> <span class="tex-span"><i>h</i></span> — the initial level of water in the cup, </li><li> <span class="tex-span"><i>v</i></span> — the speed of drinking process from the cup in milliliters per second, </li><li> <span class="tex-span"><i>e</i></span> — the growth of water because of rain if you do not drink from the cup. </li></ul></div><div class="output-specification"><p>If it is impossible to make the cup empty, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print a real number — time in seconds needed the cup will be empty. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>. It is guaranteed that if the answer exists, it doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div>

## Input

<p>The only line of the input contains four integer numbers <span class="tex-span"><i>d</i>, <i>h</i>, <i>v</i>, <i>e</i></span> (<span class="tex-span">1 ≤ <i>d</i>, <i>h</i>, <i>v</i>, <i>e</i> ≤ 10<sup class="upper-index">4</sup></span>), where:</p><ul> <li> <span class="tex-span"><i>d</i></span> — the diameter of your cylindrical cup, </li><li> <span class="tex-span"><i>h</i></span> — the initial level of water in the cup, </li><li> <span class="tex-span"><i>v</i></span> — the speed of drinking process from the cup in milliliters per second, </li><li> <span class="tex-span"><i>e</i></span> — the growth of water because of rain if you do not drink from the cup. </li></ul>

## Output

<p>If it is impossible to make the cup empty, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print a real number — time in seconds needed the cup will be empty. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>. It is guaranteed that if the answer exists, it doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>





```input1
1 2 3 100

```




```input2
1 1 1 1

```




```output1
NO

```




```output2
YES
3.659792366325

```



## Note

<p>In the first example the water fills the cup faster than you can drink from it.</p><p>In the second example area of the cup's bottom equals to <img align="middle" class="tex-formula" src="file://1Wj6nu9z.png" style="max-width: 100.0%;max-height: 100.0%;">, thus we can conclude that you decrease the level of water by <img align="middle" class="tex-formula" src="file://0KlkM86z.png" style="max-width: 100.0%;max-height: 100.0%;"> centimeters per second. At the same time water level increases by <span class="tex-span">1</span> centimeter per second due to rain. Thus, cup will be empty in <img align="middle" class="tex-formula" src="file://AxneN8L4.png" style="max-width: 100.0%;max-height: 100.0%;"> seconds.</p>
