## Description

<div><p>Nikolay lives in a two-storied house. There are $n$ rooms on each floor, arranged in a row and numbered from one from left to right. So each room can be represented by the number of the floor and the number of the room on this floor (room number is an integer between $1$ and $n$). </p><p>If Nikolay is currently in some room, he can move to any of the neighbouring rooms (if they exist). Rooms with numbers $i$ and $i+1$ on each floor are neighbouring, for all $1 \leq i \leq n - 1$. There may also be staircases that connect two rooms from different floors having the same numbers. If there is a staircase connecting the room $x$ on the first floor and the room $x$ on the second floor, then Nikolay can use it to move from one room to another.</p><center> <img class="tex-graphics" src="file://HdNyX2YN.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small"> The picture illustrates a house with $n = 4$. There is a staircase between the room $2$ on the first floor and the room $2$ on the second floor, and another staircase between the room $4$ on the first floor and the room $4$ on the second floor. The arrows denote possible directions in which Nikolay can move. The picture corresponds to the string "<span class="tex-font-style-tt">0101</span>" in the input. </span></center> <p>Nikolay wants to move through some rooms in his house. To do this, he firstly chooses any room where he starts. Then Nikolay moves between rooms according to the aforementioned rules. Nikolay never visits the same room twice (he won't enter a room where he has already been). </p><p>Calculate the maximum number of rooms Nikolay can visit during his tour, if:</p><ul> <li> he can start <span class="tex-font-style-bf">in any room on any floor of his choice</span>, </li><li> and <span class="tex-font-style-bf">he won't visit the same room twice</span>. </li></ul></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases in the input. Then test cases follow. Each test case consists of two lines.</p><p>The first line contains one integer $n$ $(1 \le n \le 1\,000)$ — the number of rooms on each floor.</p><p>The second line contains one string consisting of $n$ characters, each character is either a '<span class="tex-font-style-tt">0</span>' or a '<span class="tex-font-style-tt">1</span>'. If the $i$-th character is a '<span class="tex-font-style-tt">1</span>', then there is a staircase between the room $i$ on the first floor and the room $i$ on the second floor. If the $i$-th character is a '<span class="tex-font-style-tt">0</span>', then there is no staircase between the room $i$ on the first floor and the room $i$ on the second floor.</p><p><span class="tex-font-style-bf">In hacks</span> it is allowed to use only one test case in the input, so $t = 1$ should be satisfied.</p></div><div class="output-specification"><p>For each test case print one integer — the maximum number of rooms Nikolay can visit during his tour, if he can start in any room on any floor, and he won't visit the same room twice.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases in the input. Then test cases follow. Each test case consists of two lines.</p><p>The first line contains one integer $n$ $(1 \le n \le 1\,000)$ — the number of rooms on each floor.</p><p>The second line contains one string consisting of $n$ characters, each character is either a '<span class="tex-font-style-tt">0</span>' or a '<span class="tex-font-style-tt">1</span>'. If the $i$-th character is a '<span class="tex-font-style-tt">1</span>', then there is a staircase between the room $i$ on the first floor and the room $i$ on the second floor. If the $i$-th character is a '<span class="tex-font-style-tt">0</span>', then there is no staircase between the room $i$ on the first floor and the room $i$ on the second floor.</p><p><span class="tex-font-style-bf">In hacks</span> it is allowed to use only one test case in the input, so $t = 1$ should be satisfied.</p>

## Output

<p>For each test case print one integer — the maximum number of rooms Nikolay can visit during his tour, if he can start in any room on any floor, and he won't visit the same room twice.</p>





```input1
4
5
00100
8
00000000
5
11111
3
110
```




```output1
6
8
10
6
```



## Note

<p>In the first test case Nikolay may start in the first room of the first floor. Then he moves to the second room on the first floor, and then — to the third room on the first floor. Then he uses a staircase to get to the third room on the second floor. Then he goes to the fourth room on the second floor, and then — to the fifth room on the second floor. So, Nikolay visits $6$ rooms.</p><p>There are no staircases in the second test case, so Nikolay can only visit all rooms on the same floor (if he starts in the leftmost or in the rightmost room).</p><p>In the third test case it is possible to visit all rooms: first floor, first room $\rightarrow$ second floor, first room $\rightarrow$ second floor, second room $\rightarrow$ first floor, second room $\rightarrow$ first floor, third room $\rightarrow$ second floor, third room $\rightarrow$ second floor, fourth room $\rightarrow$ first floor, fourth room $\rightarrow$ first floor, fifth room $\rightarrow$ second floor, fifth room.</p><p>In the fourth test case it is also possible to visit all rooms: second floor, third room $\rightarrow$ second floor, second room $\rightarrow$ second floor, first room $\rightarrow$ first floor, first room $\rightarrow$ first floor, second room $\rightarrow$ first floor, third room.</p>
