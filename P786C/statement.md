## Description

<div><p>Rick and Morty want to find MR. PBH and they can't do it alone. So they need of Mr. Meeseeks. They Have generated <span class="tex-span"><i>n</i></span> Mr. Meeseeks, standing in a line numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each of them has his own color. <span class="tex-span"><i>i</i></span>-th Mr. Meeseeks' color is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Rick and Morty are gathering their army and they want to divide Mr. Meeseeks into some squads. They don't want their squads to be too colorful, so each squad should have Mr. Meeseeks of at most <span class="tex-span"><i>k</i></span> different colors. Also each squad should be a continuous subarray of Mr. Meeseeks in the line. Meaning that for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>e</i> ≤ <i>j</i> ≤ <i>n</i></span>, if Mr. Meeseeks number <span class="tex-span"><i>i</i></span> and Mr. Meeseeks number <span class="tex-span"><i>j</i></span> are in the same squad then Mr. Meeseeks number <span class="tex-span"><i>e</i></span> should be in that same squad.</p><center> <img class="tex-graphics" src="file://T2Qoed4u.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Also, each squad needs its own presidio, and building a presidio needs money, so they want the total number of squads to be minimized.</p><p>Rick and Morty haven't finalized the exact value of <span class="tex-span"><i>k</i></span>, so in order to choose it, for each <span class="tex-span"><i>k</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> (inclusive) need to know the minimum number of presidios needed.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of Mr. Meeseeks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — colors of Mr. Meeseeks in order they standing in a line.</p></div><div class="output-specification"><p>In the first and only line of input print <span class="tex-span"><i>n</i></span> integers separated by spaces. <span class="tex-span"><i>i</i></span>-th integer should be the minimum number of presidios needed if the value of <span class="tex-span"><i>k</i></span> is <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of Mr. Meeseeks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — colors of Mr. Meeseeks in order they standing in a line.</p>

## Output

<p>In the first and only line of input print <span class="tex-span"><i>n</i></span> integers separated by spaces. <span class="tex-span"><i>i</i></span>-th integer should be the minimum number of presidios needed if the value of <span class="tex-span"><i>k</i></span> is <span class="tex-span"><i>i</i></span>.</p>





```input1
5
1 3 4 3 3

```




```input2
8
1 5 7 8 1 7 6 1

```




```output1
4 2 1 1 1 

```




```output2
8 4 3 2 1 1 1 1 

```



## Note

<p>For the first sample testcase, some optimal ways of dividing army into squads for each <span class="tex-span"><i>k</i></span> are:</p><ol> <li> <span class="tex-span">[1], [3], [4], [3, 3]</span> </li><li> <span class="tex-span">[1], [3, 4, 3, 3]</span> </li><li> <span class="tex-span">[1, 3, 4, 3, 3]</span> </li><li> <span class="tex-span">[1, 3, 4, 3, 3]</span> </li><li> <span class="tex-span">[1, 3, 4, 3, 3]</span> </li></ol><p>For the second testcase, some optimal ways of dividing army into squads for each <span class="tex-span"><i>k</i></span> are:</p><ol> <li> <span class="tex-span">[1], [5], [7], [8], [1], [7], [6], [1]</span> </li><li> <span class="tex-span">[1, 5], [7, 8], [1, 7], [6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7], [8], [1, 7, 6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7, 8], [1, 7, 6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7, 8, 1, 7, 6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7, 8, 1, 7, 6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7, 8, 1, 7, 6, 1]</span> </li><li> <span class="tex-span">[1, 5, 7, 8, 1, 7, 6, 1]</span> </li></ol>
