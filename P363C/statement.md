## Description

<div><p>Many modern text editors automatically check the spelling of the user's text. Some editors even suggest how to correct typos.</p><p>In this problem your task to implement a small functionality to correct two types of typos in a word. We will assume that three identical letters together is a typo (for example, word "<span class="tex-font-style-tt">helllo</span>" contains a typo). Besides, a couple of identical letters immediately followed by another couple of identical letters is a typo too (for example, words "<span class="tex-font-style-tt">helloo</span>" and "<span class="tex-font-style-tt">wwaatt</span>" contain typos).</p><p>Write a code that deletes the minimum number of letters from a word, correcting described typos in the word. You are allowed to delete letters from both ends and from the middle of the word.</p></div><div class="input-specification"><p>The single line of the input contains word <span class="tex-span"><i>s</i></span>, its length is from 1 to 200000 characters. The given word <span class="tex-span"><i>s</i></span> consists of lowercase English letters.</p></div><div class="output-specification"><p>Print such word <span class="tex-span"><i>t</i></span> that it doesn't contain any typos described in the problem statement and is obtained from <span class="tex-span"><i>s</i></span> by deleting the least number of letters.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The single line of the input contains word <span class="tex-span"><i>s</i></span>, its length is from 1 to 200000 characters. The given word <span class="tex-span"><i>s</i></span> consists of lowercase English letters.</p>

## Output

<p>Print such word <span class="tex-span"><i>t</i></span> that it doesn't contain any typos described in the problem statement and is obtained from <span class="tex-span"><i>s</i></span> by deleting the least number of letters.</p><p>If there are multiple solutions, print any of them.</p>





```input1
helloo

```




```input2
woooooow

```




```output1
hello

```




```output2
woow

```



## Note

<p>The second valid answer to the test from the statement is "<span class="tex-font-style-tt">heloo</span>".</p>
