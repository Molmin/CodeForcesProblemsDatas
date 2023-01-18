## Description

<div><p>Valera has <span class="tex-span">2·<i>n</i></span> cubes, each cube contains an integer from <span class="tex-span">10</span> to <span class="tex-span">99</span>. He arbitrarily chooses <span class="tex-span"><i>n</i></span> cubes and puts them in the first heap. The remaining cubes form the second heap. </p><p>Valera decided to play with cubes. During the game he takes a cube from the first heap and writes down the number it has. Then he takes a cube from the second heap and write out its two digits near two digits he had written (to the right of them). In the end he obtained a single fourdigit integer — the first two digits of it is written on the cube from the first heap, and the second two digits of it is written on the second cube from the second heap.</p><p>Valera knows arithmetic very well. So, he can easily count the number of distinct fourdigit numbers he can get in the game. The other question is: how to split cubes into two heaps so that this number (the number of distinct fourdigit integers Valera can get) will be as large as possible?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span">2·<i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(10 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 99)</span>, denoting the numbers on the cubes.</p></div><div class="output-specification"><p>In the first line print a single number — the maximum possible number of distinct four-digit numbers Valera can obtain. In the second line print <span class="tex-span">2·<i>n</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. The numbers mean: the <span class="tex-span"><i>i</i></span>-th cube belongs to the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th heap in your division.</p><p>If there are multiple optimal ways to split the cubes into the heaps, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span">2·<i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(10 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 99)</span>, denoting the numbers on the cubes.</p>

## Output

<p>In the first line print a single number — the maximum possible number of distinct four-digit numbers Valera can obtain. In the second line print <span class="tex-span">2·<i>n</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. The numbers mean: the <span class="tex-span"><i>i</i></span>-th cube belongs to the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th heap in your division.</p><p>If there are multiple optimal ways to split the cubes into the heaps, print any of them.</p>





```input1
1
10 99

```




```input2
2
13 24 13 45

```




```output1
1
2 1 

```




```output2
4
1 2 2 1 

```



## Note

<p>In the first test case Valera can put the first cube in the first heap, and second cube — in second heap. In this case he obtain number <span class="tex-span">1099</span>. If he put the second cube in the first heap, and the first cube in the second heap, then he can obtain number <span class="tex-span">9910</span>. In both cases the maximum number of distinct integers is equal to one.</p><p>In the second test case Valera can obtain numbers <span class="tex-span">1313, 1345, 2413, 2445</span>. Note, that if he put the first and the third cubes in the first heap, he can obtain only two numbers <span class="tex-span">1324</span> and <span class="tex-span">1345</span>.</p>
