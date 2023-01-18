## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><p>— I... I survived.</p><p>— Welcome home, Chtholly.</p><p>— I kept my promise...</p><p>— I made it... I really made it!</p></span></div></div><p>After several days of fighting, Chtholly Nota Seniorious miraculously returned from the fierce battle.</p><p>As promised, Willem is now baking butter cake for her.</p><p>However, although Willem is skilled in making dessert, he rarely bakes butter cake.</p><p>This time, Willem made a big mistake — he accidentally broke the oven!</p><p>Fortunately, Chtholly decided to help him.</p><p>Willem puts <span class="tex-span"><i>n</i></span> cakes on a roll, cakes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>i</i></span>-th cake needs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> seconds of baking.</p><p>Willem needs Chtholly to do <span class="tex-span"><i>m</i></span> operations to bake the cakes.</p><p>Operation 1: <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span></p><p>Willem asks Chtholly to check each cake in the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, if the cake needs to be baked for more than <span class="tex-span"><i>x</i></span> seconds, he would bake it for <span class="tex-span"><i>x</i></span> seconds and put it back in its place. More precisely, for every <span class="tex-span"><i>i</i></span> in range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is strictly more than <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> becomes equal <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i></span>.</p><p>Operation 2: <span class="tex-span">2 <i>l</i> <i>r</i> <i>x</i></span></p><p>Willem asks Chtholly to count the number of cakes in the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> that needs to be cooked for exactly <span class="tex-span"><i>x</i></span> seconds. More formally you should find number of such <span class="tex-span"><i>i</i></span> in range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>x</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines are the <span class="tex-span"><i>m</i></span> operations described above. It is guaranteed that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each operation of the second type, print the answer.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines are the <span class="tex-span"><i>m</i></span> operations described above. It is guaranteed that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each operation of the second type, print the answer.</p>





```input1
5 6
1 5 5 5 8
2 2 5 5
1 2 4 3
2 2 5 2
2 2 5 5
1 3 5 1
2 1 5 1

```




```input2
7 7
1 9 2 6 8 1 7
2 1 7 1
2 2 5 2
1 4 7 7
2 2 4 2
1 3 4 5
2 3 3 3
2 3 7 2

```




```input3
8 13
75 85 88 100 105 120 122 128
1 1 8 70
2 3 8 30
1 3 8 3
2 2 5 15
1 2 4 10
2 1 5 5
1 2 7 27
2 1 5 5
1 3 7 12
1 1 7 4
2 1 8 1
1 4 8 5
2 1 8 1

```




```output1
3
3
0
3

```




```output2
2
1
1
0
1

```




```output3
1
2
3
4
5
6

```


