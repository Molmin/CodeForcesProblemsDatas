## Description

<div><p>Teachers of one programming summer school decided to make a surprise for the students by giving them names in the style of the "Hobbit" movie. Each student must get a pseudonym maximally similar to his own name. The pseudonym must be a name of some character of the popular saga and now the teachers are busy matching pseudonyms to student names.</p><p>There are <span class="tex-span"><i>n</i></span> students in a summer school. Teachers chose exactly <span class="tex-span"><i>n</i></span> pseudonyms for them. Each student must get exactly one pseudonym corresponding to him. Let us determine the relevance of a pseudonym <span class="tex-span"><i>b</i></span> to a student with name <span class="tex-span"><i>a</i></span> as the length of the largest common prefix <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. We will represent such value as <img align="middle" class="tex-formula" src="file://DnQv9G0A.png" style="max-width: 100.0%;max-height: 100.0%;">. Then we can determine the <span class="tex-font-style-it">quality</span> of matching of the pseudonyms to students as a sum of relevances of all pseudonyms to the corresponding students.</p><p>Find the matching between students and pseudonyms with the maximum <span class="tex-font-style-it">quality</span>.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of students in the summer school.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the name of the students. Each name is a non-empty word consisting of lowercase English letters. Some names can be repeating.</p><p>The last <span class="tex-span"><i>n</i></span> lines contain the given pseudonyms. Each pseudonym is a non-empty word consisting of small English letters. Some pseudonyms can be repeating.</p><p>The total length of all the names and pseudonyms doesn't exceed <span class="tex-span">800 000</span> characters.</p></div><div class="output-specification"><p>In the first line print the maximum possible <span class="tex-font-style-it">quality</span> of matching pseudonyms to students.</p><p>In the next <span class="tex-span"><i>n</i></span> lines describe the optimal matching. Each line must have the form <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>), that means that the student who was number <span class="tex-span"><i>a</i></span> in the input, must match to the pseudonym number <span class="tex-span"><i>b</i></span> in the input.</p><p>The matching should be a one-to-one correspondence, that is, each student and each pseudonym should occur exactly once in your output. If there are several optimal answers, output any.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of students in the summer school.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the name of the students. Each name is a non-empty word consisting of lowercase English letters. Some names can be repeating.</p><p>The last <span class="tex-span"><i>n</i></span> lines contain the given pseudonyms. Each pseudonym is a non-empty word consisting of small English letters. Some pseudonyms can be repeating.</p><p>The total length of all the names and pseudonyms doesn't exceed <span class="tex-span">800 000</span> characters.</p>

## Output

<p>In the first line print the maximum possible <span class="tex-font-style-it">quality</span> of matching pseudonyms to students.</p><p>In the next <span class="tex-span"><i>n</i></span> lines describe the optimal matching. Each line must have the form <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>), that means that the student who was number <span class="tex-span"><i>a</i></span> in the input, must match to the pseudonym number <span class="tex-span"><i>b</i></span> in the input.</p><p>The matching should be a one-to-one correspondence, that is, each student and each pseudonym should occur exactly once in your output. If there are several optimal answers, output any.</p>





```input1
5
gennady
galya
boris
bill
toshik
bilbo
torin
gendalf
smaug
galadriel

```




```output1
11
4 1
2 5
1 3
5 2
3 4

```



## Note

<p>The first test from the statement the match looks as follows: </p><ul> <li> <span class="tex-font-style-bf">bil</span>l <span class="tex-span"> → </span> <span class="tex-font-style-bf">bil</span>bo (lcp = 3) </li><li> <span class="tex-font-style-bf">gal</span>ya <span class="tex-span"> → </span> <span class="tex-font-style-bf">gal</span>adriel (lcp = 3) </li><li> <span class="tex-font-style-bf">gen</span>nady <span class="tex-span"> → </span> <span class="tex-font-style-bf">gen</span>dalf (lcp = 3) </li><li> <span class="tex-font-style-bf">to</span>shik <span class="tex-span"> → </span> <span class="tex-font-style-bf">to</span>rin (lcp = 2) </li><li> boris <span class="tex-span"> → </span> smaug (lcp = 0) </li></ul>
