## Description

<div><p>In the evenings Donkey would join Shrek to look at the stars. They would sit on a log, sipping tea and they would watch the starry sky. The sky hung above the roof, right behind the chimney. Shrek's stars were to the right of the chimney and the Donkey's stars were to the left. Most days the Donkey would just count the stars, so he knew that they are exactly <span class="tex-span"><i>n</i></span>. This time he wanted a challenge. He imagined a coordinate system: he put the origin of the coordinates at the intersection of the roof and the chimney, directed the <span class="tex-span"><i>OX</i></span> axis to the left along the roof and the <span class="tex-span"><i>OY</i></span> axis — up along the chimney (see figure). The Donkey imagined two rays emanating from he origin of axes at angles <span class="tex-span">α<sub class="lower-index">1</sub></span> and <span class="tex-span">α<sub class="lower-index">2</sub></span> to the <span class="tex-span"><i>OX</i></span> axis.</p><center> <img class="tex-graphics" src="file://yBvmj4fP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now he chooses any star that lies strictly between these rays. After that he imagines more rays that emanate from this star at the same angles <span class="tex-span">α<sub class="lower-index">1</sub></span> and <span class="tex-span">α<sub class="lower-index">2</sub></span> to the <span class="tex-span"><i>OX</i></span> axis and chooses another star that lies strictly between the new rays. He repeats the operation as long as there still are stars he can choose between the rays that emanate from a star. </p><center> <img class="tex-graphics" src="file://tup9YjaV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As a result, the Donkey gets a chain of stars. He can consecutively get to each star if he acts by the given rules.</p><p>Your task is to find the maximum number of stars <span class="tex-span"><i>m</i></span> that the Donkey's chain can contain.</p><p>Note that the chain must necessarily start in the point of the origin of the axes, that isn't taken into consideration while counting the number <span class="tex-span"><i>m</i></span> of stars in the chain.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of stars. The second line contains simple fractions representing relationships "<span class="tex-span"><i>a</i></span>/<span class="tex-span"><i>b</i></span> <span class="tex-span"><i>c</i></span>/<span class="tex-span"><i>d</i></span>", such that <img align="middle" class="tex-formula" src="file://3Zu0GpoC.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://wItGTwAs.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup></span>; <img align="middle" class="tex-formula" src="file://yOQkmnUK.png" style="max-width: 100.0%;max-height: 100.0%;">; <img align="middle" class="tex-formula" src="file://sjDaFoMk.png" style="max-width: 100.0%;max-height: 100.0%;">; <img align="middle" class="tex-formula" src="file://7kDg9D6Z.png" style="max-width: 100.0%;max-height: 100.0%;">). The given numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> are integers.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)— the stars' coordinates.</p><p>It is guaranteed that all stars have distinct coordinates.</p></div><div class="output-specification"><p>In a single line print number <span class="tex-span"><i>m</i></span> — the answer to the problem.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of stars. The second line contains simple fractions representing relationships "<span class="tex-span"><i>a</i></span>/<span class="tex-span"><i>b</i></span> <span class="tex-span"><i>c</i></span>/<span class="tex-span"><i>d</i></span>", such that <img align="middle" class="tex-formula" src="file://3Zu0GpoC.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://wItGTwAs.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup></span>; <img align="middle" class="tex-formula" src="file://yOQkmnUK.png" style="max-width: 100.0%;max-height: 100.0%;">; <img align="middle" class="tex-formula" src="file://sjDaFoMk.png" style="max-width: 100.0%;max-height: 100.0%;">; <img align="middle" class="tex-formula" src="file://7kDg9D6Z.png" style="max-width: 100.0%;max-height: 100.0%;">). The given numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> are integers.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)— the stars' coordinates.</p><p>It is guaranteed that all stars have distinct coordinates.</p>

## Output

<p>In a single line print number <span class="tex-span"><i>m</i></span> — the answer to the problem.</p>





```input1
15
1/3 2/1
3 1
6 2
4 2
2 5
4 5
6 6
3 4
1 6
2 1
7 4
9 3
5 3
1 3
15 5
12 4

```




```output1
4

```



## Note

<p>In the sample the longest chain the Donkey can build consists of four stars. Note that the Donkey can't choose the stars that lie on the rays he imagines.</p><center> <img class="tex-graphics" src="file://u0Kslzlz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
