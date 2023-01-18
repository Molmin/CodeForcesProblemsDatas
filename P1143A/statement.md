## Description

<div><p>Three years have passes and nothing changed. It is still raining in London, and Mr. Black has to close all the doors in his home in order to not be flooded. Once, however, Mr. Black became so nervous that he opened one door, then another, then one more and so on until he opened all the doors in his house.</p><p>There are exactly two exits from Mr. Black's house, let's name them left and right exits. There are several doors in each of the exits, so each door in Mr. Black's house is located either in the left or in the right exit. You know where each door is located. Initially all the doors are closed. Mr. Black can exit the house if and only if all doors in at least one of the exits is open. You are given a sequence in which Mr. Black opened the doors, please find the smallest index $k$ such that Mr. Black can exit the house after opening the first $k$ doors.</p><p>We have to note that Mr. Black opened each door at most once, and in the end all doors became open.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of doors.</p><p>The next line contains $n$ integers: the sequence in which Mr. Black opened the doors. The $i$-th of these integers is equal to $0$ in case the $i$-th opened door is located in the left exit, and it is equal to $1$ in case it is in the right exit.</p><p>It is guaranteed that there is at least one door located in the left exit and there is at least one door located in the right exit.</p></div><div class="output-specification"><p>Print the smallest integer $k$ such that after Mr. Black opened the first $k$ doors, he was able to exit the house.</p></div>

## Input

<p>The first line contains integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of doors.</p><p>The next line contains $n$ integers: the sequence in which Mr. Black opened the doors. The $i$-th of these integers is equal to $0$ in case the $i$-th opened door is located in the left exit, and it is equal to $1$ in case it is in the right exit.</p><p>It is guaranteed that there is at least one door located in the left exit and there is at least one door located in the right exit.</p>

## Output

<p>Print the smallest integer $k$ such that after Mr. Black opened the first $k$ doors, he was able to exit the house.</p>





```input1
5
0 0 1 0 0
```




```input2
4
1 0 0 1
```




```output1
3
```




```output2
3
```



## Note

<p>In the first example the first two doors are from the left exit, so when Mr. Black opened both of them only, there were two more closed door in the left exit and one closed door in the right exit. So Mr. Black wasn't able to exit at that moment.</p><p>When he opened the third door, all doors from the right exit became open, so Mr. Black was able to exit the house.</p><p>In the second example when the first two doors were opened, there was open closed door in each of the exit.</p><p>With three doors opened Mr. Black was able to use the left exit.</p>
