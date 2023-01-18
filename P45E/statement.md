## Description

<div><p>Vasya is a born Berland film director, he is currently working on a new blockbuster, "The Unexpected". Vasya knows from his own experience how important it is to choose the main characters' names and surnames wisely. He made up a list of <span class="tex-span"><i>n</i></span> names and <span class="tex-span"><i>n</i></span> surnames that he wants to use. Vasya haven't decided yet how to call characters, so he is free to match any name to any surname. Now he has to make the list of all the main characters in the following format: "<span class="tex-font-style-tt"><span class="tex-span"><i>Name</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>Surname</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>Name</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>Surname</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>Name</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span"><i>Surname</i><sub class="lower-index"><i>n</i></sub></span></span>", i.e. all the name-surname pairs should be separated by exactly one comma and exactly one space, and the name should be separated from the surname by exactly one space. First of all Vasya wants to maximize the number of the pairs, in which the name and the surname start from one letter. If there are several such variants, Vasya wants to get the lexicographically minimal one. Help him.</p><p>An answer will be verified a line in the format as is shown above, including the needed commas and spaces. It's the lexicographical minimality of such a line that needs to be ensured. The output line <span class="tex-font-style-bf">shouldn't end with a space or with a comma</span>.</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of names and surnames. Then follow <span class="tex-span"><i>n</i></span> lines — the list of names. Then follow <span class="tex-span"><i>n</i></span> lines — the list of surnames. No two from those <span class="tex-span">2<i>n</i></span> strings match. Every name and surname is a non-empty string consisting of no more than 10 Latin letters. It is guaranteed that the first letter is uppercase and the rest are lowercase.</p></div><div class="output-specification"><p>The output data consist of a single line — the needed list. Note that <span class="tex-font-style-bf">one should follow closely</span> the output data format!</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of names and surnames. Then follow <span class="tex-span"><i>n</i></span> lines — the list of names. Then follow <span class="tex-span"><i>n</i></span> lines — the list of surnames. No two from those <span class="tex-span">2<i>n</i></span> strings match. Every name and surname is a non-empty string consisting of no more than 10 Latin letters. It is guaranteed that the first letter is uppercase and the rest are lowercase.</p>

## Output

<p>The output data consist of a single line — the needed list. Note that <span class="tex-font-style-bf">one should follow closely</span> the output data format!</p>





```input1
4
Ann
Anna
Sabrina
John
Petrov
Ivanova
Stoltz
Abacaba

```




```input2
4
Aa
Ab
Ac
Ba
Ad
Ae
Bb
Bc

```




```output1
Ann Abacaba, Anna Ivanova, John Petrov, Sabrina Stoltz
```




```output2
Aa Ad, Ab Ae, Ac Bb, Ba Bc
```


