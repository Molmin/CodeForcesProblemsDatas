## Description

<div><p>Vitya has just started learning Berlanese language. It is known that Berlanese uses the Latin alphabet. Vowel letters are "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">u</span>", "<span class="tex-font-style-tt">i</span>", and "<span class="tex-font-style-tt">e</span>". Other letters are consonant.</p><p>In Berlanese, there has to be a vowel after every consonant, but there can be any letter after any vowel. The only exception is a consonant "<span class="tex-font-style-tt">n</span>"; after this letter, there can be any letter (not only a vowel) or there can be no letter at all. For example, the words "<span class="tex-font-style-tt">harakiri</span>", "<span class="tex-font-style-tt">yupie</span>", "<span class="tex-font-style-tt">man</span>", and "<span class="tex-font-style-tt">nbo</span>" are Berlanese while the words "<span class="tex-font-style-tt">horse</span>", "<span class="tex-font-style-tt">king</span>", "<span class="tex-font-style-tt">my</span>", and "<span class="tex-font-style-tt">nz</span>" are not.</p><p>Help Vitya find out if a word $s$ is Berlanese.</p></div><div class="input-specification"><p>The first line of the input contains the string $s$ consisting of $|s|$ ($1\leq |s|\leq 100$) lowercase Latin letters.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a vowel after every consonant except "<span class="tex-font-style-tt">n</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains the string $s$ consisting of $|s|$ ($1\leq |s|\leq 100$) lowercase Latin letters.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a vowel after every consonant except "<span class="tex-font-style-tt">n</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
sumimasen

```




```input2
ninja

```




```input3
codeforces

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first and second samples, a vowel goes after each consonant except "<span class="tex-font-style-tt">n</span>", so the word is Berlanese.</p><p>In the third sample, the consonant "<span class="tex-font-style-tt">c</span>" goes after the consonant "<span class="tex-font-style-tt">r</span>", and the consonant "<span class="tex-font-style-tt">s</span>" stands on the end, so the word is not Berlanese.</p>
