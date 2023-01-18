## Description

<div><p>Petr has just bought a new car. He's just arrived at the most known Petersburg's petrol station to refuel it when he suddenly discovered that the petrol tank is secured with a combination lock! The lock has a scale of $360$ degrees and a pointer which initially points at zero:</p><center> <img class="tex-graphics" src="file://3MLZi7KT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Petr called his car dealer, who instructed him to rotate the lock's wheel exactly $n$ times. The $i$-th rotation should be $a_i$ degrees, either clockwise or counterclockwise, and after all $n$ rotations the pointer should again point at zero.</p><p>This confused Petr a little bit as he isn't sure which rotations should be done clockwise and which should be done counterclockwise. As there are many possible ways of rotating the lock, help him and find out whether there exists at least one, such that after all $n$ rotations the pointer will point at zero again.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 15$) — the number of rotations.</p><p>Each of the following $n$ lines contains one integer $a_i$ ($1 \leq a_i \leq 180$) — the angle of the $i$-th rotation in degrees.</p></div><div class="output-specification"><p>If it is possible to do all the rotations so that the pointer will point at zero after all of them are performed, print a single word "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>". Petr will probably buy a new car in this case.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 15$) — the number of rotations.</p><p>Each of the following $n$ lines contains one integer $a_i$ ($1 \leq a_i \leq 180$) — the angle of the $i$-th rotation in degrees.</p>

## Output

<p>If it is possible to do all the rotations so that the pointer will point at zero after all of them are performed, print a single word "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>". Petr will probably buy a new car in this case.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
3
10
20
30
```




```input2
3
10
10
10
```




```input3
3
120
120
120
```




```output1
YES
```




```output2
NO
```




```output3
YES
```



## Note

<p>In the first example, we can achieve our goal by applying the first and the second rotation clockwise, and performing the third rotation counterclockwise.</p><p>In the second example, it's impossible to perform the rotations in order to make the pointer point at zero in the end.</p><p>In the third example, Petr can do all three rotations clockwise. In this case, the whole wheel will be rotated by $360$ degrees clockwise and the pointer will point at zero again.</p>
