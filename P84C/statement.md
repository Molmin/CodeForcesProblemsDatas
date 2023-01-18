## Description

<div><p>Perhaps many have heard that the World Biathlon Championship has finished. Although our hero Valera was not present at this spectacular event himself and only watched it on TV, it excited him so much that he decided to enroll in a biathlon section.</p><p>Of course, biathlon as any sport, proved very difficult in practice. It takes much time and effort. Workouts, workouts, and workouts, — that's what awaited Valera on his way to great achievements in biathlon.</p><p>As for the workouts, you all probably know that every professional biathlete should ski fast and shoot precisely at the shooting range. Only in this case you can hope to be successful, because running and shooting are the two main components of biathlon. Valera has been diligent in his ski trainings, which is why he runs really fast, however, his shooting accuracy is nothing to write home about.</p><p>On a biathlon base where Valera is preparing for the competition, there is a huge rifle range with <span class="tex-span"><i>n</i></span> targets. Each target have shape of a circle, and <span class="tex-font-style-bf">the center of each circle is located on the <span class="tex-span"><i>Ox</i></span> axis</span>. At the last training session Valera made the total of <span class="tex-span"><i>m</i></span> shots. To make monitoring of his own results easier for him, one rather well-known programmer (of course it is you) was commissioned to write a program that would reveal how many and which targets Valera hit. More specifically, for each target the program must print the number of <span class="tex-font-style-bf">the first</span> successful shot (in the target), or "-1" if this was not hit. <span class="tex-font-style-bf">The target is considered hit if the shot is inside the circle or on its boundary.</span> Valera is counting on you and perhaps, thanks to you he will one day win international competitions.</p></div><div class="input-specification"><p>The first line of the input file contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>), which is the number of targets. The next <span class="tex-span"><i>n</i></span> lines contain descriptions of the targets. Each target is a circle whose center is located on the <span class="tex-span"><i>Ox</i></span> axis. Each circle is given by its coordinate of the center <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - 2·10<sup class="upper-index">4</sup> ≤ <i>x</i> ≤ 2·10<sup class="upper-index">4</sup></span>) and its radius <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 1000</span>). <span class="tex-font-style-bf">It is guaranteed that no two targets coincide, intersect or are nested into each other, but they can touch each other.</span> </p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), which is the number of shots. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the shots, which are points on the plane, given by their coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"> - 2·10<sup class="upper-index">4</sup> ≤ <i>x</i>, <i>y</i> ≤ 2·10<sup class="upper-index">4</sup></span>).</p><p>All the numbers in the input are integers. </p><p>Targets and shots are numbered starting from one in the order of the input.</p></div><div class="output-specification"><p>Print on the first line a single number, the number of targets hit by Valera. Print on the second line for each of the targets the number of its first hit or "-1" (without quotes) if this number does not exist. Separate numbers with spaces.</p></div>

## Input

<p>The first line of the input file contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>), which is the number of targets. The next <span class="tex-span"><i>n</i></span> lines contain descriptions of the targets. Each target is a circle whose center is located on the <span class="tex-span"><i>Ox</i></span> axis. Each circle is given by its coordinate of the center <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - 2·10<sup class="upper-index">4</sup> ≤ <i>x</i> ≤ 2·10<sup class="upper-index">4</sup></span>) and its radius <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 1000</span>). <span class="tex-font-style-bf">It is guaranteed that no two targets coincide, intersect or are nested into each other, but they can touch each other.</span> </p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), which is the number of shots. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the shots, which are points on the plane, given by their coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"> - 2·10<sup class="upper-index">4</sup> ≤ <i>x</i>, <i>y</i> ≤ 2·10<sup class="upper-index">4</sup></span>).</p><p>All the numbers in the input are integers. </p><p>Targets and shots are numbered starting from one in the order of the input.</p>

## Output

<p>Print on the first line a single number, the number of targets hit by Valera. Print on the second line for each of the targets the number of its first hit or "-1" (without quotes) if this number does not exist. Separate numbers with spaces.</p>





```input1
3
2 1
5 2
10 1
5
0 1
1 3
3 0
4 0
4 0

```




```input2
3
3 2
7 1
11 2
4
2 1
6 0
6 4
11 2

```




```output1
2
3 3 -1 

```




```output2
3
1 2 4 

```


