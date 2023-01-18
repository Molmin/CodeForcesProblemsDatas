## Description

<div><p>One day Vasya was lying in bed watching his electronic clock to fall asleep quicker.</p><p>Vasya lives in a strange country, where days have <span class="tex-span"><i>h</i></span> hours, and every hour has <span class="tex-span"><i>m</i></span> minutes. Clock shows time in decimal number system, in format <span class="tex-font-style-tt">H:M</span>, where the string <span class="tex-font-style-tt">H</span> always has a fixed length equal to the number of digits in the decimal representation of number <span class="tex-span"><i>h</i> - 1</span>. To achieve this, leading zeros are added if necessary. The string <span class="tex-font-style-tt">M</span> has a similar format, and its length is always equal to the number of digits in the decimal representation of number <span class="tex-span"><i>m</i> - 1</span>. For example, if <span class="tex-span"><i>h</i> = 17</span>, <span class="tex-span"><i>m</i> = 1000</span>, then time equal to 13 hours and 75 minutes will be displayed as "<span class="tex-font-style-tt">13:075</span>".</p><p>Vasya had been watching the clock from <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> hours <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> minutes to <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> hours <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> minutes inclusive, and then he fell asleep. Now he asks you to count how many times he saw the moment at which at least <span class="tex-span"><i>k</i></span> digits changed on the clock simultaneously.</p><p>For example, when switching 04:19 <span class="tex-span"> → </span> 04:20 two digits change. When switching 23:59 <span class="tex-span"> → </span> 00:00, four digits change.</p><p>Consider that Vasya has been watching the clock for strictly less than one day. Note that the last time Vasya saw on the clock before falling asleep was "<span class="tex-font-style-tt">h2:m2</span>". That is, Vasya <span class="tex-font-style-bf">didn't see</span> the moment at which time "<span class="tex-font-style-tt">h2:m2</span>" switched to the next value.</p></div><div class="input-specification"><p>The first line of the input file contains three space-separated integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>h</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>). The second line contains space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">1</sub> &lt; <i>h</i></span>, <span class="tex-span">0 ≤ <i>m</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>). The third line contains space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">2</sub> &lt; <i>h</i></span>, <span class="tex-span">0 ≤ <i>m</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p></div><div class="output-specification"><p>Print a single number — the number of times Vasya saw the moment of changing at least <span class="tex-span"><i>k</i></span> digits simultaneously.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line of the input file contains three space-separated integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>h</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>). The second line contains space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">1</sub> &lt; <i>h</i></span>, <span class="tex-span">0 ≤ <i>m</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>). The third line contains space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">2</sub> &lt; <i>h</i></span>, <span class="tex-span">0 ≤ <i>m</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p>

## Output

<p>Print a single number — the number of times Vasya saw the moment of changing at least <span class="tex-span"><i>k</i></span> digits simultaneously.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
5 5 2
4 4
2 1

```




```input2
24 60 1
0 0
23 59

```




```input3
24 60 3
23 59
23 59

```




```output1
3

```




```output2
1439

```




```output3
0

```



## Note

<p>In the first example Vasya will see the following moments of time: 4:4 <img align="middle" class="tex-formula" src="file://UqnHU1GC.png" style="max-width: 100.0%;max-height: 100.0%;"> 0:0 <span class="tex-span"> → </span> 0:1 <span class="tex-span"> → </span> 0:2 <span class="tex-span"> → </span> 0:3 <span class="tex-span"> → </span> 0:4 <img align="middle" class="tex-formula" src="file://tOdimsX9.png" style="max-width: 100.0%;max-height: 100.0%;"> 1:0 <span class="tex-span"> → </span> 1:1 <span class="tex-span"> → </span> 1:2 <span class="tex-span"> → </span> 1:3 <span class="tex-span"> → </span> 1:4 <img align="middle" class="tex-formula" src="file://NspDCJTU.png" style="max-width: 100.0%;max-height: 100.0%;"> 2:0 <span class="tex-span"> → </span> 2:1 <span class="tex-span"> → </span> 2:2 <span class="tex-span"> → </span> 2:3 <span class="tex-span"> → </span> 2:4. Double arrow (<img align="middle" class="tex-formula" src="file://CtXTUs8k.png" style="max-width: 100.0%;max-height: 100.0%;">) marks the sought moments of time (in this example — when Vasya sees two numbers changing simultaneously).</p><p>In the second example <span class="tex-span"><i>k</i> = 1</span>. Any switching time can be accepted, since during switching of the clock at least one digit is changed. Total switching equals to <span class="tex-span">24·60 = 1440</span>, but Vasya have not seen one of them — the switching of 23:59 <img align="middle" class="tex-formula" src="file://lyY41dd9.png" style="max-width: 100.0%;max-height: 100.0%;"> 00:00.</p><p>In the third example Vasya fell asleep immediately after he began to look at the clock, so he did not see any change.</p>
