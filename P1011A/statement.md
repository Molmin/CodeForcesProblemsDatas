## Description

<div><p>Natasha is going to fly to Mars. She needs to build a rocket, which consists of several stages in some order. Each of the stages is defined by a lowercase Latin letter. This way, the rocket can be described by the string&nbsp;— concatenation of letters, which correspond to the stages.</p><p>There are $n$ stages available. The rocket must contain exactly $k$ of them. Stages in the rocket should be ordered by their weight. So, after the stage with some letter can go only stage with a letter, which is at least two positions after in the alphabet (skipping one letter in between, or even more). For example, after letter '<span class="tex-font-style-tt">c</span>' can't go letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">d</span>', but can go letters '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">f</span>', ..., '<span class="tex-font-style-tt">z</span>'.</p><p>For the rocket to fly as far as possible, its weight should be minimal. The weight of the rocket is equal to the sum of the weights of its stages. The weight of the stage is the number of its letter in the alphabet. For example, the stage '<span class="tex-font-style-tt">a</span> 'weighs one ton,' <span class="tex-font-style-tt">b</span> 'weighs two tons, and' <span class="tex-font-style-tt">z</span>'&nbsp;— $26$ tons.</p><p>Build the rocket with the minimal weight or determine, that it is impossible to build a rocket at all. Each stage can be used at most once.</p></div><div class="input-specification"><p>The first line of input contains two integers&nbsp;— $n$ and $k$ ($1 \le k \le n \le 50$)&nbsp;– the number of available stages and the number of stages to use in the rocket.</p><p>The second line contains string $s$, which consists of exactly $n$ lowercase Latin letters. Each letter defines a new stage, which can be used to build the rocket. Each stage can be used at most once.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimal total weight of the rocket or <span class="tex-font-style-tt">-1</span>, if it is impossible to build the rocket at all.</p></div>

## Input

<p>The first line of input contains two integers&nbsp;— $n$ and $k$ ($1 \le k \le n \le 50$)&nbsp;– the number of available stages and the number of stages to use in the rocket.</p><p>The second line contains string $s$, which consists of exactly $n$ lowercase Latin letters. Each letter defines a new stage, which can be used to build the rocket. Each stage can be used at most once.</p>

## Output

<p>Print a single integer&nbsp;— the minimal total weight of the rocket or <span class="tex-font-style-tt">-1</span>, if it is impossible to build the rocket at all.</p>





```input1
5 3
xyabd

```




```input2
7 4
problem

```




```input3
2 2
ab

```




```input4
12 1
abaabbaaabbb

```




```output1
29
```




```output2
34
```




```output3
-1
```




```output4
1
```



## Note

<p>In the first example, the following rockets satisfy the condition:</p><ul><li> "<span class="tex-font-style-tt">adx</span>" (weight is $1+4+24=29$);</li><li> "<span class="tex-font-style-tt">ady</span>" (weight is $1+4+25=30$);</li><li> "<span class="tex-font-style-tt">bdx</span>" (weight is $2+4+24=30$);</li><li> "<span class="tex-font-style-tt">bdy</span>" (weight is $2+4+25=31$).</li></ul><p>Rocket "<span class="tex-font-style-tt">adx</span>" has the minimal weight, so the answer is $29$.</p><p>In the second example, target rocket is "<span class="tex-font-style-tt">belo</span>". Its weight is $2+5+12+15=34$.</p><p>In the third example, $n=k=2$, so the rocket must have both stages: '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. This rocket doesn't satisfy the condition, because these letters are adjacent in the alphabet. Answer is <span class="tex-font-style-tt">-1</span>.</p>
