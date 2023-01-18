## Description

<div><p>Berland Gardeners United Inc. hired you for the project called "SmartGarden". The main feature of this project is automatic garden watering.</p><p>Formally the garden can be represented as a square of $n \times n$ cells with rows numbered $1$ to $n$ from top to bottom and columns numbered $1$ to $n$ from left to right. Each cell of the garden contains either a plant or a slab. </p><p>It's known that slabs are located on the main diagonal of the matrix representing the garden, and in the cells that are below the main diagonal and share a side with at least one cell of the main diagonal. All the remaining cells of the garden are filled with plants.</p><center> <img class="tex-graphics" src="file://LDkyhiDy.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example of the garden for $n=5$.</span> </center><p>During implementation of the project you created a smart robot that takes a list of commands as an input, which are processed one by one. Each command contains: </p><ul> <li> a list of horizontal lines (rows in the matrix representing the garden); </li><li> a list of vertical lines (columns in the matrix representing the garden). </li></ul><p>While executing each command robot waters only cells in the intersection of specified rows and specified columns. So, if you specify $r$ rows and $c$ columns, then exactly $r \cdot c$ cells will be watered.</p><p>In the demo for the customer you have tuned robot in such a way that it waters all the garden. To do that you prepared a single command containing all $n$ rows and all $n$ columns.</p><p>Unfortunately, 5 hours before the demo for your customer it turned out that the CEO of Berland Gardeners United Inc. was going to take part in it. Moreover, most probably he will be standing on a garden slab during the demo!</p><p>Now you need to create a list of commands for the robot so that it waters all the plants and doesn't water any cell containing a slab. Since it's only a beta version of "SmartGarden", the total number of commands shouldn't exceed $50$.</p><p>Create a program that, for a given size of the garden, will find a list of no more than $50$ commands that allow the robot to water all the plants in the garden without watering the slabs. It is allowed to water a plant several times.</p></div><div class="input-specification"><p>The first and the only line of the input contains a single integer $n$ ($2 \le n \le 5000$), where $n$ is the size of the garden.</p></div><div class="output-specification"><p>In the first line print the total number of commands for the robot $k$ ($1 \le k \le 50$). In the next $2 \cdot k$ lines print all the commands. Each command should be specified by $2$ lines. The first line of each command should describe rows in the command and the second line should describe columns in the command. Each of these $2$ lines should have the following format:</p><ul> <li> the first number of the line should specify the total number of items $x$ in the appropriate list; </li><li> then $x$ <span class="tex-font-style-bf">distinct</span> numbers follow, where each number is in the range $1 \dots n$ and describes a chosen row for the first line and a chosen column for the second line. </li></ul><p>If there are multiple ways to water the garden, print any of them.</p></div>

## Input

<p>The first and the only line of the input contains a single integer $n$ ($2 \le n \le 5000$), where $n$ is the size of the garden.</p>

## Output

<p>In the first line print the total number of commands for the robot $k$ ($1 \le k \le 50$). In the next $2 \cdot k$ lines print all the commands. Each command should be specified by $2$ lines. The first line of each command should describe rows in the command and the second line should describe columns in the command. Each of these $2$ lines should have the following format:</p><ul> <li> the first number of the line should specify the total number of items $x$ in the appropriate list; </li><li> then $x$ <span class="tex-font-style-bf">distinct</span> numbers follow, where each number is in the range $1 \dots n$ and describes a chosen row for the first line and a chosen column for the second line. </li></ul><p>If there are multiple ways to water the garden, print any of them.</p>





```input1
2
```




```input2
4
```




```output1
2
1 1
1 2
1 1
1 2
```




```output2
4
2 1 4
1 2
2 1 2
2 3 4
1 3
2 1 4
1 4
1 1
```


