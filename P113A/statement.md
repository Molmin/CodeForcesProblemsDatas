## Description

<div><p>Petya got interested in grammar on his third year in school. He invented his own language called Petya's. Petya wanted to create a maximally simple language that would be enough to chat with friends, that's why all the language's grammar can be described with the following set of rules:</p><ul><li> There are three parts of speech: the adjective, the noun, the verb. Each word in his language is an adjective, noun or verb. </li><li> There are two genders: masculine and feminine. Each word in his language has gender either masculine or feminine. </li><li> Masculine adjectives end with <span class="tex-font-style-tt">-lios</span>, and feminine adjectives end with <span class="tex-font-style-tt">-liala</span>. </li><li> Masculine nouns end with <span class="tex-font-style-tt">-etr</span>, and feminime nouns end with <span class="tex-font-style-tt">-etra</span>. </li><li> Masculine verbs end with <span class="tex-font-style-tt">-initis</span>, and feminime verbs end with <span class="tex-font-style-tt">-inites</span>. </li><li> Thus, each word in the Petya's language has one of the six endings, given above. There are no other endings in Petya's language. </li><li> It is accepted that the whole word consists of an ending. That is, words "<span class="tex-font-style-tt">lios</span>", "<span class="tex-font-style-tt">liala</span>", "<span class="tex-font-style-tt">etr</span>" and so on belong to the Petya's language. </li><li> There aren't any punctuation marks, grammatical tenses, singular/plural forms or other language complications. </li><li> A sentence is either exactly one valid language word or exactly one <span class="tex-font-style-it">statement</span>. </li></ul><p><span class="tex-font-style-it">Statement</span> is any sequence of the Petya's language, that satisfy both conditions:</p><ul><li> Words in statement follow in the following order (from the left to the right): zero or more adjectives followed by exactly one noun followed by zero or more verbs. </li><li> All words in the statement should have the same gender.</li></ul><p>After Petya's friend Vasya wrote instant messenger (an instant messaging program) that supported the Petya's language, Petya wanted to add spelling and grammar checking to the program. As Vasya was in the country and Petya didn't feel like waiting, he asked you to help him with this problem. Your task is to define by a given sequence of words, whether it is true that the given text represents exactly one sentence in Petya's language.</p></div><div class="input-specification"><p>The first line contains one or more words consisting of lowercase Latin letters. The overall number of characters (including letters and spaces) does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that any two consecutive words are separated by exactly one space and the input data do not contain any other spaces. It is possible that given words do not belong to the Petya's language.</p></div><div class="output-specification"><p>If some word of the given text does not belong to the Petya's language or if the text contains more that one sentence, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes).</p></div>

## Input

<p>The first line contains one or more words consisting of lowercase Latin letters. The overall number of characters (including letters and spaces) does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that any two consecutive words are separated by exactly one space and the input data do not contain any other spaces. It is possible that given words do not belong to the Petya's language.</p>

## Output

<p>If some word of the given text does not belong to the Petya's language or if the text contains more that one sentence, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes).</p>





```input1
petr

```




```input2
etis atis animatis etis atis amatis

```




```input3
nataliala kataliala vetra feinites

```




```output1
YES

```




```output2
NO

```




```output3
YES

```


