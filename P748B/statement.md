## Description

<div><p>Santa Claus decided to disassemble his keyboard to clean it. After he returned all the keys back, he suddenly realized that some pairs of keys took each other's place! That is, Santa suspects that each key is either on its place, or on the place of another key, which is located exactly where the first key should be. </p><p>In order to make sure that he's right and restore the correct order of keys, Santa typed his favorite patter looking only to his keyboard.</p><p>You are given the Santa's favorite patter and the string he actually typed. Determine which pairs of keys could be mixed. Each key must occur in pairs <span class="tex-font-style-bf">at most once</span>.</p></div><div class="input-specification"><p>The input consists of only two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> denoting the favorite Santa's patter and the resulting string. <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are not empty and have the same length, which is at most <span class="tex-span">1000</span>. Both strings consist only of lowercase English letters.</p></div><div class="output-specification"><p>If Santa is wrong, and there is no way to divide some of keys into pairs and swap keys in each pair so that the keyboard will be fixed, print «<span class="tex-font-style-tt">-1</span>» (without quotes).</p><p>Otherwise, the first line of output should contain the only integer <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 0</span>)&nbsp;— the number of pairs of keys that should be swapped. The following <span class="tex-span"><i>k</i></span> lines should contain two space-separated letters each, denoting the keys which should be swapped. All printed letters must be distinct.</p><p>If there are several possible answers, print any of them. You are free to choose the order of the pairs and the order of keys in a pair.</p><p>Each letter must occur at most once. Santa considers the keyboard to be fixed if he can print his favorite patter without mistakes.</p></div>

## Input

<p>The input consists of only two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> denoting the favorite Santa's patter and the resulting string. <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are not empty and have the same length, which is at most <span class="tex-span">1000</span>. Both strings consist only of lowercase English letters.</p>

## Output

<p>If Santa is wrong, and there is no way to divide some of keys into pairs and swap keys in each pair so that the keyboard will be fixed, print «<span class="tex-font-style-tt">-1</span>» (without quotes).</p><p>Otherwise, the first line of output should contain the only integer <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 0</span>)&nbsp;— the number of pairs of keys that should be swapped. The following <span class="tex-span"><i>k</i></span> lines should contain two space-separated letters each, denoting the keys which should be swapped. All printed letters must be distinct.</p><p>If there are several possible answers, print any of them. You are free to choose the order of the pairs and the order of keys in a pair.</p><p>Each letter must occur at most once. Santa considers the keyboard to be fixed if he can print his favorite patter without mistakes.</p>





```input1
helloworld
ehoolwlroz

```




```input2
hastalavistababy
hastalavistababy

```




```input3
merrychristmas
christmasmerry

```




```output1
3
h e
l o
d z

```




```output2
0

```




```output3
-1

```


