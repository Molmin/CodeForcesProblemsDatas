## Description

<div><p>Vera adores poems. All the poems Vera knows are divided into quatrains (groups of four lines) and in each quatrain some lines contain rhymes.</p><p>Let's consider that all lines in the poems consist of lowercase Latin letters (without spaces). Letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>", "<span class="tex-font-style-tt">i</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">u</span>" are considered vowels.</p><p>Two lines rhyme if their suffixes that start from the <span class="tex-span"><i>k</i></span>-th vowels (counting from the end) match. If a line has less than <span class="tex-span"><i>k</i></span> vowels, then such line can't rhyme with any other line. For example, if <span class="tex-span"><i>k</i> = 1</span>, lines <span class="tex-span"><i>commit</i></span> and <span class="tex-span"><i>hermit</i></span> rhyme (the corresponding suffixes equal <span class="tex-span"><i>it</i></span>), and if <span class="tex-span"><i>k</i> = 2</span>, they do not rhyme (<span class="tex-span"><i>ommit</i> ≠ <i>ermit</i></span>).</p><p>Today on a literature lesson Vera learned that quatrains can contain four different schemes of rhymes, namely the following ones (the same letters stand for rhyming lines): </p><ul> <li> Clerihew (<span class="tex-span"><i>aabb</i></span>); </li><li> Alternating (<span class="tex-span"><i>abab</i></span>); </li><li> Enclosed (<span class="tex-span"><i>abba</i></span>). </li></ul><p>If all lines of a quatrain pairwise rhyme, then the quatrain can belong to any rhyme scheme (this situation is represented by <span class="tex-span"><i>aaaa</i></span>).</p><p>If all quatrains of a poem belong to the same rhyme scheme, then we can assume that the whole poem belongs to this rhyme scheme. If in each quatrain all lines pairwise rhyme, then the rhyme scheme of the poem is <span class="tex-span"><i>aaaa</i></span>. Let us note that it doesn't matter whether lines from different quatrains rhyme with each other or not. In other words, it is possible that different quatrains aren't connected by a rhyme.</p><p>Vera got a long poem as a home task. The girl has to analyse it and find the poem rhyme scheme. Help Vera cope with the task.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2500</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>)&nbsp;— the number of quatrains in the poem and the vowel's number, correspondingly. Next <span class="tex-span">4<i>n</i></span> lines contain the poem. Each line is not empty and only consists of small Latin letters. The total length of the lines does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p>If we assume that the lines are numbered starting from 1, then the first quatrain contains lines number <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>; the second one contains lines number <span class="tex-span">5</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">8</span>; and so on.</p></div><div class="output-specification"><p>Print the rhyme scheme of the poem as "<span class="tex-font-style-tt">aabb</span>", "<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">abba</span>", "<span class="tex-font-style-tt">aaaa</span>"; or "<span class="tex-font-style-tt">NO</span>" if the poem does not belong to any of the above mentioned schemes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2500</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>)&nbsp;— the number of quatrains in the poem and the vowel's number, correspondingly. Next <span class="tex-span">4<i>n</i></span> lines contain the poem. Each line is not empty and only consists of small Latin letters. The total length of the lines does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p>If we assume that the lines are numbered starting from 1, then the first quatrain contains lines number <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>; the second one contains lines number <span class="tex-span">5</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">8</span>; and so on.</p>

## Output

<p>Print the rhyme scheme of the poem as "<span class="tex-font-style-tt">aabb</span>", "<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">abba</span>", "<span class="tex-font-style-tt">aaaa</span>"; or "<span class="tex-font-style-tt">NO</span>" if the poem does not belong to any of the above mentioned schemes.</p>





```input1
1 1
day
may
sun
fun

```




```input2
1 1
day
may
gray
way

```




```input3
2 1
a
a
a
a
a
a
e
e

```




```input4
2 1
day
may
sun
fun
test
hill
fest
thrill

```




```output1
aabb

```




```output2
aaaa

```




```output3
aabb

```




```output4
NO

```



## Note

<p>In the last sample both quatrains have rhymes but finding the common scheme is impossible, so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
