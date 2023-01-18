## Description

<div><p>Vasya decided to write an anonymous letter cutting the letters out of a newspaper heading. He knows heading <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and text <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> that he wants to send. Vasya can use every single heading letter no more than once. Vasya doesn't have to cut the spaces out of the heading — he just leaves some blank space to mark them. Help him; find out if he will manage to compose the needed text.</p></div><div class="input-specification"><p>The first line contains a newspaper heading <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>. The second line contains the letter text <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> и <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> are non-empty lines consisting of spaces, uppercase and lowercase Latin letters, whose lengths do not exceed 200 symbols. The uppercase and lowercase letters should be differentiated. Vasya does not cut spaces out of the heading.</p></div><div class="output-specification"><p>If Vasya can write the given anonymous letter, print <span class="tex-font-style-tt">YES</span>, otherwise print <span class="tex-font-style-tt">NO</span></p></div>

## Input

<p>The first line contains a newspaper heading <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>. The second line contains the letter text <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> и <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> are non-empty lines consisting of spaces, uppercase and lowercase Latin letters, whose lengths do not exceed 200 symbols. The uppercase and lowercase letters should be differentiated. Vasya does not cut spaces out of the heading.</p>

## Output

<p>If Vasya can write the given anonymous letter, print <span class="tex-font-style-tt">YES</span>, otherwise print <span class="tex-font-style-tt">NO</span></p>





```input1
Instead of dogging Your footsteps it disappears but you dont notice anything
where is your dog

```




```input2
Instead of dogging Your footsteps it disappears but you dont notice anything
Your dog is upstears

```




```input3
Instead of dogging your footsteps it disappears but you dont notice anything
Your dog is upstears

```




```input4
abcdefg hijk
k j i h g f e d c b a

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




```output4
YES

```


