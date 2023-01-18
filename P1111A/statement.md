## Description

<div><p>We all know that a superhero can transform to certain other superheroes. But not all Superheroes can transform to any other superhero. A superhero with name $s$ can transform to another superhero with name $t$ if $s$ can be made equal to $t$ by changing any vowel in $s$ to any other vowel and any consonant in $s$ to any other consonant. Multiple changes can be made.</p><p><span class="tex-font-style-bf">In this problem</span>, we consider the letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">i</span>', '<span class="tex-font-style-tt">o</span>' and '<span class="tex-font-style-tt">u</span>' to be vowels and all the other letters to be consonants.</p><p>Given the names of two superheroes, determine if the superhero with name $s$ can be transformed to the Superhero with name $t$.</p></div><div class="input-specification"><p>The first line contains the string $s$ having length between $1$ and $1000$, inclusive.</p><p>The second line contains the string $t$ having length between $1$ and $1000$, inclusive.</p><p>Both strings $s$ and $t$ are guaranteed to be different and consist of lowercase English letters only.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the superhero with name $s$ can be transformed to the superhero with name $t$ and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains the string $s$ having length between $1$ and $1000$, inclusive.</p><p>The second line contains the string $t$ having length between $1$ and $1000$, inclusive.</p><p>Both strings $s$ and $t$ are guaranteed to be different and consist of lowercase English letters only.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the superhero with name $s$ can be transformed to the superhero with name $t$ and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
a
u
```




```input2
abc
ukm
```




```input3
akm
ua
```




```output1
Yes
```




```output2
Yes
```




```output3
No
```



## Note

<p>In the first sample, since both '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">u</span>' are vowels, it is possible to convert string $s$ to $t$.</p><p>In the third sample, '<span class="tex-font-style-tt">k</span>' is a consonant, whereas '<span class="tex-font-style-tt">a</span>' is a vowel, so it is not possible to convert string $s$ to $t$.</p>
