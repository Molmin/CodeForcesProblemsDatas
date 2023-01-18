## Description

<div><p>Melody Pond was stolen from her parents as a newborn baby by Madame Kovarian, to become a weapon of the Silence in their crusade against the Doctor. Madame Kovarian changed Melody's name to River Song, giving her a new identity that allowed her to kill the Eleventh Doctor.</p><p>Heidi figured out that Madame Kovarian uses a very complicated hashing function in order to change the names of the babies she steals. In order to prevent this from happening to future Doctors, Heidi decided to prepare herself by learning some basic hashing techniques.</p><p>The first hashing function she designed is as follows.</p><p>Given two positive integers $(x, y)$ she defines $H(x,y):=x^2+2xy+x+1$.</p><p>Now, Heidi wonders if the function is reversible. That is, given a positive integer $r$, can you find a pair $(x, y)$ (of positive integers) such that $H(x, y) = r$?</p><p>If multiple such pairs exist, output the one with smallest possible $x$. If there is no such pair, output "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first and only line contains an integer $r$ ($1 \le r \le 10^{12}$).</p></div><div class="output-specification"><p>Output integers $x, y$ such that $H(x,y) = r$ and $x$ is smallest possible, or "<span class="tex-font-style-tt">NO</span>" if no such pair exists.</p></div>

## Input

<p>The first and only line contains an integer $r$ ($1 \le r \le 10^{12}$).</p>

## Output

<p>Output integers $x, y$ such that $H(x,y) = r$ and $x$ is smallest possible, or "<span class="tex-font-style-tt">NO</span>" if no such pair exists.</p>





```input1
19
```




```input2
16
```




```output1
1 8
```




```output2
NO
```


