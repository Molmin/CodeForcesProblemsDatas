## Description

<div><p>The knight is standing in front of a long and narrow hallway. A princess is waiting at the end of it.</p><p>In a hallway there are three doors: a red door, a green door and a blue door. The doors are placed one after another, however, possibly in a different order. To proceed to the next door, the knight must first open the door before.</p><p>Each door can be only opened with a key of the corresponding color. So three keys: a red key, a green key and a blue key&nbsp;— are also placed somewhere in the hallway. To open the door, the knight should first pick up the key of its color.</p><p>The knight has a map of the hallway. It can be transcribed as a string, consisting of six characters: </p><ul> <li> <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">G</span>, <span class="tex-font-style-tt">B</span>&nbsp;— denoting red, green and blue doors, respectively; </li><li> <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">g</span>, <span class="tex-font-style-tt">b</span>&nbsp;— denoting red, green and blue keys, respectively. </li></ul><p>Each of these six characters appears in the string exactly once.</p><p>The knight is standing at the beginning of the hallway&nbsp;— on the left on the map.</p><p>Given a map of the hallway, determine if the knight can open all doors and meet the princess at the end of the hallway.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 720$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single string. Each character is one of <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">G</span>, <span class="tex-font-style-tt">B</span> (for the doors), <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">g</span>, <span class="tex-font-style-tt">b</span> (for the keys), and each of them appears exactly once.</p></div><div class="output-specification"><p>For each testcase, print <span class="tex-font-style-tt">YES</span> if the knight can open all doors. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 720$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single string. Each character is one of <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">G</span>, <span class="tex-font-style-tt">B</span> (for the doors), <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">g</span>, <span class="tex-font-style-tt">b</span> (for the keys), and each of them appears exactly once.</p>

## Output

<p>For each testcase, print <span class="tex-font-style-tt">YES</span> if the knight can open all doors. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
4
rgbBRG
RgbrBG
bBrRgG
rgRGBb
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first testcase, the knight first collects all keys, then opens all doors with them.</p><p>In the second testcase, there is a red door right in front of the knight, but he doesn't have a key for it.</p><p>In the third testcase, the key to each door is in front of each respective door, so the knight collects the key and uses it immediately three times.</p><p>In the fourth testcase, the knight can't open the blue door.</p>
