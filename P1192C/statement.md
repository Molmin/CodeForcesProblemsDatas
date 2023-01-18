## Description

<div><p>A <span class="tex-font-style-bf">cubeword</span> is a special type of a crossword. When building a cubeword, you start by choosing a positive integer $a$: the side length of the cube. Then, you build a big cube consisting of $a \times a \times a$ unit cubes. This big cube has 12 edges. Then, you discard all unit cubes that do not touch the edges of the big cube. The figure below shows the object you will get for $a=6$.</p><center> <img class="tex-graphics" height="113px" src="file://JbwU8NGY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Finally, you assign a letter to each of the unit cubes in the object. You must get a meaningful word along each edge of the big cube. Each edge can be read in either direction, and it is sufficient if one of the two directions of reading gives a meaningful word.</p><p>The figure below shows the object for $a=6$ in which some unit cubes already have assigned letters. You can already read the words '<span class="tex-font-style-tt">SUBMIT</span>', '<span class="tex-font-style-tt">ACCEPT</span>' and '<span class="tex-font-style-tt">TURING</span>' along three edges of the big cube.</p><center> <img class="tex-graphics" height="265px" src="file://UfzWhTsZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a list of valid words. Each word from the wordlist may appear on arbitrarily many edges of a valid cubeword. Find and report the number of different cubewords that can be constructed, modulo $998,244,353$.</p><p>If one cubeword can be obtained from another by rotation or mirroring, they are considered <span class="tex-font-style-bf">distinct</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 100,000$) – the number of words.</p><p>Then, $n$ lines follow. Each of these lines contains one word that can appear on the edges of the big cube. The length of each word is between 3 and 10, inclusive.</p><p>It is guaranteed that all words are different.</p></div><div class="output-specification"><p>Output a single integer, the number of distinct cubewords for the given list of valid words modulo $998,244,353$.</p></div><div><h2>Scoring</h2><p>Subtask 1 (21 points): the words consist only of letters '<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">f</span>' (lowercase)</p><p>Subtask 2 (29 points): the words consist only of letters '<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">p</span>' (lowercase)</p><p>Subtask 3 (34 points): the words consist of letters '<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">p</span>' (lowercase) and '<span class="tex-font-style-tt">A</span>' - '<span class="tex-font-style-tt">P</span>' (uppercase)</p><p>Subtask 4 (16 points): the words consist of letters '<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">z</span>' (lowercase), '<span class="tex-font-style-tt">A</span>' - '<span class="tex-font-style-tt">Z</span>' (uppercase) and digits '<span class="tex-font-style-tt">0</span>' - '<span class="tex-font-style-tt">9</span>'</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 100,000$) – the number of words.</p><p>Then, $n$ lines follow. Each of these lines contains one word that can appear on the edges of the big cube. The length of each word is between 3 and 10, inclusive.</p><p>It is guaranteed that all words are different.</p>

## Output

<p>Output a single integer, the number of distinct cubewords for the given list of valid words modulo $998,244,353$.</p>





```input1
1
radar
```




```input2
1
robot
```




```input3
2
FLOW
WOLF
```




```input4
2
baobab
bob
```




```input5
3
TURING
SUBMIT
ACCEPT
```




```input6
3
MAN1LA
MAN6OS
AN4NAS
```




```output1
1
```




```output2
2
```




```output3
2
```




```output4
4097
```




```output5
162
```




```output6
114
```



## Note

<p>In the first sample, the only possibility is for the word "<span class="tex-font-style-tt">radar</span>" to be on each edge of the cube.</p><p>In the second sample, there are two cubes, which are just rotations of each other – the word "<span class="tex-font-style-tt">robot</span>" is on every edge, and the difference between the two cubes is whether the lower left front corner contains '<span class="tex-font-style-tt">r</span>' or '<span class="tex-font-style-tt">t</span>'.</p><p>The third sample is similar to the second one. The fact that we can read the word on each edge in both directions does not affect the answer.</p><p>In the fourth sample, there is one cube with the word "<span class="tex-font-style-tt">bob</span>" on each edge. There are also $2^{12} = 4096$ cubes with the word "<span class="tex-font-style-tt">baobab</span>" on each edge. (For each of the 12 edges, we have two possible directions in which the word "<span class="tex-font-style-tt">baobab</span>" can appear.)</p>
