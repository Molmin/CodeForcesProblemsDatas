## Description

<div><p>A one-dimensional Japanese crossword can be represented as a binary string of length <span class="tex-span"><i>x</i></span>. An encoding of this crossword is an array <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span>, where <span class="tex-span"><i>n</i></span> is the number of segments formed completely of <span class="tex-span">1</span>'s, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the length of <span class="tex-span"><i>i</i></span>-th segment. No two segments touch or intersect.</p><p>For example: </p><ul> <li> If <span class="tex-span"><i>x</i> = 6</span> and the crossword is <span class="tex-span">111011</span>, then its encoding is an array <span class="tex-span">{3, 2}</span>; </li><li> If <span class="tex-span"><i>x</i> = 8</span> and the crossword is <span class="tex-span">01101010</span>, then its encoding is an array <span class="tex-span">{2, 1, 1}</span>; </li><li> If <span class="tex-span"><i>x</i> = 5</span> and the crossword is <span class="tex-span">11111</span>, then its encoding is an array <span class="tex-span">{5}</span>; </li><li> If <span class="tex-span"><i>x</i> = 5</span> and the crossword is <span class="tex-span">00000</span>, then its encoding is an empty array. </li></ul><p>Mishka wants to create a new one-dimensional Japanese crossword. He has already picked the length and the encoding for this crossword. And now he needs to check if there is <span class="tex-font-style-bf">exactly one</span> crossword such that its length and encoding are equal to the length and encoding he picked. Help him to check it!</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the encoding and the length of the crossword Mishka picked.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) — the encoding.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> if there exists <span class="tex-font-style-bf">exaclty one</span> crossword with chosen length and encoding. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the encoding and the length of the crossword Mishka picked.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) — the encoding.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> if there exists <span class="tex-font-style-bf">exaclty one</span> crossword with chosen length and encoding. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
2 4
1 3

```




```input2
3 10
3 3 2

```




```input3
2 10
1 3

```




```output1
NO

```




```output2
YES

```




```output3
NO

```


