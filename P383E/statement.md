## Description

<div><p>Iahubina is tired of so many complicated languages, so she decided to invent a new, simple language. She already made a dictionary consisting of <span class="tex-span"><i>n</i></span> 3-words. A 3-word is a sequence of exactly <span class="tex-span">3</span> lowercase letters of the first 24 letters of the English alphabet (<span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>x</i></span>). She decided that some of the letters are vowels, and all the others are consonants. The whole language is based on a simple rule: any word that contains at least one vowel is <span class="tex-font-style-it">correct</span>.</p><p>Iahubina forgot which letters are the vowels, and wants to find some possible correct sets of vowels. She asks Iahub questions. In each question, she will give Iahub a set of letters considered vowels (in this question). For each question she wants to know how many words of the dictionary are correct, considering the given set of vowels.</p><p>Iahubina wants to know the <span class="tex-span"><i>xor</i></span> of the squared answers to all the possible questions. There are <span class="tex-span">2<sup class="upper-index">24</sup></span> different questions, they are all subsets of the set of the first 24 letters of the English alphabet. Help Iahub find that number.</p></div><div class="input-specification"><p>The first line contains one integer, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains a 3-word consisting of <span class="tex-span">3</span> lowercase letters. There will be no two identical 3-words.</p></div><div class="output-specification"><p>Print one number, the <span class="tex-span"><i>xor</i></span> of the squared answers to the queries.</p></div>

## Input

<p>The first line contains one integer, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains a 3-word consisting of <span class="tex-span">3</span> lowercase letters. There will be no two identical 3-words.</p>

## Output

<p>Print one number, the <span class="tex-span"><i>xor</i></span> of the squared answers to the queries.</p>





```input1
5
abc
aaa
ada
bcd
def

```




```output1
0

```


