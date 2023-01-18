## Description

<div><p>Generous sponsors of the olympiad in which Chloe and Vladik took part allowed all the participants to choose a prize for them on their own. Christmas is coming, so sponsors decided to decorate the Christmas tree with their prizes. </p><p>They took <span class="tex-span"><i>n</i></span> prizes for the contestants and wrote on each of them a unique id (integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>). A gift <span class="tex-span"><i>i</i></span> is characterized by integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— pleasantness of the gift. The pleasantness of the gift can be positive, negative or zero. Sponsors placed the gift <span class="tex-span">1</span> on the top of the tree. All the other gifts hung on a rope tied to some other gift so that each gift hung on the first gift, possibly with a sequence of ropes and another gifts. Formally, the gifts formed a rooted tree with <span class="tex-span"><i>n</i></span> vertices.</p><p>The prize-giving procedure goes in the following way: the participants come to the tree one after another, choose any of the remaining gifts and cut the rope this prize hang on. Note that all the ropes which were used to hang other prizes on the chosen one are not cut. So the contestant gets the chosen gift as well as the all the gifts that hang on it, possibly with a sequence of ropes and another gifts.</p><p>Our friends, Chloe and Vladik, shared the first place on the olympiad and they will choose prizes at the same time! To keep themselves from fighting, they decided to choose two different gifts so that the sets of the gifts that hang on them with a sequence of ropes and another gifts don't intersect. In other words, there shouldn't be any gift that hang both on the gift chosen by Chloe and on the gift chosen by Vladik. From all of the possible variants they will choose such pair of prizes that the sum of pleasantness of all the gifts that they will take after cutting the ropes is as large as possible.</p><p>Print the maximum sum of pleasantness that Vladik and Chloe can get. If it is impossible for them to choose the gifts without fighting, print <span class="tex-font-style-tt">Impossible</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of gifts.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the pleasantness of the gifts.</p><p>The next <span class="tex-span">(<i>n</i> - 1)</span> lines contain two numbers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the description of the tree's edges. It means that gifts with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected to each other with a rope. The gifts' ids in the description of the ropes can be given in arbirtary order: <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> hangs on <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> hangs on <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>It is guaranteed that all the gifts hang on the first gift, possibly with a sequence of ropes and another gifts.</p></div><div class="output-specification"><p>If it is possible for Chloe and Vladik to choose prizes without fighting, print single integer&nbsp;— the maximum possible sum of pleasantness they can get together.</p><p>Otherwise print <span class="tex-font-style-tt">Impossible</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of gifts.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the pleasantness of the gifts.</p><p>The next <span class="tex-span">(<i>n</i> - 1)</span> lines contain two numbers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the description of the tree's edges. It means that gifts with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected to each other with a rope. The gifts' ids in the description of the ropes can be given in arbirtary order: <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> hangs on <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> hangs on <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>It is guaranteed that all the gifts hang on the first gift, possibly with a sequence of ropes and another gifts.</p>

## Output

<p>If it is possible for Chloe and Vladik to choose prizes without fighting, print single integer&nbsp;— the maximum possible sum of pleasantness they can get together.</p><p>Otherwise print <span class="tex-font-style-tt">Impossible</span>.</p>





```input1
8
0 5 -1 4 3 2 6 5
1 2
2 4
2 5
1 3
3 6
6 7
6 8

```




```input2
4
1 -5 1 1
1 2
1 4
2 3

```




```input3
1
-1

```




```output1
25
```




```output2
2
```




```output3
Impossible
```


