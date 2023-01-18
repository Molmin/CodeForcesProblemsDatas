## Description

<div><p>You are given $n$ words, each of which consists of lowercase alphabet letters. Each word <span class="tex-font-style-bf">contains at least</span> one vowel. You are going to choose some of the given words and make as many beautiful lyrics as possible.</p><p>Each <span class="tex-font-style-it">lyric</span> consists of two lines. Each <span class="tex-font-style-it">line</span> consists of two words separated by whitespace. </p><p>A lyric is <span class="tex-font-style-it">beautiful</span> if and only if it satisfies all conditions below. </p><ul> <li> The number of vowels in the first word of the first line is the same as the number of vowels in the first word of the second line. </li><li> The number of vowels in the second word of the first line is the same as the number of vowels in the second word of the second line. </li><li> The last vowel of the first line is the same as the last vowel of the second line. Note that there may be consonants after the vowel. </li></ul><p>Also, letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">i</span>", and "<span class="tex-font-style-tt">u</span>" are vowels. Note that "<span class="tex-font-style-tt">y</span>" is <span class="tex-font-style-bf">never</span> vowel.</p><p>For example of a beautiful lyric, </p><center> "<span class="tex-font-style-tt">hello hellooowww</span>" <p>"<span class="tex-font-style-tt">whatsup yowowowow</span>" </p></center> is a beautiful lyric because there are two vowels each in "<span class="tex-font-style-tt">hello</span>" and "<span class="tex-font-style-tt">whatsup</span>", four vowels each in "<span class="tex-font-style-tt">hellooowww</span>" and "<span class="tex-font-style-tt">yowowowow</span>" (keep in mind that "<span class="tex-font-style-tt">y</span>" is not a vowel), and the last vowel of each line is "<span class="tex-font-style-tt">o</span>".<p>For example of a not beautiful lyric, </p><center> "<span class="tex-font-style-tt">hey man</span>"<p>"<span class="tex-font-style-tt">iam mcdic</span>" </p></center> is not a beautiful lyric because "<span class="tex-font-style-tt">hey</span>" and "<span class="tex-font-style-tt">iam</span>" don't have same number of vowels and the last vowels of two lines are different ("<span class="tex-font-style-tt">a</span>" in the first and "<span class="tex-font-style-tt">i</span>" in the second).<p>How many beautiful lyrics can you write from given words? Note that you cannot use a word more times than it is given to you. For example, if a word is given three times, you can use it at most three times.</p></div><div class="input-specification"><p>The first line contains single integer $n$ ($1 \le n \le 10^{5}$)&nbsp;— the number of words.</p><p>The $i$-th of the next $n$ lines contains string $s_{i}$ consisting lowercase alphabet letters&nbsp;— the $i$-th word. It is guaranteed that the sum of the total word length is equal or less than $10^{6}$. Each word contains at least one vowel.</p></div><div class="output-specification"><p>In the first line, print $m$&nbsp;— the number of maximum possible beautiful lyrics.</p><p>In next $2m$ lines, print $m$ beautiful lyrics (two lines per lyric).</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains single integer $n$ ($1 \le n \le 10^{5}$)&nbsp;— the number of words.</p><p>The $i$-th of the next $n$ lines contains string $s_{i}$ consisting lowercase alphabet letters&nbsp;— the $i$-th word. It is guaranteed that the sum of the total word length is equal or less than $10^{6}$. Each word contains at least one vowel.</p>

## Output

<p>In the first line, print $m$&nbsp;— the number of maximum possible beautiful lyrics.</p><p>In next $2m$ lines, print $m$ beautiful lyrics (two lines per lyric).</p><p>If there are multiple answers, print any.</p>





```input1
14
wow
this
is
the
first
mcdics
codeforces
round
hooray
i
am
proud
about
that
```




```input2
7
arsijo
suggested
the
idea
for
this
problem
```




```input3
4
same
same
same
differ
```




```output1
3
about proud
hooray round
wow first
this is
i that
mcdics am
```




```output2
0
```




```output3
1
same differ
same same
```



## Note

<p>In the first example, those beautiful lyrics are one of the possible answers. Let's look at the first lyric on the sample output of the first example. "<span class="tex-font-style-tt">about proud hooray round</span>" forms a beautiful lyric because "<span class="tex-font-style-tt">about</span>" and "<span class="tex-font-style-tt">hooray</span>" have same number of vowels, "<span class="tex-font-style-tt">proud</span>" and "<span class="tex-font-style-tt">round</span>" have same number of vowels, and both lines have same last vowel. On the other hand, you cannot form any beautiful lyric with the word "<span class="tex-font-style-tt">codeforces</span>".</p><p>In the second example, you cannot form any beautiful lyric from given words.</p><p>In the third example, you can use the word "<span class="tex-font-style-tt">same</span>" up to three times.</p>
