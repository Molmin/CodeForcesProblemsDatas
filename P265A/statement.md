## Description

<div><p>There is a sequence of colorful stones. The color of each stone is one of red, green, or blue. You are given a string <span class="tex-span"><i>s</i></span>. The <span class="tex-span"><i>i</i></span>-th (1-based) character of <span class="tex-span"><i>s</i></span> represents the color of the <span class="tex-span"><i>i</i></span>-th stone. If the character is "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>", the color of the corresponding stone is red, green, or blue, respectively.</p><p>Initially Squirrel Liss is standing on the first stone. You perform instructions one or more times.</p><p>Each instruction is one of the three types: "<span class="tex-font-style-tt">RED</span>", "<span class="tex-font-style-tt">GREEN</span>", or "<span class="tex-font-style-tt">BLUE</span>". After an instruction <span class="tex-span"><i>c</i></span>, if Liss is standing on a stone whose colors is <span class="tex-span"><i>c</i></span>, Liss will move one stone forward, else she will not move.</p><p>You are given a string <span class="tex-span"><i>t</i></span>. The number of instructions is equal to the length of <span class="tex-span"><i>t</i></span>, and the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>t</i></span> represents the <span class="tex-span"><i>i</i></span>-th instruction.</p><p>Calculate the final position of Liss (the number of the stone she is going to stand on in the end) after performing all the instructions, and print its 1-based position. It is guaranteed that Liss don't move out of the sequence.</p></div><div class="input-specification"><p>The input contains two lines. The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>). The second line contains the string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 50</span>). The characters of each string will be one of "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>". It is guaranteed that Liss don't move out of the sequence.</p></div><div class="output-specification"><p>Print the final 1-based position of Liss in a single line.</p></div>

## Input

<p>The input contains two lines. The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>). The second line contains the string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 50</span>). The characters of each string will be one of "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>". It is guaranteed that Liss don't move out of the sequence.</p>

## Output

<p>Print the final 1-based position of Liss in a single line.</p>





```input1
RGB
RRR

```




```input2
RRRBGBRBBB
BBBRR

```




```input3
BRRBGBRGRBGRGRRGGBGBGBRGBRGRGGGRBRRRBRBBBGRRRGGBBB
BBRBGGRGRGBBBRBGRBRBBBBRBRRRBGBBGBBRRBBGGRBRRBRGRB

```




```output1
2

```




```output2
3

```




```output3
15

```


