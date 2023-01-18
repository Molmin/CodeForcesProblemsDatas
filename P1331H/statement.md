## Description

<div><p>You are given a mysterious language (codenamed "UnknownX") available in "Custom Test" tab. Find out what this language is, and use it to solve the following problem.</p><p>You are given an integer $input = 1000 * n + mod$ ($1 \le n, mod \le 999$). Calculate <a href="https://en.wikipedia.org/wiki/Double_factorial">double factorial</a> of $n$ modulo $mod$.</p></div><div class="input-specification"><p>The input contains a single integer $input$ ($1001 \le input \le 999999$). You are guaranteed that $input \mod 1000 \neq 0$.</p></div><div class="output-specification"><p>Output a single number.</p></div>

## Input

<p>The input contains a single integer $input$ ($1001 \le input \le 999999$). You are guaranteed that $input \mod 1000 \neq 0$.</p>

## Output

<p>Output a single number.</p>





```input1
6100
```




```input2
9900
```




```input3
100002
```




```input4
123456
```




```output1
48
```




```output2
45
```




```output3
0
```




```output4
171
```



## Note

<p>In the first test case you need to calculate $6!! \mod 100$; $6!! = 6 * 4 * 2 = 48$.</p><p>In the second test case you need to calculate $9!! \mod 900$; $9!! = 9 * 7 * 5 * 3 = 945$.</p><p>In the third test case you need to calculate $100!! \mod 2$; you can notice that $100!!$ is a multiple of 100 and thus is divisible by 2.</p>
