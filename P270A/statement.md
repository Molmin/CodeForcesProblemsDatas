## Description

<div><p>Emuskald needs a fence around his farm, but he is too lazy to build it himself. So he purchased a fence-building robot.</p><p>He wants the fence to be a regular polygon. The robot builds the fence along a single path, but it can only make fence corners at a single angle <span class="tex-span"><i>a</i></span>.</p><p>Will the robot be able to build the fence Emuskald wants? In other words, is there a regular polygon which angles are equal to <span class="tex-span"><i>a</i></span>?</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 &lt; <i>t</i> &lt; 180</span>) — the number of tests. Each of the following <span class="tex-span"><i>t</i></span> lines contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 &lt; <i>a</i> &lt; 180</span>) — the angle the robot can make corners at measured in degrees.</p></div><div class="output-specification"><p>For each test, output on a single line "<span class="tex-font-style-tt">YES</span>" (without quotes), if the robot can build a fence Emuskald wants, and "<span class="tex-font-style-tt">NO</span>" (without quotes), if it is impossible.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 &lt; <i>t</i> &lt; 180</span>) — the number of tests. Each of the following <span class="tex-span"><i>t</i></span> lines contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 &lt; <i>a</i> &lt; 180</span>) — the angle the robot can make corners at measured in degrees.</p>

## Output

<p>For each test, output on a single line "<span class="tex-font-style-tt">YES</span>" (without quotes), if the robot can build a fence Emuskald wants, and "<span class="tex-font-style-tt">NO</span>" (without quotes), if it is impossible.</p>





```input1
3
30
60
90

```




```output1
NO
YES
YES

```



## Note

<p>In the first test case, it is impossible to build the fence, since there is no regular polygon with angle <img align="middle" class="tex-formula" src="file://G8aFRRPq.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second test case, the fence is a regular triangle, and in the last test case — a square.</p>
