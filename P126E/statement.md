## Description

<div><p>Doctor prescribed medicine to his patient. The medicine is represented by pills. Each pill consists of a shell and healing powder. The shell consists of two halves; each half has one of four colors — blue, red, white or yellow.</p><p>The doctor wants to put <span class="tex-span">28</span> pills in a rectangular box <span class="tex-span">7 × 8</span> in size. Besides, each pill occupies exactly two neighboring cells and any cell contains exactly one half of a pill. Thus, the result is a four colored picture <span class="tex-span">7 × 8</span> in size.</p><p>The doctor thinks that a patient will recover sooner if the picture made by the pills will be special. Unfortunately, putting the pills in the box so as to get the required picture is not a very easy task. That's why doctor asks you to help. </p><p>Doctor has some amount of pills of each of <span class="tex-span">10</span> painting types. They all contain the same medicine, that's why it doesn't matter which <span class="tex-span">28</span> of them will be stored inside the box.</p><p>Place the pills in the box so that the required picture was formed. If it is impossible to place the pills in the required manner, then place them so that the number of matching colors in all <span class="tex-span">56</span> cells in the final arrangement and the doctor's picture were maximum.</p></div><div class="input-specification"><p>First <span class="tex-span">7</span> lines contain the doctor's picture. Each line contains <span class="tex-span">8</span> characters, each character can be "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">Y</span>" that stands for blue, red, white and yellow colors correspondingly.</p><p>Next four lines contain <span class="tex-span">10</span> numbers that stand for, correspondingly, the number of pills painted:</p><p>"<span class="tex-font-style-tt">BY</span>" "<span class="tex-font-style-tt">BW</span>" "<span class="tex-font-style-tt">BR</span>" "<span class="tex-font-style-tt">BB</span>"</p><p>"<span class="tex-font-style-tt">RY</span>" "<span class="tex-font-style-tt">RW</span>" "<span class="tex-font-style-tt">RR</span>"</p><p>"<span class="tex-font-style-tt">WY</span>" "<span class="tex-font-style-tt">WW</span>"</p><p>"<span class="tex-font-style-tt">YY</span>"</p><p>Those numbers lie within range from <span class="tex-span">0</span> to <span class="tex-span">28</span> inclusively. It is guaranteed that the total number of pills in no less than <span class="tex-span">28</span>.</p></div><div class="output-specification"><p>Print on the first line the maximal number cells for which the colors match.</p><p>Then print <span class="tex-span">13</span> lines each containing <span class="tex-span">15</span> characters — the pills' position in the optimal arrangement. The intersections of odd lines and odd columns should contain characters "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">Y</span>". All other positions should contain characters "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">-</span>" and "<span class="tex-font-style-tt">|</span>". Use "<span class="tex-font-style-tt">-</span>" and "<span class="tex-font-style-tt">|</span>" to show which halves belong to one pill. See the samples for more clarification.</p><p>If there are several possible solutions, print any of them.</p></div>

## Input

<p>First <span class="tex-span">7</span> lines contain the doctor's picture. Each line contains <span class="tex-span">8</span> characters, each character can be "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">Y</span>" that stands for blue, red, white and yellow colors correspondingly.</p><p>Next four lines contain <span class="tex-span">10</span> numbers that stand for, correspondingly, the number of pills painted:</p><p>"<span class="tex-font-style-tt">BY</span>" "<span class="tex-font-style-tt">BW</span>" "<span class="tex-font-style-tt">BR</span>" "<span class="tex-font-style-tt">BB</span>"</p><p>"<span class="tex-font-style-tt">RY</span>" "<span class="tex-font-style-tt">RW</span>" "<span class="tex-font-style-tt">RR</span>"</p><p>"<span class="tex-font-style-tt">WY</span>" "<span class="tex-font-style-tt">WW</span>"</p><p>"<span class="tex-font-style-tt">YY</span>"</p><p>Those numbers lie within range from <span class="tex-span">0</span> to <span class="tex-span">28</span> inclusively. It is guaranteed that the total number of pills in no less than <span class="tex-span">28</span>.</p>

## Output

<p>Print on the first line the maximal number cells for which the colors match.</p><p>Then print <span class="tex-span">13</span> lines each containing <span class="tex-span">15</span> characters — the pills' position in the optimal arrangement. The intersections of odd lines and odd columns should contain characters "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">Y</span>". All other positions should contain characters "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">-</span>" and "<span class="tex-font-style-tt">|</span>". Use "<span class="tex-font-style-tt">-</span>" and "<span class="tex-font-style-tt">|</span>" to show which halves belong to one pill. See the samples for more clarification.</p><p>If there are several possible solutions, print any of them.</p>





```input1
WWWBBWWW
WWWBBWWW
YYWBBWWW
YYWBBWRR
YYWBBWRR
YYWBBWRR
YYWBBWRR
0 0 0 8
0 1 5
1 10
5

```




```input2
WWWWWWWW
WBYWRBBY
BRYRBWYY
WWBRYWBB
BWWRWBYW
RBWRBWYY
WWWWWWWW
0 0 0 1
0 0 1
0 1
25

```




```output1
53
W.W.W.B.B.W.W.W
|.|.|.|.|.|.|.|
W.W.W.B.B.W.W.W
...............
Y.Y.W.B.B.W.W-W
|.|.|.|.|.|....
Y.Y.W.B.B.W.R.R
............|.|
Y.Y.W.B.B.R.R.R
|.|.|.|.|.|....
Y.Y.W.B.B.W.R.R
............|.|
Y-Y.B-B.B-B.R.R

```




```output2
15
W.Y.Y-Y.Y-Y.Y-Y
|.|............
W.Y.Y.Y.Y.B-B.Y
....|.|.|.....|
Y-Y.Y.Y.Y.Y-Y.Y
...............
Y.Y.Y.R.Y.Y.Y-Y
|.|.|.|.|.|....
Y.Y.Y.R.Y.Y.Y.Y
............|.|
Y-Y.Y.Y-Y.Y.Y.Y
....|.....|....
Y-Y.Y.Y-Y.Y.Y-Y

```


