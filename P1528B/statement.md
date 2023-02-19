## Description

<div><p>Kavi has $2n$ points lying on the $OX$ axis, $i$-th of which is located at $x = i$.</p><p>Kavi considers all ways to split these $2n$ points into $n$ pairs. Among those, he is interested in <span class="tex-font-style-bf">good</span> pairings, which are defined as follows:</p><p>Consider $n$ segments with ends at the points in correspondent pairs. The pairing is called good, if for every $2$ different segments $A$ and $B$ among those, at least one of the following holds:</p><ul> <li> One of the segments $A$ and $B$ lies completely inside the other. </li><li> $A$ and $B$ have the same length. </li></ul><p>Consider the following example:</p><center> <img class="tex-graphics" src="file://2dsUVfdF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>$A$ is a good pairing since the red segment lies completely inside the blue segment.</p><p>$B$ is a good pairing since the red and the blue segment have the same length.</p><p>$C$ is not a good pairing since none of the red or blue segments lies inside the other, neither do they have the same size.</p><p>Kavi is interested in the number of good pairings, so he wants you to find it for him. As the result can be large, find this number modulo $998244353$.</p><p>Two pairings are called different, if some two points are in one pair in some pairing and in different pairs in another.</p></div><div class="input-specification"><p>The single line of the input contains a single integer $n$ $(1\le n \le 10^6)$.</p></div><div class="output-specification"><p>Print the number of good pairings modulo $998244353$.</p></div>

## Input

<p>The single line of the input contains a single integer $n$ $(1\le n \le 10^6)$.</p>

## Output

<p>Print the number of good pairings modulo $998244353$.</p>





```input1
1
```




```input2
2
```




```input3
3
```




```input4
100
```




```output1
1
```




```output2
3
```




```output3
6
```




```output4
688750769
```



## Note

<p>The good pairings for the second example are: </p><center> <img class="tex-graphics" src="file://oP9kpeH3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, the good pairings are: </p><center> <img class="tex-graphics" src="file://3sty2xGG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
