## Description

<div><p>Today in the scientific lyceum of the Kingdom of Kremland, there was a biology lesson. The topic of the lesson was the <span class="tex-font-style-it">genomes</span>. Let's call the <span class="tex-font-style-it">genome</span> the string "<span class="tex-font-style-tt">ACTG</span>".</p><p>Maxim was very boring to sit in class, so the teacher came up with a task for him: on a given string $s$ consisting of uppercase letters and length of at least $4$, you need to find the minimum number of <span class="tex-font-style-it">operations</span> that you need to apply, so that the <span class="tex-font-style-it">genome</span> appears in it as a substring. For one <span class="tex-font-style-it">operation</span>, you can replace any letter in the string $s$ with the next or previous in the alphabet. For example, for the letter "<span class="tex-font-style-tt">D</span>" the previous one will be "<span class="tex-font-style-tt">C</span>", and the next&nbsp;— "<span class="tex-font-style-tt">E</span>". In this problem, we assume that for the letter "<span class="tex-font-style-tt">A</span>", the previous one will be the letter "<span class="tex-font-style-tt">Z</span>", and the next one will be "<span class="tex-font-style-tt">B</span>", and for the letter "<span class="tex-font-style-tt">Z</span>", the previous one is the letter "<span class="tex-font-style-tt">Y</span>", and the next one is the letter "<span class="tex-font-style-tt">A</span>".</p><p>Help Maxim solve the problem that the teacher gave him.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($4 \leq n \leq 50$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$, consisting of exactly $n$ uppercase letters of the Latin alphabet.</p></div><div class="output-specification"><p>Output the minimum number of <span class="tex-font-style-it">operations</span> that need to be applied to the string $s$ so that the <span class="tex-font-style-it">genome</span> appears as a substring in it.</p></div>

## Input

<p>The first line contains a single integer $n$ ($4 \leq n \leq 50$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$, consisting of exactly $n$ uppercase letters of the Latin alphabet.</p>

## Output

<p>Output the minimum number of <span class="tex-font-style-it">operations</span> that need to be applied to the string $s$ so that the <span class="tex-font-style-it">genome</span> appears as a substring in it.</p>





```input1
4
ZCTH
```




```input2
5
ZDATG
```




```input3
6
AFBAKC
```




```output1
2
```




```output2
5
```




```output3
16
```



## Note

<p>In the first example, you should replace the letter "<span class="tex-font-style-tt">Z</span>" with "<span class="tex-font-style-tt">A</span>" for one <span class="tex-font-style-it">operation</span>, the letter "<span class="tex-font-style-tt">H</span>"&nbsp;— with the letter "<span class="tex-font-style-tt">G</span>" for one <span class="tex-font-style-it">operation</span>. You will get the string "<span class="tex-font-style-tt">ACTG</span>", in which the <span class="tex-font-style-it">genome</span> is present as a substring.</p><p>In the second example, we replace the letter "<span class="tex-font-style-tt">A</span>" with "<span class="tex-font-style-tt">C</span>" for two <span class="tex-font-style-it">operations</span>, the letter "<span class="tex-font-style-tt">D</span>"&nbsp;— with the letter "<span class="tex-font-style-tt">A</span>" for three <span class="tex-font-style-it">operations</span>. You will get the string "<span class="tex-font-style-tt">ZACTG</span>", in which there is a <span class="tex-font-style-it">genome</span>.</p>
