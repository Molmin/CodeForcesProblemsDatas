## Description

<div><p>Let's call some square matrix with integer values in its cells <span class="tex-font-style-it">palindromic</span> if it doesn't change after the order of rows is reversed and it doesn't change after the order of columns is reversed.</p><p>For example, the following matrices are <span class="tex-font-style-bf"><span class="tex-font-style-it">palindromic</span></span>:</p><center> <img class="tex-graphics" src="file://cQeJYdWu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The following matrices are <span class="tex-font-style-bf">not <span class="tex-font-style-it">palindromic</span></span> because they change after the order of rows is reversed:</p><center> <img class="tex-graphics" src="file://oHIi5d26.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The following matrices are <span class="tex-font-style-bf">not <span class="tex-font-style-it">palindromic</span></span> because they change after the order of columns is reversed:</p><center> <img class="tex-graphics" src="file://fvYegEww.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given $n^2$ integers. Put them into a matrix of $n$ rows and $n$ columns so that each number is used exactly once, each cell contains exactly one number and the resulting matrix is <span class="tex-font-style-it">palindromic</span>. If there are multiple answers, print any. If there is no solution, print "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 20$).</p><p>The second line contains $n^2$ integers $a_1, a_2, \dots, a_{n^2}$ ($1 \le a_i \le 1000$) — the numbers to put into a matrix of $n$ rows and $n$ columns.</p></div><div class="output-specification"><p>If it is possible to put all of the $n^2$ numbers into a matrix of $n$ rows and $n$ columns so that each number is used exactly once, each cell contains exactly one number and the resulting matrix is <span class="tex-font-style-it">palindromic</span>, then print "<span class="tex-font-style-tt">YES</span>". Then print $n$ lines with $n$ space-separated numbers — the resulting matrix.</p><p>If it's impossible to construct any matrix, then print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 20$).</p><p>The second line contains $n^2$ integers $a_1, a_2, \dots, a_{n^2}$ ($1 \le a_i \le 1000$) — the numbers to put into a matrix of $n$ rows and $n$ columns.</p>

## Output

<p>If it is possible to put all of the $n^2$ numbers into a matrix of $n$ rows and $n$ columns so that each number is used exactly once, each cell contains exactly one number and the resulting matrix is <span class="tex-font-style-it">palindromic</span>, then print "<span class="tex-font-style-tt">YES</span>". Then print $n$ lines with $n$ space-separated numbers — the resulting matrix.</p><p>If it's impossible to construct any matrix, then print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p>





```input1
4
1 8 8 1 2 2 2 2 2 2 2 2 1 8 8 1
```




```input2
3
1 1 1 1 1 3 3 3 3
```




```input3
4
1 2 1 9 8 4 3 8 8 3 4 8 9 2 1 1
```




```input4
1
10
```




```output1
YES
1 2 2 1
8 2 2 8
8 2 2 8
1 2 2 1
```




```output2
YES
1 3 1
3 1 3
1 3 1
```




```output3
NO
```




```output4
YES
10
```



## Note

<p>Note that there exist multiple answers for the first two examples.</p>
