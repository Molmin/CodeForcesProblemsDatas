## Description

<div><p>Little Nastya has a hobby, she likes to remove some letters from word, to obtain another word. But it turns out to be pretty hard for her, because she is too young. Therefore, her brother Sergey always helps her.</p><p>Sergey gives Nastya the word <span class="tex-span"><i>t</i></span> and wants to get the word <span class="tex-span"><i>p</i></span> out of it. Nastya removes letters in a certain order (one after another, in this order strictly), which is specified by permutation of letters' indices of the word <span class="tex-span"><i>t</i></span>: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>... <i>a</i><sub class="lower-index">|<i>t</i>|</sub></span>. We denote the length of word <span class="tex-span"><i>x</i></span> as <span class="tex-span">|<i>x</i>|</span>. Note that after removing one letter, the indices of other letters don't change. For example, if <span class="tex-span"><i>t</i> = </span>"<span class="tex-font-style-tt">nastya</span>" and <span class="tex-span"><i>a</i> = [4, 1, 5, 3, 2, 6]</span> then removals make the following sequence of words "<span class="tex-font-style-tt">nastya</span>" <img align="middle" class="tex-formula" src="file://wjkCnnqV.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">nas<span class="tex-font-style-striked">t</span>ya</span>" <img align="middle" class="tex-formula" src="file://0cnCHWWS.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-striked">n</span>as<span class="tex-font-style-striked">t</span>ya</span>" <img align="middle" class="tex-formula" src="file://qKEhLihq.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-striked">n</span>as<span class="tex-font-style-striked">t</span><span class="tex-font-style-striked">y</span>a</span>" <img align="middle" class="tex-formula" src="file://xcbRRuTA.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-striked">n</span>a<span class="tex-font-style-striked">s</span><span class="tex-font-style-striked">t</span><span class="tex-font-style-striked">y</span>a</span>" <img align="middle" class="tex-formula" src="file://U8PHq4vN.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-striked">n</span><span class="tex-font-style-striked">a</span><span class="tex-font-style-striked">s</span><span class="tex-font-style-striked">t</span><span class="tex-font-style-striked">y</span>a</span>" <img align="middle" class="tex-formula" src="file://iVyUWUwx.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-striked">n</span><span class="tex-font-style-striked">a</span><span class="tex-font-style-striked">s</span><span class="tex-font-style-striked">t</span><span class="tex-font-style-striked">y</span><span class="tex-font-style-striked">a</span></span>".</p><p>Sergey knows this permutation. His goal is to stop his sister at some point and continue removing by himself to get the word <span class="tex-span"><i>p</i></span>. Since Nastya likes this activity, Sergey wants to stop her as late as possible. Your task is to determine, how many letters Nastya can remove before she will be stopped by Sergey.</p><p>It is guaranteed that the word <span class="tex-span"><i>p</i></span> can be obtained by removing the letters from word <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first and second lines of the input contain the words <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>p</i></span>, respectively. Words are composed of lowercase letters of the Latin alphabet (<span class="tex-span">1 ≤ |<i>p</i>| &lt; |<i>t</i>| ≤ 200 000</span>). It is guaranteed that the word <span class="tex-span"><i>p</i></span> can be obtained by removing the letters from word <span class="tex-span"><i>t</i></span>.</p><p>Next line contains a permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">|<i>t</i>|</sub></span> of letter indices that specifies the order in which Nastya removes letters of <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>t</i>|</span>, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct).</p></div><div class="output-specification"><p>Print a single integer number, the maximum number of letters that Nastya can remove.</p></div>

## Input

<p>The first and second lines of the input contain the words <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>p</i></span>, respectively. Words are composed of lowercase letters of the Latin alphabet (<span class="tex-span">1 ≤ |<i>p</i>| &lt; |<i>t</i>| ≤ 200 000</span>). It is guaranteed that the word <span class="tex-span"><i>p</i></span> can be obtained by removing the letters from word <span class="tex-span"><i>t</i></span>.</p><p>Next line contains a permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">|<i>t</i>|</sub></span> of letter indices that specifies the order in which Nastya removes letters of <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>t</i>|</span>, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct).</p>

## Output

<p>Print a single integer number, the maximum number of letters that Nastya can remove.</p>





```input1
ababcba
abb
5 3 4 1 7 6 2

```




```input2
bbbabb
bb
1 6 3 4 2 5

```




```output1
3
```




```output2
4
```



## Note

<p>In the first sample test sequence of removing made by Nastya looks like this:</p><p>"<span class="tex-font-style-tt">ababcba</span>" <img align="middle" class="tex-formula" src="file://CVNmmfVm.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">abab<span class="tex-font-style-striked">c</span>ba</span>" <img align="middle" class="tex-formula" src="file://EDUwB1wT.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">ab<span class="tex-font-style-striked">a</span>b<span class="tex-font-style-striked">c</span>ba</span>" <img align="middle" class="tex-formula" src="file://hQMK2XYp.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">ab<span class="tex-font-style-striked">a</span><span class="tex-font-style-striked">b</span><span class="tex-font-style-striked">c</span>ba</span>" </p><p>Nastya can not continue, because it is impossible to get word "<span class="tex-font-style-tt">abb</span>" from word "<span class="tex-font-style-tt"><span class="tex-font-style-striked">a</span>b<span class="tex-font-style-striked">a</span><span class="tex-font-style-striked">b</span><span class="tex-font-style-striked">c</span>ba</span>".</p><p>So, Nastya will remove only three letters.</p>
