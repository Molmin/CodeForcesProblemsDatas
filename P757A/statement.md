## Description

<div><p>Bash wants to become a Pokemon master one day. Although he liked a lot of Pokemon, he has always been fascinated by Bulbasaur the most. Soon, things started getting serious and his fascination turned into an obsession. Since he is too young to go out and catch Bulbasaur, he came up with his own way of catching a Bulbasaur.</p><p>Each day, he takes the front page of the newspaper. He cuts out the letters one at a time, from anywhere on the front page of the newspaper to form the word <span class="tex-font-style-tt">"Bulbasaur"</span> (without quotes) and sticks it on his wall. Bash is very particular about case&nbsp;— the first letter of <span class="tex-font-style-tt">"Bulbasaur"</span> must be upper case and the rest must be lower case. By doing this he thinks he has caught one Bulbasaur. He then repeats this step on the left over part of the newspaper. He keeps doing this until it is not possible to form the word <span class="tex-font-style-tt">"Bulbasaur"</span> from the newspaper.</p><p>Given the text on the front page of the newspaper, can you tell how many Bulbasaurs he will catch today?</p><p>Note: <span class="tex-font-style-bf">uppercase and lowercase letters are considered different.</span></p></div><div class="input-specification"><p>Input contains a single line containing a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1  ≤  |<i>s</i>|  ≤  10<sup class="upper-index">5</sup></span>)&nbsp;— the text on the front page of the newspaper without spaces and punctuation marks. <span class="tex-span">|<i>s</i>|</span> is the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The string <span class="tex-span"><i>s</i></span> contains lowercase and uppercase English letters, i.e. <img align="middle" class="tex-formula" src="file://FRuBmoGh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Output a single integer, the answer to the problem.</p></div>

## Input

<p>Input contains a single line containing a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1  ≤  |<i>s</i>|  ≤  10<sup class="upper-index">5</sup></span>)&nbsp;— the text on the front page of the newspaper without spaces and punctuation marks. <span class="tex-span">|<i>s</i>|</span> is the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The string <span class="tex-span"><i>s</i></span> contains lowercase and uppercase English letters, i.e. <img align="middle" class="tex-formula" src="file://FRuBmoGh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Output a single integer, the answer to the problem.</p>





```input1
Bulbbasaur

```




```input2
F

```




```input3
aBddulbasaurrgndgbualdBdsagaurrgndbb

```




```output1
1

```




```output2
0

```




```output3
2

```



## Note

<p>In the first case, you could pick: <span class="tex-font-style-tt"><span class="tex-font-style-bf">Bulb</span>b<span class="tex-font-style-bf">asaur</span></span>.</p><p>In the second case, there is no way to pick even a single Bulbasaur.</p><p>In the third case, you can rearrange the string to <span class="tex-font-style-tt"><span class="tex-font-style-bf">BulbasaurBulbasaur</span>addrgndgddgargndbb</span> to get two words "<span class="tex-font-style-tt">Bulbasaur</span>".</p>
