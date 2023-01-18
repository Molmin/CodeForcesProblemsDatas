## Description

<div><p>The R1 company has recently bought a high rise building in the centre of Moscow for its main office. It's time to decorate the new office, and the first thing to do is to write the company's slogan above the main entrance to the building.</p><p>The slogan of the company consists of <span class="tex-span"><i>n</i></span> characters, so the decorators hung a large banner, <span class="tex-span"><i>n</i></span> meters wide and <span class="tex-span">1</span> meter high, divided into <span class="tex-span"><i>n</i></span> equal squares. The first character of the slogan must be in the first square (the leftmost) of the poster, the second character must be in the second square, and so on.</p><p>Of course, the R1 programmers want to write the slogan on the poster themselves. To do this, they have a large (and a very heavy) ladder which was put exactly opposite the <span class="tex-span"><i>k</i></span>-th square of the poster. To draw the <span class="tex-span"><i>i</i></span>-th character of the slogan on the poster, you need to climb the ladder, standing in front of the <span class="tex-span"><i>i</i></span>-th square of the poster. This action (along with climbing up and down the ladder) takes one hour for a painter. The painter is not allowed to draw characters in the adjacent squares when the ladder is in front of the <span class="tex-span"><i>i</i></span>-th square because the uncomfortable position of the ladder may make the characters untidy. Besides, the programmers can move the ladder. In one hour, they can move the ladder either a meter to the right or a meter to the left.</p><p>Drawing characters and moving the ladder is very tiring, so the programmers want to finish the job in as little time as possible. Develop for them an optimal poster painting plan!</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span> — the number of characters in the slogan and the initial position of the ladder, correspondingly. The next line contains the slogan as <span class="tex-span"><i>n</i></span> characters written without spaces. Each character of the slogan is either a large English letter, or digit, or one of the characters: '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">!</span>', '<span class="tex-font-style-tt">,</span>', '<span class="tex-font-style-tt">?</span>'.</p></div><div class="output-specification"><p>In <span class="tex-span"><i>t</i></span> lines, print the actions the programmers need to make. In the <span class="tex-span"><i>i</i></span>-th line print:</p><ul> <li> "<span class="tex-font-style-tt">LEFT</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was "move the ladder to the left"; </li><li> "<span class="tex-font-style-tt">RIGHT</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was "move the ladder to the right"; </li><li> "<span class="tex-font-style-tt">PRINT</span> <span class="tex-span"><i>x</i></span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was to "go up the ladder, paint character <span class="tex-span"><i>x</i></span>, go down the ladder". </li></ul><p>The painting time (variable <span class="tex-span"><i>t</i></span>) must be minimum possible. If there are multiple optimal painting plans, you can print any of them.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span> — the number of characters in the slogan and the initial position of the ladder, correspondingly. The next line contains the slogan as <span class="tex-span"><i>n</i></span> characters written without spaces. Each character of the slogan is either a large English letter, or digit, or one of the characters: '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">!</span>', '<span class="tex-font-style-tt">,</span>', '<span class="tex-font-style-tt">?</span>'.</p>

## Output

<p>In <span class="tex-span"><i>t</i></span> lines, print the actions the programmers need to make. In the <span class="tex-span"><i>i</i></span>-th line print:</p><ul> <li> "<span class="tex-font-style-tt">LEFT</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was "move the ladder to the left"; </li><li> "<span class="tex-font-style-tt">RIGHT</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was "move the ladder to the right"; </li><li> "<span class="tex-font-style-tt">PRINT</span> <span class="tex-span"><i>x</i></span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th action was to "go up the ladder, paint character <span class="tex-span"><i>x</i></span>, go down the ladder". </li></ul><p>The painting time (variable <span class="tex-span"><i>t</i></span>) must be minimum possible. If there are multiple optimal painting plans, you can print any of them.</p>





```input1
2 2
R1

```




```input2
2 1
R1

```




```input3
6 4
GO?GO!

```




```output1
PRINT 1
LEFT
PRINT R

```




```output2
PRINT R
RIGHT
PRINT 1

```




```output3
RIGHT
RIGHT
PRINT !
LEFT
PRINT O
LEFT
PRINT G
LEFT
PRINT ?
LEFT
PRINT O
LEFT
PRINT G

```



## Note

<p>Note that the ladder cannot be shifted by less than one meter. The ladder can only stand in front of some square of the poster. For example, you cannot shift a ladder by half a meter and position it between two squares. Then go up and paint the first character and the second character.</p>
