## Description

<div><p>Phoenix is playing with a new puzzle, which consists of $n$ identical puzzle pieces. Each puzzle piece is a right isosceles triangle as shown below.</p><center> <img class="tex-graphics" height="113px" src="file://HNBenKZP.png" style="max-width: 100.0%;max-height: 100.0%;" width="113px">   <span class="tex-font-size-small">A puzzle piece</span> </center><p>The goal of the puzzle is to create a <span class="tex-font-style-bf">square</span> using the $n$ pieces. He is allowed to rotate and move the pieces around, but none of them can overlap and all $n$ pieces must be used (of course, the square shouldn't contain any holes as well). Can he do it?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of puzzle pieces.</p></div><div class="output-specification"><p>For each test case, if Phoenix can create a square with the $n$ puzzle pieces, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of puzzle pieces.</p>

## Output

<p>For each test case, if Phoenix can create a square with the $n$ puzzle pieces, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
3
2
4
6
```




```output1
YES
YES
NO
```



## Note

<p>For $n=2$, Phoenix can create a square like this:</p><center> <img class="tex-graphics" height="113px" src="file://WzOzBEyN.png" style="max-width: 100.0%;max-height: 100.0%;" width="113px">   </center><p>For $n=4$, Phoenix can create a square like this:</p><center> <img class="tex-graphics" height="159px" src="file://KjpTnjbQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="159px">   </center><p>For $n=6$, it is impossible for Phoenix to create a square.</p>
