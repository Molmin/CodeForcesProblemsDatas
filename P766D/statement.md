## Description

<div><p>Mahmoud wants to write a new dictionary that contains <span class="tex-span"><i>n</i></span> words and relations between them. There are two types of relations: synonymy (i.&nbsp;e. the two words mean the same) and antonymy (i.&nbsp;e. the two words mean the opposite). From time to time he discovers a new relation between two words.</p><p>He know that if two words have a relation between them, then each of them has relations with the words that has relations with the other. For example, if <span class="tex-font-style-tt">like</span> means <span class="tex-font-style-tt">love</span> and <span class="tex-font-style-tt">love</span> is the opposite of <span class="tex-font-style-tt">hate</span>, then <span class="tex-font-style-tt">like</span> is also the opposite of <span class="tex-font-style-tt">hate</span>. One more example: if <span class="tex-font-style-tt">love</span> is the opposite of <span class="tex-font-style-tt">hate</span> and <span class="tex-font-style-tt">hate</span> is the opposite of <span class="tex-font-style-tt">like</span>, then <span class="tex-font-style-tt">love</span> means <span class="tex-font-style-tt">like</span>, and so on.</p><p>Sometimes Mahmoud discovers a wrong relation. A wrong relation is a relation that makes two words equal and opposite at the same time. For example if he knows that <span class="tex-font-style-tt">love</span> means <span class="tex-font-style-tt">like</span> and <span class="tex-font-style-tt">like</span> is the opposite of <span class="tex-font-style-tt">hate</span>, and then he figures out that <span class="tex-font-style-tt">hate</span> means <span class="tex-font-style-tt">like</span>, the last relation is absolutely wrong because it makes <span class="tex-font-style-tt">hate</span> and <span class="tex-font-style-tt">like</span> opposite and have the same meaning at the same time.</p><p>After Mahmoud figured out many relations, he was worried that some of them were wrong so that they will make other relations also wrong, so he decided to tell every relation he figured out to his coder friend Ehab and for every relation he wanted to know is it correct or wrong, basing on the previously discovered relations. If it is wrong he ignores it, and doesn't check with following relations.</p><p>After adding all relations, Mahmoud asked Ehab about relations between some words based on the information he had given to him. Ehab is busy making a Codeforces round so he asked you for help.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) where <span class="tex-span"><i>n</i></span> is the number of words in the dictionary, <span class="tex-span"><i>m</i></span> is the number of relations Mahmoud figured out and <span class="tex-span"><i>q</i></span> is the number of questions Mahmoud asked after telling all relations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct words <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> consisting of small English letters with length not exceeding <span class="tex-span">20</span>, which are the words in the dictionary.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>) followed by two different words <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> which has appeared in the dictionary words. If <span class="tex-span"><i>t</i> = 1</span>, that means <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> has a synonymy relation with <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, otherwise <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> has an antonymy relation with <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each of them contains two different words which has appeared in the dictionary. That are the pairs of words Mahmoud wants to know the relation between basing on the relations he had discovered.</p><p>All words in input contain only lowercase English letters and their lengths don't exceed <span class="tex-span">20</span> characters. In all relations and in all questions the two words are different.</p></div><div class="output-specification"><p>First, print <span class="tex-span"><i>m</i></span> lines, one per each relation. If some relation is wrong (makes two words opposite and have the same meaning at the same time) you should print "<span class="tex-font-style-tt">NO</span>" (without quotes) and ignore it, otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p><p>After that print <span class="tex-span"><i>q</i></span> lines, one per each question. If the two words have the same meaning, output <span class="tex-span">1</span>. If they are opposites, output <span class="tex-span">2</span>. If there is no relation between them, output <span class="tex-span">3</span>.</p><p>See the samples for better understanding.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) where <span class="tex-span"><i>n</i></span> is the number of words in the dictionary, <span class="tex-span"><i>m</i></span> is the number of relations Mahmoud figured out and <span class="tex-span"><i>q</i></span> is the number of questions Mahmoud asked after telling all relations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct words <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> consisting of small English letters with length not exceeding <span class="tex-span">20</span>, which are the words in the dictionary.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>) followed by two different words <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> which has appeared in the dictionary words. If <span class="tex-span"><i>t</i> = 1</span>, that means <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> has a synonymy relation with <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, otherwise <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> has an antonymy relation with <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each of them contains two different words which has appeared in the dictionary. That are the pairs of words Mahmoud wants to know the relation between basing on the relations he had discovered.</p><p>All words in input contain only lowercase English letters and their lengths don't exceed <span class="tex-span">20</span> characters. In all relations and in all questions the two words are different.</p>

## Output

<p>First, print <span class="tex-span"><i>m</i></span> lines, one per each relation. If some relation is wrong (makes two words opposite and have the same meaning at the same time) you should print "<span class="tex-font-style-tt">NO</span>" (without quotes) and ignore it, otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p><p>After that print <span class="tex-span"><i>q</i></span> lines, one per each question. If the two words have the same meaning, output <span class="tex-span">1</span>. If they are opposites, output <span class="tex-span">2</span>. If there is no relation between them, output <span class="tex-span">3</span>.</p><p>See the samples for better understanding.</p>





```input1
3 3 4
hate love like
1 love like
2 love hate
1 hate like
love like
love hate
like hate
hate like

```




```input2
8 6 5
hi welcome hello ihateyou goaway dog cat rat
1 hi welcome
1 ihateyou goaway
2 hello ihateyou
2 hi goaway
2 hi hello
1 hi hello
dog cat
dog hi
hi hello
ihateyou goaway
welcome ihateyou

```




```output1
YES
YES
NO
1
2
2
2

```




```output2
YES
YES
YES
YES
NO
YES
3
3
1
1
2

```


