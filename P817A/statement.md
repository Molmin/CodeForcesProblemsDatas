## Description

<div><p>Captain Bill the Hummingbird and his crew recieved an interesting challenge offer. Some stranger gave them a map, potion of teleportation and said that only this potion might help them to reach the treasure. </p><p>Bottle with potion has two values <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> written on it. These values define four moves which can be performed using the potion:</p><ul> <li> <img align="middle" class="tex-formula" src="file://fjvL6wj0.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://Tu1nYtcN.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://8YsmKosn.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://STJT4N75.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul><p>Map shows that the position of Captain Bill the Hummingbird is <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and the position of the treasure is <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>You task is to tell Captain Bill the Hummingbird whether he should accept this challenge or decline. If it is possible for Captain to reach the treasure using the potion then output <span class="tex-font-style-tt">"YES"</span>, otherwise <span class="tex-font-style-tt">"NO"</span> (without quotes).</p><p><span class="tex-font-style-bf">The potion can be used infinite amount of times.</span></p></div><div class="input-specification"><p>The first line contains four integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">5</sup></span>) — positions of Captain Bill the Hummingbird and treasure respectively.</p><p>The second line contains two integer numbers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">5</sup></span>) — values on the potion bottle.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">"YES"</span> if it is possible for Captain to reach the treasure using the potion, otherwise print <span class="tex-font-style-tt">"NO"</span> (without quotes).</p></div>

## Input

<p>The first line contains four integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">5</sup></span>) — positions of Captain Bill the Hummingbird and treasure respectively.</p><p>The second line contains two integer numbers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">5</sup></span>) — values on the potion bottle.</p>

## Output

<p>Print <span class="tex-font-style-tt">"YES"</span> if it is possible for Captain to reach the treasure using the potion, otherwise print <span class="tex-font-style-tt">"NO"</span> (without quotes).</p>





```input1
0 0 0 6
2 3

```




```input2
1 1 3 6
1 5

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example there exists such sequence of moves:</p><ol> <li> <img align="middle" class="tex-formula" src="file://Oqkp8El3.png" style="max-width: 100.0%;max-height: 100.0%;"> — the first type of move </li><li> <img align="middle" class="tex-formula" src="file://NPJEF1sa.png" style="max-width: 100.0%;max-height: 100.0%;"> — the third type of move </li></ol>
