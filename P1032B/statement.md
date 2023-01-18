## Description

<div><p>At many competitions that have a word «cup» in its official name the winner is presented with an actual cup. This time the organizers of one unusual programming competition have decided to please the winner even more and to add a nameplate to the cup with the handle of the winner.</p><p>The nameplate is to be rectangular and the text on it will be printed as a table of several rows and columns. Having some measurements done, the organizers have found out that the number $a$ of rows cannot be greater than $5$ while the number $b$ of columns cannot exceed $20$. Every cell of the table will contain either an asterisk («<span class="tex-font-style-tt">*</span>») or a letter of user's handle.</p><p>Furthermore, the organizers want the rows of the table to be uniform, which means that the number of asterisks used in different rows should differ by at most one (i.e. you can't have two asterisks in the first row and none in the second). The main goal, however, is to obtain the winner's handle precisely when reading the table from top to bottom and from left to right in every row (skipping asterisks).</p><p>The organizers want for the nameplate to have as few rows as possible and among all valid tables with the minimum number of rows they want to choose the one that has the minimum number of columns.</p><p>The winner is not yet determined so your task is to write a program that, given a certain handle, generates the necessary table.</p></div><div class="input-specification"><p>The only line contains one string $s$ ($1 \le |s| \le 100$), comprised of uppercase and lowercase Latin letters, &nbsp;— the handle of the winner.</p></div><div class="output-specification"><p>In the first line output the minimum number $a$ of rows in the table and the minimum number $b$ of columns in an optimal table with rows.</p><p>The following $a$ lines should contain $b$ characters each &nbsp;— any valid table.</p></div>

## Input

<p>The only line contains one string $s$ ($1 \le |s| \le 100$), comprised of uppercase and lowercase Latin letters, &nbsp;— the handle of the winner.</p>

## Output

<p>In the first line output the minimum number $a$ of rows in the table and the minimum number $b$ of columns in an optimal table with rows.</p><p>The following $a$ lines should contain $b$ characters each &nbsp;— any valid table.</p>





```input1
tourist
```




```input2
MyNameIsLifeIAmForeverByYourSideMyNameIsLife
```




```output1
1 7
tourist
```




```output2
3 15
MyNameIsLifeIAm
ForeverByYourSi
deMyNameIsL*ife
```


