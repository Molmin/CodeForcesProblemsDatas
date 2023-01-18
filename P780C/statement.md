## Description

<div><p>Andryusha goes through a park each day. The squares and paths between them look boring to Andryusha, so he decided to decorate them.</p><p>The park consists of <span class="tex-span"><i>n</i></span> squares connected with <span class="tex-span">(<i>n</i> - 1)</span> bidirectional paths in such a way that any square is reachable from any other using these paths. Andryusha decided to hang a colored balloon at each of the squares. The baloons' colors are described by positive integers, starting from <span class="tex-span">1</span>. In order to make the park varicolored, Andryusha wants to choose the colors in a special way. More precisely, he wants to use such colors that if <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> are distinct squares that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> have a direct path between them, and <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> have a direct path between them, then balloon colors on these three squares are distinct.</p><p>Andryusha wants to use as little different colors as possible. Help him to choose the colors!</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of squares in the park.</p><p>Each of the next <span class="tex-span">(<i>n</i> - 1)</span> lines contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>)&nbsp;— the indices of two squares directly connected by a path.</p><p>It is guaranteed that any square is reachable from any other using the paths.</p></div><div class="output-specification"><p>In the first line print single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of colors Andryusha has to use.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the balloon color on the <span class="tex-span"><i>i</i></span>-th square. Each of these numbers should be within range from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of squares in the park.</p><p>Each of the next <span class="tex-span">(<i>n</i> - 1)</span> lines contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>)&nbsp;— the indices of two squares directly connected by a path.</p><p>It is guaranteed that any square is reachable from any other using the paths.</p>

## Output

<p>In the first line print single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of colors Andryusha has to use.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the balloon color on the <span class="tex-span"><i>i</i></span>-th square. Each of these numbers should be within range from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p>





```input1
3
2 3
1 3

```




```input2
5
2 3
5 3
4 3
1 3

```




```input3
5
2 1
3 2
4 3
5 4

```




```output1
3
1 3 2
```




```output2
5
1 3 2 5 4
```




```output3
3
1 2 3 1 2
```



## Note

<p>In the first sample the park consists of three squares: <span class="tex-span">1 → 3 → 2</span>. Thus, the balloon colors have to be distinct.</p><center> <img class="tex-graphics" height="68px" src="file://1gKvJxxw.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px">   <span class="tex-font-size-small">Illustration for the first sample.</span> </center><p>In the second example there are following triples of consequently connected squares: </p><ul> <li> <span class="tex-span">1 → 3 → 2</span> </li><li> <span class="tex-span">1 → 3 → 4</span> </li><li> <span class="tex-span">1 → 3 → 5</span> </li><li> <span class="tex-span">2 → 3 → 4</span> </li><li> <span class="tex-span">2 → 3 → 5</span> </li><li> <span class="tex-span">4 → 3 → 5</span> </li></ul> We can see that each pair of squares is encountered in some triple, so all colors have to be distinct.<center> <img class="tex-graphics" height="178px" src="file://rP31bmB5.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px">   <span class="tex-font-size-small">Illustration for the second sample.</span> </center><p>In the third example there are following triples: </p><ul> <li> <span class="tex-span">1 → 2 → 3</span> </li><li> <span class="tex-span">2 → 3 → 4</span> </li><li> <span class="tex-span">3 → 4 → 5</span> </li></ul> We can see that one or two colors is not enough, but there is an answer that uses three colors only.<center> <img class="tex-graphics" height="106px" src="file://GVXXBXIj.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px">   <span class="tex-font-size-small">Illustration for the third sample.</span> </center>
