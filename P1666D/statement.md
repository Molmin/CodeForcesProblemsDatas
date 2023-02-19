## Description

<div><p>Daisy loves playing games with words. Recently, she has been playing the following Deletive Editing word game with Daniel. </p><p>Daisy picks a word, for example, "<span class="tex-font-style-tt">DETERMINED</span>". On each game turn, Daniel calls out a letter, for example, '<span class="tex-font-style-tt">E</span>', and Daisy removes <span class="tex-font-style-bf">the first occurrence</span> of this letter from the word, getting "<span class="tex-font-style-tt">DTERMINED</span>". On the next turn, Daniel calls out a letter again, for example, '<span class="tex-font-style-tt">D</span>', and Daisy removes its first occurrence, getting "<span class="tex-font-style-tt">TERMINED</span>". They continue with '<span class="tex-font-style-tt">I</span>', getting "<span class="tex-font-style-tt">TERMNED</span>", with '<span class="tex-font-style-tt">N</span>', getting "<span class="tex-font-style-tt">TERMED</span>", and with '<span class="tex-font-style-tt">D</span>', getting "<span class="tex-font-style-tt">TERME</span>". Now, if Daniel calls out the letter '<span class="tex-font-style-tt">E</span>', Daisy gets "<span class="tex-font-style-tt">TRME</span>", but there is no way she can get the word "<span class="tex-font-style-tt">TERM</span>" if they start playing with the word "<span class="tex-font-style-tt">DETERMINED</span>".</p><p>Daisy is curious if she can get the final word of her choice, starting from the given initial word, by playing this game for zero or more turns. Your task it help her to figure this out.</p></div><div class="input-specification"><p>The first line of the input contains an integer $n$&nbsp;— the number of test cases ($1 \le n \le 10\,000$). The following $n$ lines contain test cases. </p><p>Each test case consists of two words $s$ and $t$ separated by a space. Each word consists of at least one and at most 30 uppercase English letters; $s$ is the Daisy's initial word for the game; $t$ is the final word that Daisy would like to get at the end of the game.</p></div><div class="output-specification"><p>Output $n$ lines to the output&nbsp;— a single line for each test case. Output "<span class="tex-font-style-tt">YES</span>" if it is possible for Daisy to get from the initial word $s$ to the final word $t$ by playing the Deletive Editing game. Output "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains an integer $n$&nbsp;— the number of test cases ($1 \le n \le 10\,000$). The following $n$ lines contain test cases. </p><p>Each test case consists of two words $s$ and $t$ separated by a space. Each word consists of at least one and at most 30 uppercase English letters; $s$ is the Daisy's initial word for the game; $t$ is the final word that Daisy would like to get at the end of the game.</p>

## Output

<p>Output $n$ lines to the output&nbsp;— a single line for each test case. Output "<span class="tex-font-style-tt">YES</span>" if it is possible for Daisy to get from the initial word $s$ to the final word $t$ by playing the Deletive Editing game. Output "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
6
DETERMINED TRME
DETERMINED TERM
PSEUDOPSEUDOHYPOPARATHYROIDISM PEPA
DEINSTITUTIONALIZATION DONATION
CONTEST CODE
SOLUTION SOLUTION
```




```output1
YES
NO
NO
YES
NO
YES
```


