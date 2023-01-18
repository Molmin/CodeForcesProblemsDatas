## Description

<div><p><span class="tex-font-style-it">All of us know that girls in Arpa’s land are... ok, you’ve got the idea :D</span></p><p>Anyone knows that Arpa isn't a normal man, he is ... well, sorry, I can't explain it more. Mehrdad is interested about the reason, so he asked Sipa, one of the best biology scientists in Arpa's land, for help. Sipa has a DNA editor.</p><center> <img class="tex-graphics" height="222px" src="file://RhdlJHyW.png" style="max-width: 100.0%;max-height: 100.0%;" width="280px"> </center><p>Sipa put Arpa under the DNA editor. DNA editor showed Arpa's DNA as a string <span class="tex-span"><i>S</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters. Also Sipa has another DNA <span class="tex-span"><i>T</i></span> consisting of lowercase English letters that belongs to a normal man.</p><p>Now there are <span class="tex-span">(<i>n</i> + 1)</span> options to change Arpa's DNA, numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span>. <span class="tex-span"><i>i</i></span>-th of them is to put <span class="tex-span"><i>T</i></span> between <span class="tex-span"><i>i</i></span>-th and <span class="tex-span">(<i>i</i> + 1)</span>-th characters of <span class="tex-span"><i>S</i></span> (<span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i></span>). If <span class="tex-span"><i>i</i> = 0</span>, <span class="tex-span"><i>T</i></span> will be put before <span class="tex-span"><i>S</i></span>, and if <span class="tex-span"><i>i</i> = <i>n</i></span>, it will be put after <span class="tex-span"><i>S</i></span>.</p><p>Mehrdad wants to choose the most <span class="tex-font-style-it">interesting</span> option for Arpa's DNA among these <span class="tex-span"><i>n</i> + 1</span> options. DNA <span class="tex-span"><i>A</i></span> is more <span class="tex-font-style-it">interesting</span> than <span class="tex-span"><i>B</i></span> if <span class="tex-span"><i>A</i></span> is lexicographically smaller than <span class="tex-span"><i>B</i></span>. Mehrdad asked Sipa <span class="tex-span"><i>q</i></span> questions: </p><p>Given integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>k</i>, <i>x</i>, <i>y</i></span>, what is the most interesting option if we only consider such options <span class="tex-span"><i>i</i></span> that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> and <img align="middle" class="tex-formula" src="file://Tiku4EH5.png" style="max-width: 100.0%;max-height: 100.0%;">? If there are several most interesting options, Mehrdad wants to know one with the smallest number <span class="tex-span"><i>i</i></span>.</p><p>Since Sipa is a biology scientist but not a programmer, you should help him.</p></div><div class="input-specification"><p>The first line contains strings <span class="tex-span"><i>S</i></span>, <span class="tex-span"><i>T</i></span> and integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ |<i>S</i>|, |<i>T</i>|, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— Arpa's DNA, the DNA of a normal man, and the number of Mehrdad's questions. The strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> consist only of small English letters.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the Mehrdad's questions. Each of these lines contain five integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>k</i>, <i>x</i>, <i>y</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ <i>y</i> &lt; <i>k</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers. The <span class="tex-span"><i>j</i></span>-th of them should be the number <span class="tex-span"><i>i</i></span> of the most interesting option among those that satisfy the conditions of the <span class="tex-span"><i>j</i></span>-th question. If there is no option <span class="tex-span"><i>i</i></span> satisfying the conditions in some question, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains strings <span class="tex-span"><i>S</i></span>, <span class="tex-span"><i>T</i></span> and integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ |<i>S</i>|, |<i>T</i>|, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— Arpa's DNA, the DNA of a normal man, and the number of Mehrdad's questions. The strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> consist only of small English letters.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the Mehrdad's questions. Each of these lines contain five integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>k</i>, <i>x</i>, <i>y</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ <i>y</i> &lt; <i>k</i></span>).</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers. The <span class="tex-span"><i>j</i></span>-th of them should be the number <span class="tex-span"><i>i</i></span> of the most interesting option among those that satisfy the conditions of the <span class="tex-span"><i>j</i></span>-th question. If there is no option <span class="tex-span"><i>i</i></span> satisfying the conditions in some question, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
abc d 4
0 3 2 0 0
0 3 1 0 0
1 2 1 0 0
0 1 3 2 2

```




```input2
abbbbbbaaa baababaaab 10
1 2 1 0 0
2 7 8 4 7
2 3 9 2 8
3 4 6 1 1
0 8 5 2 4
2 8 10 4 7
7 10 1 0 0
1 4 6 0 2
0 9 8 0 6
4 8 5 0 1

```




```output1
2 3 2 -1 

```




```output2
1 4 2 -1 2 4 10 1 1 5 

```



## Note

<p>Explanation of first sample case:</p><p>In the first question Sipa has two options: <span class="tex-font-style-tt">dabc</span> (<span class="tex-span"><i>i</i> = 0</span>) and <span class="tex-font-style-tt">abdc</span> (<span class="tex-span"><i>i</i> = 2</span>). The latter (<span class="tex-font-style-tt">abcd</span>) is better than <span class="tex-font-style-tt">abdc</span>, so answer is <span class="tex-span">2</span>.</p><p>In the last question there is no <span class="tex-span"><i>i</i></span> such that <span class="tex-span">0 ≤ <i>i</i> ≤ 1</span> and <img align="middle" class="tex-formula" src="file://gvPExnlq.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
