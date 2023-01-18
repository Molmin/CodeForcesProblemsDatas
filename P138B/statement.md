## Description

<div><p>Andrey's favourite number is <span class="tex-span"><i>n</i></span>. Andrey's friends gave him two identical numbers <span class="tex-span"><i>n</i></span> as a New Year present. He hung them on a wall and watched them adoringly.</p><p>Then Andrey got bored from looking at the same number and he started to swap digits first in one, then in the other number, then again in the first number and so on (arbitrary number of changes could be made in each number). At some point it turned out that if we sum the resulting numbers, then the number of zeroes with which the sum will end would be maximum among the possible variants of digit permutations in those numbers.</p><p>Given number <span class="tex-span"><i>n</i></span>, can you find the two digit permutations that have this property?</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> — the original number. The number of digits in this number does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The number is written without any leading zeroes.</p></div><div class="output-specification"><p>Print two permutations of digits of number <span class="tex-span"><i>n</i></span>, such that the sum of these numbers ends with the maximum number of zeroes. The permutations can have leading zeroes (if they are present, they all should be printed). The permutations do not have to be different. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> — the original number. The number of digits in this number does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The number is written without any leading zeroes.</p>

## Output

<p>Print two permutations of digits of number <span class="tex-span"><i>n</i></span>, such that the sum of these numbers ends with the maximum number of zeroes. The permutations can have leading zeroes (if they are present, they all should be printed). The permutations do not have to be different. If there are several answers, print any of them.</p>





```input1
198

```




```input2
500

```




```output1
981
819

```




```output2
500
500

```


