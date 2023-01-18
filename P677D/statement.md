## Description

<div><p>Vanya is in the palace that can be represented as a grid <span class="tex-span"><i>n</i> × <i>m</i></span>. Each room contains a single chest, an the room located in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th columns contains the chest of type <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>. Each chest of type <span class="tex-span"><i>x</i> ≤ <i>p</i> - 1</span> contains a key that can open any chest of type <span class="tex-span"><i>x</i> + 1</span>, and all chests of type <span class="tex-span">1</span> are not locked. There is exactly one chest of type <span class="tex-span"><i>p</i></span> and it contains a treasure.</p><p>Vanya starts in cell <span class="tex-span">(1, 1)</span> (top left corner). What is the minimum total distance Vanya has to walk in order to get the treasure? Consider the distance between cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> (the cell in the row <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>) and <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> is equal to <span class="tex-span">|<i>r</i><sub class="lower-index">1</sub> - <i>r</i><sub class="lower-index">2</sub>| + |<i>c</i><sub class="lower-index">1</sub> - <i>c</i><sub class="lower-index">2</sub>|</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300, 1 ≤ <i>p</i> ≤ <i>n</i>·<i>m</i></span>)&nbsp;— the number of rows and columns in the table representing the palace and the number of different types of the chests, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>p</i></span>)&nbsp;— the types of the chests in corresponding rooms. It's guaranteed that for each <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>p</i></span> there is at least one chest of this type (that is, there exists a pair of <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>rc</i></sub> = <i>x</i></span>). Also, it's guaranteed that there is exactly one chest of type <span class="tex-span"><i>p</i></span>.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum possible total distance Vanya has to walk in order to get the treasure from the chest of type <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300, 1 ≤ <i>p</i> ≤ <i>n</i>·<i>m</i></span>)&nbsp;— the number of rows and columns in the table representing the palace and the number of different types of the chests, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>p</i></span>)&nbsp;— the types of the chests in corresponding rooms. It's guaranteed that for each <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>p</i></span> there is at least one chest of this type (that is, there exists a pair of <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>rc</i></sub> = <i>x</i></span>). Also, it's guaranteed that there is exactly one chest of type <span class="tex-span"><i>p</i></span>.</p>

## Output

<p>Print one integer&nbsp;— the minimum possible total distance Vanya has to walk in order to get the treasure from the chest of type <span class="tex-span"><i>p</i></span>.</p>





```input1
3 4 3
2 1 1 1
1 1 1 1
2 1 1 3

```




```input2
3 3 9
1 3 5
8 9 7
4 6 2

```




```input3
3 4 12
1 2 3 4
8 7 6 5
9 10 11 12

```




```output1
5

```




```output2
22

```




```output3
11

```


