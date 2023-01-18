## Description

<div><p>You are given an integer <span class="tex-span"><i>N</i></span>. Consider all possible segments on the coordinate axis with endpoints at integer points with coordinates between 0 and <span class="tex-span"><i>N</i></span>, inclusive; there will be <img align="middle" class="tex-formula" src="file://QhtfFDHq.png" style="max-width: 100.0%;max-height: 100.0%;"> of them.</p><p>You want to draw these segments in several layers so that in each layer the segments don't overlap (they might touch at the endpoints though). You <span class="tex-font-style-bf">can not</span> move the segments to a different location on the coordinate axis. </p><p>Find the minimal number of layers you have to use for the given <span class="tex-span"><i>N</i></span>.</p></div><div class="input-specification"><p>The only input line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Output a single integer - the minimal number of layers required to draw the segments for the given <span class="tex-span"><i>N</i></span>.</p></div>

## Input

<p>The only input line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>).</p>

## Output

<p>Output a single integer - the minimal number of layers required to draw the segments for the given <span class="tex-span"><i>N</i></span>.</p>





```input1
2

```




```input2
3

```




```input3
4

```




```output1
2

```




```output2
4

```




```output3
6

```



## Note

<p>As an example, here are the segments and their optimal arrangement into layers for <span class="tex-span"><i>N</i> = 4</span>.</p><center> <img class="tex-graphics" src="file://ZipCNRTG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
