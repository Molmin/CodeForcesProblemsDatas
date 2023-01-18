## Description

<div><p>Vika has <span class="tex-span"><i>n</i></span> jars with paints of distinct colors. All the jars are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the <span class="tex-span"><i>i</i></span>-th jar contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> liters of paint of color <span class="tex-span"><i>i</i></span>.</p><p>Vika also has an infinitely long rectangular piece of paper of width <span class="tex-span">1</span>, consisting of squares of size <span class="tex-span">1 × 1</span>. Squares are numbered <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and so on. Vika decided that she will start painting squares one by one from left to right, starting from the square number <span class="tex-span">1</span> and some arbitrary color. If the square was painted in color <span class="tex-span"><i>x</i></span>, then the next square will be painted in color <span class="tex-span"><i>x</i> + 1</span>. In case of <span class="tex-span"><i>x</i> = <i>n</i></span>, next square is painted in color <span class="tex-span">1</span>. If there is no more paint of the color Vika wants to use now, then she stops.</p><p>Square is always painted in only one color, and it takes exactly <span class="tex-span">1</span> liter of paint. Your task is to calculate the maximum number of squares that might be painted, if Vika chooses right color to paint the first square.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of jars with colors Vika has.</p><p>The second line of the input contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of liters of paint in the <span class="tex-span"><i>i</i></span>-th jar, i.e. the number of liters of color <span class="tex-span"><i>i</i></span> that Vika has.</p></div><div class="output-specification"><p>The only line of the output should contain a single integer&nbsp;— the maximum number of squares that Vika can paint if she follows the rules described above.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of jars with colors Vika has.</p><p>The second line of the input contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of liters of paint in the <span class="tex-span"><i>i</i></span>-th jar, i.e. the number of liters of color <span class="tex-span"><i>i</i></span> that Vika has.</p>

## Output

<p>The only line of the output should contain a single integer&nbsp;— the maximum number of squares that Vika can paint if she follows the rules described above.</p>





```input1
5
2 4 2 3 3

```




```input2
3
5 5 5

```




```input3
6
10 10 10 1 10 10

```




```output1
12

```




```output2
15

```




```output3
11

```



## Note

<p>In the first sample the best strategy is to start painting using color <span class="tex-span">4</span>. Then the squares will be painted in the following colors (from left to right): 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5.</p><p>In the second sample Vika can start to paint using any color.</p><p>In the third sample Vika should start painting using color number <span class="tex-span">5</span>.</p>
