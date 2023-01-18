## Description

<div><p>The country of Reberland is the archenemy of Berland. Recently the authorities of Berland arrested a Reberlandian spy who tried to bring the leaflets intended for agitational propaganda to Berland illegally . The most leaflets contain substrings of the Absolutely Inadmissible Swearword and maybe even the whole word.</p><p>Berland legal system uses the difficult algorithm in order to determine the guilt of the spy. The main part of this algorithm is the following procedure.</p><p>All the <span class="tex-span"><i>m</i></span> leaflets that are brought by the spy are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. After that it's needed to get the answer to <span class="tex-span"><i>q</i></span> queries of the following kind: "<span class="tex-font-style-it">In which leaflet in the segment of numbers <span class="tex-span">[<i>l</i>, <i>r</i>]</span> the substring of the Absolutely Inadmissible Swearword <span class="tex-span">[<i>p</i><sub class="lower-index"><i>l</i></sub>, <i>p</i><sub class="lower-index"><i>r</i></sub>]</span> occurs more often?</span>".</p><p>The expert wants you to automate that procedure because this time texts of leaflets are too long. Help him!</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5·10<sup class="upper-index">5</sup></span>) — the Absolutely Inadmissible Swearword. The string <span class="tex-span"><i>s</i></span> consists of only lowercase English letters.</p><p>The second line contains the only integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of texts of leaflets for expertise.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the only string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the text of the <span class="tex-span"><i>i</i></span>-th leaflet. The sum of lengths of all leaflet texts doesn't exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>. The text of the leaflets consists of only lowercase English letters.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of queries for expertise.</p><p>Finally, each of the last <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>r</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i>, 1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>p</i><sub class="lower-index"><i>r</i></sub> ≤ |<i>s</i>|</span>), where <span class="tex-span">|<i>s</i>|</span> is the length of the Absolutely Inadmissible Swearword.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers — the number of the text with the most occurences and the number of occurences of the substring <span class="tex-span">[<i>p</i><sub class="lower-index"><i>l</i></sub>, <i>p</i><sub class="lower-index"><i>r</i></sub>]</span> of the string <span class="tex-span"><i>s</i></span>. If there are several text numbers print the smallest one.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5·10<sup class="upper-index">5</sup></span>) — the Absolutely Inadmissible Swearword. The string <span class="tex-span"><i>s</i></span> consists of only lowercase English letters.</p><p>The second line contains the only integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of texts of leaflets for expertise.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the only string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the text of the <span class="tex-span"><i>i</i></span>-th leaflet. The sum of lengths of all leaflet texts doesn't exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>. The text of the leaflets consists of only lowercase English letters.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of queries for expertise.</p><p>Finally, each of the last <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>r</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i>, 1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>p</i><sub class="lower-index"><i>r</i></sub> ≤ |<i>s</i>|</span>), where <span class="tex-span">|<i>s</i>|</span> is the length of the Absolutely Inadmissible Swearword.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers — the number of the text with the most occurences and the number of occurences of the substring <span class="tex-span">[<i>p</i><sub class="lower-index"><i>l</i></sub>, <i>p</i><sub class="lower-index"><i>r</i></sub>]</span> of the string <span class="tex-span"><i>s</i></span>. If there are several text numbers print the smallest one.</p>





```input1
suffixtree
3
suffixtreesareawesome
cartesiantreeisworsethansegmenttree
nyeeheeheee
2
1 2 1 10
1 3 9 10

```




```output1
1 1
3 4

```


