## Description

<div><p>Andi is a mathematician, a computer scientist, and a songwriter. After spending so much time writing songs, he finally writes a catchy melody that he thought as his best creation. However, the singer who will sing the song/melody has a unique vocal range, thus, an adjustment may be needed.</p><p>A melody is defined as a sequence of $N$ notes which are represented by integers. Let $A$ be the original melody written by Andi. Andi needs to adjust $A$ into a new melody $B$ such that for every $i$ where $1 \le i &lt; N$: </p><ul> <li> If $A_i &lt; A_{i+1}$, then $B_i &lt; B_{i+1}$. </li><li> If $A_i = A_{i+1}$, then $B_i = B_{i+1}$. </li><li> If $A_i &gt; A_{i+1}$, then $B_i &gt; B_{i+1}$. </li><li> $|B_i - B_{i+1}| \le K$, i.e. the difference between two successive notes is no larger than $K$. </li></ul> Moreover, the singer also requires that all notes are within her vocal range, i.e. $L \le B_i \le R$ for all $1 \le i \le N$.<p>Help Andi to determine whether such $B$ exists, and find the lexicographically smallest $B$ if it exists. A melody $X$ is lexicographically smaller than melody $Y$ if and only if there exists $j$ ($1 \le j \le N$) such that $X_i = Y_i$ for all $i &lt; j$ and $X_{j} &lt; Y_{j}$.</p><p>For example, consider a melody $A = \{1,3,5,6,7,8,9,10,3,7,8,9,10,11,12,12\}$ as shown in the following figure. The diagonal arrow up in the figure implies that $A_i &lt; A_{i+1}$, the straight right arrow implies that $A_i = A_{i+1}$, and the diagonal arrow down implies that $A_i &gt; A_{i+1}$.</p><center> <img class="tex-graphics" src="file://DbliBy43.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Supposed we want to make a new melody with $L = 1$, $R = 8$, and $K = 6$. The new melody $B = \{1,2,3,4,5,6,7,8,2,3,4,5,6,7,8,8\}$ as shown in the figure satisfies all the requirements, and it is the lexicographically smallest possible.</p></div><div class="input-specification"><p>Input begins with a line containing four integers: $N$ $L$ $R$ $K$ ($1 \le N \le 100\,000$; $1 \le L \le R \le 10^9$; $1 \le K \le 10^9$) representing the number of notes in the melody, the vocal range ($L$ and $R$), and the maximum difference between two successive notes in the new melody, respectively. The next line contains $N$ integers: $A_i$ ($1 \le A_i \le 10^9$) representing the original melody.</p></div><div class="output-specification"><p>Output in a line $N$ integers (each separated by a single space) representing the lexicographically smallest melody satisfying all the requirements, or output <span class="tex-font-style-tt">-1</span> if there is no melody satisfying all the requirements. Note that it might be possible that the lexicographically smallest melody which satisfies all the requirements to be the same as the original melody.</p></div>

## Input

<p>Input begins with a line containing four integers: $N$ $L$ $R$ $K$ ($1 \le N \le 100\,000$; $1 \le L \le R \le 10^9$; $1 \le K \le 10^9$) representing the number of notes in the melody, the vocal range ($L$ and $R$), and the maximum difference between two successive notes in the new melody, respectively. The next line contains $N$ integers: $A_i$ ($1 \le A_i \le 10^9$) representing the original melody.</p>

## Output

<p>Output in a line $N$ integers (each separated by a single space) representing the lexicographically smallest melody satisfying all the requirements, or output <span class="tex-font-style-tt">-1</span> if there is no melody satisfying all the requirements. Note that it might be possible that the lexicographically smallest melody which satisfies all the requirements to be the same as the original melody.</p>





```input1
16 1 8 6
1 3 5 6 7 8 9 10 3 7 8 9 10 11 12 12
```




```input2
16 1 8 6
1 3 5 6 7 8 9 10 3 7 8 9 10 11 12 13
```




```input3
16 1 10 10
1 3 5 6 7 8 9 10 3 7 8 9 1 11 12 13
```




```output1
1 2 3 4 5 6 7 8 2 3 4 5 6 7 8 8
```




```output2
-1
```




```output3
1 2 3 4 5 6 7 8 1 2 3 4 1 2 3 4
```



## Note

<p><span class="tex-font-style-it">Explanation for the sample input/output #1</span></p><p>This is the example from the problem description.</p>
