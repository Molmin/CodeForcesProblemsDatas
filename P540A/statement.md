## Description

<div><p>Scrooge McDuck keeps his most treasured savings in a home safe with a combination lock. Each time he wants to put there the treasures that he's earned fair and square, he has to open the lock.</p><center> <img class="tex-graphics" src="file://CeTlOxyn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The combination lock is represented by <span class="tex-span"><i>n</i></span> rotating disks with digits from 0 to 9 written on them. Scrooge McDuck has to turn some disks so that the combination of digits on the disks forms a secret combination. In one move, he can rotate one disk one digit forwards or backwards. In particular, in one move he can go from digit 0 to digit 9 and vice versa. What minimum number of actions does he need for that?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of disks on the combination lock.</p><p>The second line contains a string of <span class="tex-span"><i>n</i></span> digits&nbsp;— the original state of the disks.</p><p>The third line contains a string of <span class="tex-span"><i>n</i></span> digits&nbsp;— Scrooge McDuck's combination that opens the lock.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of moves Scrooge McDuck needs to open the lock.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of disks on the combination lock.</p><p>The second line contains a string of <span class="tex-span"><i>n</i></span> digits&nbsp;— the original state of the disks.</p><p>The third line contains a string of <span class="tex-span"><i>n</i></span> digits&nbsp;— Scrooge McDuck's combination that opens the lock.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of moves Scrooge McDuck needs to open the lock.</p>





```input1
5
82195
64723

```




```output1
13

```



## Note

<p>In the sample he needs 13 moves:</p><ul> <li> 1 disk: <img align="middle" class="tex-formula" src="file://O1lOYo3s.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> 2 disk: <img align="middle" class="tex-formula" src="file://PbjDjCqX.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> 3 disk: <img align="middle" class="tex-formula" src="file://LHM64iqx.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> 4 disk: <img align="middle" class="tex-formula" src="file://aqEEJB0i.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> 5 disk: <img align="middle" class="tex-formula" src="file://Jy5J3c4y.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul>
