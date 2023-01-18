## Description

<div><p>Valera is a little boy. Yesterday he got a huge Math hometask at school, so Valera didn't have enough time to properly learn the English alphabet for his English lesson. Unfortunately, the English teacher decided to have a test on alphabet today. At the test Valera got a square piece of squared paper. The length of the side equals <span class="tex-span"><i>n</i></span> squares (<span class="tex-span"><i>n</i></span> is an odd number) and each unit square contains some small letter of the English alphabet.</p><p>Valera needs to know if the letters written on the square piece of paper form letter "<span class="tex-font-style-tt">X</span>". Valera's teacher thinks that the letters on the piece of paper form an "<span class="tex-font-style-tt">X</span>", if:</p><ul> <li> on both diagonals of the square paper all letters are the same; </li><li> all other squares of the paper (they are not on the diagonals) contain the same letter that is different from the letters on the diagonals. </li></ul><p>Help Valera, write the program that completes the described task for him.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 300</span>; <span class="tex-span"><i>n</i></span> is odd). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> small English letters — the description of Valera's paper.</p></div><div class="output-specification"><p>Print string "<span class="tex-font-style-tt">YES</span>", if the letters on the paper form letter "<span class="tex-font-style-tt">X</span>". Otherwise, print string "<span class="tex-font-style-tt">NO</span>". Print the strings without quotes.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 300</span>; <span class="tex-span"><i>n</i></span> is odd). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> small English letters — the description of Valera's paper.</p>

## Output

<p>Print string "<span class="tex-font-style-tt">YES</span>", if the letters on the paper form letter "<span class="tex-font-style-tt">X</span>". Otherwise, print string "<span class="tex-font-style-tt">NO</span>". Print the strings without quotes.</p>





```input1
5
xooox
oxoxo
soxoo
oxoxo
xooox

```




```input2
3
wsw
sws
wsw

```




```input3
3
xpx
pxp
xpe

```




```output1
NO

```




```output2
YES

```




```output3
NO

```


