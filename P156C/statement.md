## Description

<div><p>Sherlock Holmes found a mysterious correspondence of two VIPs and made up his mind to read it. But there is a problem! The correspondence turned out to be encrypted. The detective tried really hard to decipher the correspondence, but he couldn't understand anything. </p><p>At last, after some thought, he thought of something. Let's say there is a word <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span">|<i>s</i>|</span> lowercase Latin letters. Then for one <span class="tex-font-style-underline">operation</span> you can choose a certain position <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> &lt; |<i>s</i>|</span>) and perform one of the following actions: </p><ul> <li> either replace letter <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i></sub></span> with the one that alphabetically <span class="tex-font-style-bf">follows</span> it and replace letter <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i> + 1</sub></span> with the one that alphabetically <span class="tex-font-style-bf">precedes</span> it; </li><li> or replace letter <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i></sub></span> with the one that alphabetically <span class="tex-font-style-bf">precedes</span> it and replace letter <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i> + 1</sub></span> with the one that alphabetically <span class="tex-font-style-bf">follows</span> it. </li></ul><p>Let us note that letter "<span class="tex-font-style-tt">z</span>" doesn't have a defined following letter and letter "<span class="tex-font-style-tt">a</span>" doesn't have a defined preceding letter. That's why the corresponding changes are not acceptable. If the operation requires performing at least one unacceptable change, then such operation cannot be performed.</p><p>Two words <span class="tex-font-style-underline">coincide in their meaning</span> iff one of them can be transformed into the other one as a result of zero or more operations.</p><p>Sherlock Holmes needs to learn to quickly determine the following for each word: how many words can exist that coincide in their meaning with the given word, but differs from the given word in at least one character? Count this number for him modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The input data contains several tests. The first line contains the only integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of tests.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain the words, one per line. Each word consists of lowercase Latin letters and has length from <span class="tex-span">1</span> to <span class="tex-span">100</span>, inclusive. Lengths of words can differ.</p></div><div class="output-specification"><p>For each word you should print the number of different <span class="tex-font-style-bf">other</span> words that coincide with it in their meaning — not from the words listed in the input data, but from all possible words. As the sought number can be very large, print its value modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The input data contains several tests. The first line contains the only integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of tests.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain the words, one per line. Each word consists of lowercase Latin letters and has length from <span class="tex-span">1</span> to <span class="tex-span">100</span>, inclusive. Lengths of words can differ.</p>

## Output

<p>For each word you should print the number of different <span class="tex-font-style-bf">other</span> words that coincide with it in their meaning — not from the words listed in the input data, but from all possible words. As the sought number can be very large, print its value modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1
ab

```




```input2
1
aaaaaaaaaaa

```




```input3
2
ya
klmbfxzb

```




```output1
1

```




```output2
0

```




```output3
24
320092793

```



## Note

<p>Some explanations about the <span class="tex-font-style-underline">operation</span>:</p><ul> <li> Note that for each letter, we can clearly define the letter that follows it. Letter "<span class="tex-font-style-tt">b</span>" alphabetically follows letter "<span class="tex-font-style-tt">a</span>", letter "<span class="tex-font-style-tt">c</span>" follows letter "<span class="tex-font-style-tt">b</span>", ..., "<span class="tex-font-style-tt">z</span>" follows letter "<span class="tex-font-style-tt">y</span>". </li><li> Preceding letters are defined in the similar manner: letter "<span class="tex-font-style-tt">y</span>" precedes letter "<span class="tex-font-style-tt">z</span>", ..., "<span class="tex-font-style-tt">a</span>" precedes letter "<span class="tex-font-style-tt">b</span>". </li><li> Note that the operation never changes a word's length. </li></ul><p>In the first sample you can obtain the only other word "<span class="tex-font-style-tt">ba</span>". In the second sample you cannot obtain any other word, so the correct answer is <span class="tex-span">0</span>.</p><p>Consider the third sample. One operation can transform word "<span class="tex-font-style-tt">klmbfxzb</span>" into word "<span class="tex-font-style-tt">klmcexzb</span>": we should choose <span class="tex-span"><i>p</i> = 4</span>, and replace the fourth letter with the following one ("<span class="tex-font-style-tt">b</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">c</span>"), and the fifth one — with the preceding one ("<span class="tex-font-style-tt">f</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">e</span>"). Also, we can obtain many other words from this one. An operation can transform word "<span class="tex-font-style-tt">ya</span>" only into one other word "<span class="tex-font-style-tt">xb</span>". </p><p>Word "<span class="tex-font-style-tt">ya</span>" coincides in its meaning with words "<span class="tex-font-style-tt">xb</span>", "<span class="tex-font-style-tt">wc</span>", "<span class="tex-font-style-tt">vd</span>", ..., "<span class="tex-font-style-tt">ay</span>" (overall there are <span class="tex-span">24</span> other words). The word "<span class="tex-font-style-tt">klmbfxzb</span> has many more variants — there are <span class="tex-span">3320092814</span> other words that coincide with in the meaning. So the answer for the first word equals <span class="tex-span">24</span> and for the second one equals <span class="tex-span">320092793</span> — the number <span class="tex-span">3320092814</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span></p>
