## Description

<div><p>Little Artem likes electronics. He can spend lots of time making different schemas and looking for novelties in the nearest electronics store. The new control element was delivered to the store recently and Artem immediately bought it.</p><p>That element can store information about the matrix of integers size <span class="tex-span"><i>n</i> × <i>m</i></span>. There are <span class="tex-span"><i>n</i> + <i>m</i></span> inputs in that element, i.e. each row and each column can get the signal. When signal comes to the input corresponding to some row, this row cyclically shifts to the left, that is the first element of the row becomes last element, second element becomes first and so on. When signal comes to the input corresponding to some column, that column shifts cyclically to the top, that is first element of the column becomes last element, second element becomes first and so on. Rows are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom, while columns are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right.</p><p>Artem wants to carefully study this element before using it. For that purpose he is going to set up an experiment consisting of <span class="tex-span"><i>q</i></span> turns. On each turn he either sends the signal to some input or checks what number is stored at some position of the matrix.</p><p>Artem has completed his experiment and has written down the results, but he has lost the chip! Help Artem find any initial matrix that will match the experiment results. It is guaranteed that experiment data is consistent, which means at least one valid matrix exists.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— dimensions of the matrix and the number of turns in the experiment, respectively.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain turns descriptions, one per line. Each description starts with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) that defines the type of the operation. For the operation of first and second type integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) or <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) follows, while for the operations of the third type three integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given.</p><p>Operation of the first type (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>) means that signal comes to the input corresponding to row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, that is it will shift cyclically. Operation of the second type (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>) means that column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> will shift cyclically. Finally, operation of the third type means that at this moment of time cell located in the row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> stores value <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print the description of any valid initial matrix as <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each. All output integers should not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>If there are multiple valid solutions, output any of them.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— dimensions of the matrix and the number of turns in the experiment, respectively.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain turns descriptions, one per line. Each description starts with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) that defines the type of the operation. For the operation of first and second type integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) or <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) follows, while for the operations of the third type three integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given.</p><p>Operation of the first type (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>) means that signal comes to the input corresponding to row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, that is it will shift cyclically. Operation of the second type (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>) means that column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> will shift cyclically. Finally, operation of the third type means that at this moment of time cell located in the row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> stores value <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print the description of any valid initial matrix as <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each. All output integers should not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>If there are multiple valid solutions, output any of them.</p>





```input1
2 2 6
2 1
2 2
3 1 1 1
3 2 2 2
3 1 2 8
3 2 1 8

```




```input2
3 3 2
1 2
3 2 2 5

```




```output1
8 2 
1 8 

```




```output2
0 0 0 
0 0 5 
0 0 0 

```


