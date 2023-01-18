## Description

<div><p>Peterson loves to learn new languages, but his favorite hobby is making new ones. Language is a set of words, and word is a sequence of lowercase Latin letters.</p><p>Peterson makes new language every morning. It is difficult task to store the whole language, so Peterson have invented new data structure for storing his languages which is called <span class="tex-font-style-underline">broom</span>. Broom is rooted tree with edges marked with letters. Initially broom is represented by the only vertex&nbsp;— the root of the broom. When Peterson wants to add new word to the language he stands at the root and processes the letters of new word one by one. Consider that Peterson stands at the vertex <span class="tex-span"><i>u</i></span>. If there is an edge from <span class="tex-span"><i>u</i></span> marked with current letter, Peterson goes through this edge. Otherwise Peterson adds new edge from <span class="tex-span"><i>u</i></span> to the new vertex <span class="tex-span"><i>v</i></span>, marks it with the current letter and goes through the new edge. Size of broom is the number of vertices in it.</p><p>In the evening after working day Peterson can't understand the language he made this morning. It is too difficult for bored Peterson and he tries to make it simpler. Simplification of the language is the process of erasing some letters from some words of this language. Formally, Peterson takes some positive integer <span class="tex-span"><i>p</i></span> and erases <span class="tex-span"><i>p</i></span>-th letter from all the words of this language having length at least <span class="tex-span"><i>p</i></span>. Letters in words are indexed starting by 1. Peterson considers that simplification should change at least one word, i.e. there has to be at least one word of length at least <span class="tex-span"><i>p</i></span>. Peterson tries to make his language as simple as possible, so he wants to choose <span class="tex-span"><i>p</i></span> such that the size of the broom for his simplified language is as small as possible.</p><p>Peterson is pretty annoyed with this task so he asks you for help. Write a program to find the smallest possible size of the broom and integer <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the broom.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the broom: <span class="tex-span"><i>i</i></span>-th of them contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and letter <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— describing the edge from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> marked with letter <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are lowercase latin letters. Vertex 1 is the root of the broom.</p><p>Edges describe correct broom which is made from Peterson's language.</p></div><div class="output-specification"><p>The first line of output should contain the minimum possible size of the broom after its simplification. The second line of output should contain integer <span class="tex-span"><i>p</i></span> to choose. If there are several suitable <span class="tex-span"><i>p</i></span> values, print the smallest one.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the broom.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the broom: <span class="tex-span"><i>i</i></span>-th of them contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and letter <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— describing the edge from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> marked with letter <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are lowercase latin letters. Vertex 1 is the root of the broom.</p><p>Edges describe correct broom which is made from Peterson's language.</p>

## Output

<p>The first line of output should contain the minimum possible size of the broom after its simplification. The second line of output should contain integer <span class="tex-span"><i>p</i></span> to choose. If there are several suitable <span class="tex-span"><i>p</i></span> values, print the smallest one.</p>





```input1
5
1 2 c
2 3 a
3 4 t
2 5 t

```




```input2
16
1 2 o
2 3 f
1 4 p
4 5 i
5 6 e
6 7 c
7 8 e
4 9 r
9 10 e
10 11 t
11 12 t
12 13 y
10 14 f
14 15 i
15 16 x

```




```output1
3
2

```




```output2
12
2

```



## Note

<p><img class="tex-graphics" src="file://Vbo1UyUc.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Broom from the second sample test can be built using language "piece", "of", "pie", "pretty", "prefix". Its simplification with <span class="tex-span"><i>p</i> = 2</span> obtains the language of words "pece", "o", "pe", "petty", "pefix". This language gives us the broom with minimum possible size.</p>
