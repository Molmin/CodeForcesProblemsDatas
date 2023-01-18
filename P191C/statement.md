## Description

<div><p>They say that Berland has exactly two problems, fools and roads. Besides, Berland has <span class="tex-span"><i>n</i></span> cities, populated by the fools and connected by the roads. All Berland roads are bidirectional. As there are many fools in Berland, between each pair of cities there is a path (or else the fools would get upset). Also, between each pair of cities there is no more than one simple path (or else the fools would get lost). </p><p>But that is not the end of Berland's special features. In this country fools sometimes visit each other and thus spoil the roads. The fools aren't very smart, so they always use only the simple paths.</p><p><span class="tex-font-style-it">A simple path</span> is the path which goes through every Berland city not more than once.</p><p>The Berland government knows the paths which the fools use. Help the government count for each road, how many distinct fools can go on it.</p><p>Note how the fools' paths are given in the input.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities. </p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), that means that there is a road connecting cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of fools who visit each other. </p><p>Next <span class="tex-span"><i>k</i></span> lines contain two space-separated numbers. The <span class="tex-span"><i>i</i></span>-th line <span class="tex-span">(<i>i</i> &gt; 0)</span> contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). That means that the fool number <span class="tex-span">2<i>i</i> - 1</span> lives in city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and visits the fool number <span class="tex-span">2<i>i</i></span>, who lives in city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. The given pairs describe simple paths, because between every pair of cities there is only one simple path.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> - 1</span> integer. The integers should be separated by spaces. The <span class="tex-span"><i>i</i></span>-th number should equal the number of fools who can go on the <span class="tex-span"><i>i</i></span>-th road. The roads are numbered starting from one in the order, in which they occur in the input.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities. </p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), that means that there is a road connecting cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of fools who visit each other. </p><p>Next <span class="tex-span"><i>k</i></span> lines contain two space-separated numbers. The <span class="tex-span"><i>i</i></span>-th line <span class="tex-span">(<i>i</i> &gt; 0)</span> contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). That means that the fool number <span class="tex-span">2<i>i</i> - 1</span> lives in city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and visits the fool number <span class="tex-span">2<i>i</i></span>, who lives in city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. The given pairs describe simple paths, because between every pair of cities there is only one simple path.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> - 1</span> integer. The integers should be separated by spaces. The <span class="tex-span"><i>i</i></span>-th number should equal the number of fools who can go on the <span class="tex-span"><i>i</i></span>-th road. The roads are numbered starting from one in the order, in which they occur in the input.</p>





```input1
5
1 2
1 3
2 4
2 5
2
1 4
3 5

```




```input2
5
3 4
4 5
1 4
2 4
3
2 3
1 3
3 5

```




```output1
2 1 1 1 

```




```output2
3 1 1 1 

```



## Note

<p>In the first sample the fool number one goes on the first and third road and the fool number 3 goes on the second, first and fourth ones.</p><p>In the second sample, the fools number 1, 3 and 5 go on the first road, the fool number 5 will go on the second road, on the third road goes the fool number 3, and on the fourth one goes fool number 1.</p>
