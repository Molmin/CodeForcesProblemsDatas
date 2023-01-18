## Description

<div><p>Some people leave the lights at their workplaces on when they leave that is a waste of resources. As a hausmeister of DHBW, Sagheer waits till all students and professors leave the university building, then goes and turns all the lights off.</p><p>The building consists of <span class="tex-span"><i>n</i></span> floors with stairs at the left and the right sides. Each floor has <span class="tex-span"><i>m</i></span> rooms on the same line with a corridor that connects the left and right stairs passing by all the rooms. In other words, the building can be represented as a rectangle with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i> + 2</span> columns, where the first and the last columns represent the stairs, and the <span class="tex-span"><i>m</i></span> columns in the middle represent rooms.</p><p>Sagheer is standing at the ground floor at the left stairs. He wants to turn all the lights off in such a way that he will not go upstairs until all lights in the floor he is standing at are off. Of course, Sagheer must visit a room to turn the light there off. It takes one minute for Sagheer to go to the next floor using stairs or to move from the current room/stairs to a neighboring room/stairs on the same floor. It takes no time for him to switch the light off in the room he is currently standing in. Help Sagheer find the minimum total time to turn off all the lights.</p><p>Note that Sagheer does not have to go back to his starting position, and he does not have to visit rooms where the light is already switched off.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span> and <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>) — the number of floors and the number of rooms in each floor, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains the building description. Each line contains a binary string of length <span class="tex-span"><i>m</i> + 2</span> representing a floor (the left stairs, then <span class="tex-span"><i>m</i></span> rooms, then the right stairs) where <span class="tex-span">0</span> indicates that the light is off and <span class="tex-span">1</span> indicates that the light is on. The floors are listed from top to bottom, so that the last line represents the ground floor.</p><p>The first and last characters of each string represent the left and the right stairs, respectively, so they are always <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum total time needed to turn off all the lights.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span> and <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>) — the number of floors and the number of rooms in each floor, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains the building description. Each line contains a binary string of length <span class="tex-span"><i>m</i> + 2</span> representing a floor (the left stairs, then <span class="tex-span"><i>m</i></span> rooms, then the right stairs) where <span class="tex-span">0</span> indicates that the light is off and <span class="tex-span">1</span> indicates that the light is on. The floors are listed from top to bottom, so that the last line represents the ground floor.</p><p>The first and last characters of each string represent the left and the right stairs, respectively, so they are always <span class="tex-span">0</span>.</p>

## Output

<p>Print a single integer — the minimum total time needed to turn off all the lights.</p>





```input1
2 2
0010
0100

```




```input2
3 4
001000
000010
000010

```




```input3
4 3
01110
01110
01110
01110

```




```output1
5

```




```output2
12

```




```output3
18

```



## Note

<p>In the first example, Sagheer will go to room <span class="tex-span">1</span> in the ground floor, then he will go to room <span class="tex-span">2</span> in the second floor using the left or right stairs.</p><p>In the second example, he will go to the fourth room in the ground floor, use right stairs, go to the fourth room in the second floor, use right stairs again, then go to the second room in the last floor.</p><p>In the third example, he will walk through the whole corridor alternating between the left and right stairs at each floor.</p>
