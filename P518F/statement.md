## Description

<div><p>On a certain meeting of a ruling party "<span class="tex-font-style-tt">A</span>" minister Pavel suggested to improve the sewer system and to create a new pipe in the city.</p><p>The city is an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular squared field. Each square of the field is either empty (then the pipe can go in it), or occupied (the pipe cannot go in such square). Empty squares are denoted by character '<span class="tex-span">.</span>', occupied squares are denoted by character '<span class="tex-span">#</span>'.</p><p>The pipe must meet the following criteria:</p><ul> <li> the pipe is a polyline of width <span class="tex-span">1</span>, </li><li> the pipe goes in empty squares, </li><li> the pipe starts from the edge of the field, but not from a corner square, </li><li> the pipe ends at the edge of the field but not in a corner square, </li><li> the pipe has at most <span class="tex-span">2</span> turns (<span class="tex-span">90</span> degrees), </li><li> the border squares of the field must share <span class="tex-font-style-bf">exactly two</span> squares with the pipe, </li><li> if the pipe looks like a single segment, then the end points of the pipe must lie on distinct edges of the field, </li><li> for each non-border square of the pipe there are <span class="tex-font-style-bf">exacly two</span> side-adjacent squares that also belong to the pipe, </li><li> for each border square of the pipe there is <span class="tex-font-style-bf">exactly one</span> side-adjacent cell that also belongs to the pipe. </li></ul><p>Here are some samples of <span class="tex-font-style-bf">allowed</span> piping routes: </p><pre class="verbatim"><br>           ....#            ....#            .*..#<br>           *****            ****.            .***.<br>           ..#..            ..#*.            ..#*.<br>           #...#            #..*#            #..*#<br>           .....            ...*.            ...*.<br></pre><p>Here are some samples of <span class="tex-font-style-bf">forbidden</span> piping routes: </p><pre class="verbatim"><br>           .**.#            *...#            .*.*#<br>           .....            ****.            .*.*.<br>           ..#..            ..#*.            .*#*.<br>           #...#            #..*#            #*.*#<br>           .....            ...*.            .***.<br></pre><p>In these samples the pipes are represented by characters '<span class="tex-span"> * </span>'.</p><p>You were asked to write a program that calculates the number of distinct ways to make exactly one pipe in the city. </p><p>The two ways to make a pipe are considered distinct if they are distinct in at least one square.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>)&nbsp;—&nbsp;the height and width of Berland map.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the map of the city. </p><p>If the square of the map is marked by character '<span class="tex-span">.</span>', then the square is empty and the pipe can through it. </p><p>If the square of the map is marked by character '<span class="tex-span">#</span>', then the square is full and the pipe can't through it.</p></div><div class="output-specification"><p>In the first line of the output print a single integer — the number of distinct ways to create a pipe.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>)&nbsp;—&nbsp;the height and width of Berland map.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the map of the city. </p><p>If the square of the map is marked by character '<span class="tex-span">.</span>', then the square is empty and the pipe can through it. </p><p>If the square of the map is marked by character '<span class="tex-span">#</span>', then the square is full and the pipe can't through it.</p>

## Output

<p>In the first line of the output print a single integer — the number of distinct ways to create a pipe.</p>





```input1
3 3
...
..#
...

```




```input2
4 2
..
..
..
..

```




```input3
4 5
#...#
#...#
###.#
###.#

```




```output1
3
```




```output2
2

```




```output3
4
```



## Note

<p>In the first sample there are 3 ways to make a pipe (the squares of the pipe are marked by characters '<span class="tex-span"> * </span>'): </p><pre class="verbatim"><br>       .*.        .*.        ...<br>       .*#        **#        **#<br>       .*.        ...        .*.<br></pre>
