## Description

<div><p>Limak is a little polar bear. His parents told him to clean a house before the New Year's Eve. Their house is a rectangular grid with <span class="tex-span"><i>h</i></span> rows and <span class="tex-span"><i>w</i></span> columns. Each cell is an empty square.</p><p>He is a little bear and thus he can't clean a house by himself. Instead, he is going to use a cleaning robot.</p><p>A cleaning robot has a built-in pattern of <span class="tex-span"><i>n</i></span> moves, defined by a string of the length <span class="tex-span"><i>n</i></span>. A single move (character) moves a robot to one of four adjacent cells. Each character is one of the following four: '<span class="tex-font-style-tt">U</span>' (up), '<span class="tex-font-style-tt">D</span>' (down), '<span class="tex-font-style-tt">L</span>' (left), '<span class="tex-font-style-tt">R</span>' (right). One move takes one minute.</p><p>A cleaning robot must be placed and started in some cell. Then it repeats its pattern of moves till it hits a wall (one of four borders of a house). After hitting a wall it can be placed and used again.</p><p>Limak isn't sure if placing a cleaning robot in one cell will be enough. Thus, he is going to start it <span class="tex-span"><i>w</i>·<i>h</i></span> times, one time in each cell. Maybe some cells will be cleaned more than once but who cares?</p><p>Limak asks you one question. How much time will it take to clean a house? Find and print the number of minutes modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. It's also possible that a cleaning robot will never stop&nbsp;— then print "<span class="tex-font-style-tt">-1</span>" (without the quotes) instead.</p><p>Placing and starting a robot takes no time, however, you must count a move when robot hits a wall. Take a look into samples for further clarification.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>h</i>, <i>w</i> ≤ 500 000</span>)&nbsp;— the length of the pattern, the number of rows and the number of columns, respectively.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>&nbsp;— the pattern of <span class="tex-span"><i>n</i></span> moves. Each character is one of uppercase letters '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>' or '<span class="tex-font-style-tt">R</span>'.</p></div><div class="output-specification"><p>Print one line with the answer.</p><p>If a cleaning robot will never stop, print "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print the number of minutes it will take to clean a house modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>h</i>, <i>w</i> ≤ 500 000</span>)&nbsp;— the length of the pattern, the number of rows and the number of columns, respectively.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>&nbsp;— the pattern of <span class="tex-span"><i>n</i></span> moves. Each character is one of uppercase letters '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>' or '<span class="tex-font-style-tt">R</span>'.</p>

## Output

<p>Print one line with the answer.</p><p>If a cleaning robot will never stop, print "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print the number of minutes it will take to clean a house modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1 10 2
R

```




```input2
3 4 6
RUL

```




```input3
4 1 500000
RLRL

```




```output1
30

```




```output2
134

```




```output3
-1

```



## Note

<p>In the first sample house is a grid with <span class="tex-span">10</span> rows and <span class="tex-span">2</span> columns. Starting a robot anywhere in the second column will result in only one move (thus, one minute of cleaning) in which robot will hit a wall&nbsp;— he tried to go right but there is no third column. Starting a robot anywhere in the first column will result in two moves. The total number of minutes is <span class="tex-span">10·1 + 10·2 = 30</span>.</p><p>In the second sample a started robot will try to move "<span class="tex-font-style-tt">RULRULRULR...</span>" For example, for the leftmost cell in the second row robot will make <span class="tex-span">5</span> moves before it stops because of hitting an upper wall.</p>
