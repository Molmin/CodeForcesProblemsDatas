## Description

<div><p>As we all know Barney's job is "PLEASE" and he has not much to do at work. That's why he started playing "cups and key". In this game there are three identical cups arranged in a line from left to right. Initially key to Barney's heart is under the middle cup.</p><center> <img class="tex-graphics" src="file://7Qo7LUcd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Then at one turn Barney swaps the cup in the middle with any of other two cups randomly (he choses each with equal probability), so the chosen cup becomes the middle one. Game lasts <span class="tex-span"><i>n</i></span> turns and Barney <span class="tex-font-style-bf">independently choses</span> a cup to swap with the middle one within each turn, and the key always remains in the cup it was at the start.</p><p>After <span class="tex-span"><i>n</i></span>-th turn Barney asks a girl to guess which cup contains the key. The girl points to the middle one but Barney was distracted while making turns and doesn't know if the key is under the middle cup. That's why he asked you to tell him the probability that girl guessed right.</p><p>Number <span class="tex-span"><i>n</i></span> of game turns can be extremely large, that's why Barney did not give it to you. Instead he gave you an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> such that </p><center> <img align="middle" class="tex-formula" src="file://O6y92wB0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>in other words, <span class="tex-span"><i>n</i></span> is multiplication of all elements of the given array.</p><p>Because of precision difficulties, Barney asked you to tell him the answer as an irreducible fraction. In other words you need to find it as a fraction <span class="tex-span"><i>p</i> / <i>q</i></span> such that <img align="middle" class="tex-formula" src="file://Kk1Fieh1.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://snncCdhG.png" style="max-width: 100.0%;max-height: 100.0%;"> is the greatest common divisor. Since <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> can be extremely large, you only need to find the remainders of dividing each of them by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Please note that we want <img align="middle" class="tex-formula" src="file://5Q1HfwvY.png" style="max-width: 100.0%;max-height: 100.0%;"> of <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> to be <span class="tex-span">1</span>, <span class="tex-font-style-bf">not <img align="middle" class="tex-formula" src="file://6sCY5gwO.png" style="max-width: 100.0%;max-height: 100.0%;"> of their remainders</span> after dividing by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in array Barney gave you.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>In the only line of output print a single string <span class="tex-span"><i>x</i> / <i>y</i></span> where <span class="tex-span"><i>x</i></span> is the remainder of dividing <span class="tex-span"><i>p</i></span> by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> and <span class="tex-span"><i>y</i></span> is the remainder of dividing <span class="tex-span"><i>q</i></span> by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in array Barney gave you.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>In the only line of output print a single string <span class="tex-span"><i>x</i> / <i>y</i></span> where <span class="tex-span"><i>x</i></span> is the remainder of dividing <span class="tex-span"><i>p</i></span> by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> and <span class="tex-span"><i>y</i></span> is the remainder of dividing <span class="tex-span"><i>q</i></span> by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1
2

```




```input2
3
1 1 1

```




```output1
1/2

```




```output2
0/1

```


