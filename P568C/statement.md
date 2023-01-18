## Description

<div><p>Living in Byteland was good enough to begin with, but the good king decided to please his subjects and to introduce a national language. He gathered the best of wise men, and sent an expedition to faraway countries, so that they would find out all about how a language should be designed.</p><p>After some time, the wise men returned from the trip even wiser. They locked up for six months in the dining room, after which they said to the king: "there are a lot of different languages, but almost all of them have letters that are divided into vowels and consonants; in a word, vowels and consonants must be combined correctly."</p><p>There are very many rules, all of them have exceptions, but our language will be deprived of such defects! We propose to introduce a set of formal rules of combining vowels and consonants, and include in the language all the words that satisfy them.</p><p>The rules of composing words are:</p><ul><li> The letters are divided into vowels and consonants in some certain way;</li><li> All words have a length of exactly <span class="tex-span"><i>n</i></span>;</li><li> There are <span class="tex-span"><i>m</i></span> rules of the form (<span class="tex-span"><i>pos</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>pos</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">2</sub></span>). Each rule is: if the position <span class="tex-span"><i>pos</i><sub class="lower-index">1</sub></span> has a letter of type <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, then the position <span class="tex-span"><i>pos</i><sub class="lower-index">2</sub></span> has a letter of type <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>.</li></ul><p>You are given some string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, it is not necessarily a correct word of the new language. Among all the words of the language that lexicographically not smaller than the string <span class="tex-span"><i>s</i></span>, find the minimal one in lexicographic order.</p></div><div class="input-specification"><p>The first line contains a single line consisting of letters '<span class="tex-font-style-tt">V</span>' (Vowel) and '<span class="tex-font-style-tt">C</span>' (Consonant), determining which letters are vowels and which letters are consonants. The length of this string <span class="tex-span"><i>l</i></span> is the size of the alphabet of the new language (<span class="tex-span">1 ≤ <i>l</i> ≤ 26</span>). The first <span class="tex-span"><i>l</i></span> letters of the English alphabet are used as the letters of the alphabet of the new language. If the <span class="tex-span"><i>i</i></span>-th character of the string equals to '<span class="tex-font-style-tt">V</span>', then the corresponding letter is a vowel, otherwise it is a consonant.</p><p>The second line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4<i>n</i>(<i>n</i> - 1)</span>)&nbsp;— the number of letters in a single word and the number of rules, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe <span class="tex-span"><i>m</i></span> rules of the language in the following format: <span class="tex-span"><i>pos</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>pos</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>pos</i><sub class="lower-index">1</sub>, <i>pos</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span"><i>pos</i><sub class="lower-index">1</sub> ≠ <i>pos</i><sub class="lower-index">2</sub></span>, <img align="middle" class="tex-formula" src="file://Qe4Xr3LK.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">V</span>', '<span class="tex-font-style-tt">C</span>' <span class="tex-span">}</span>).</p><p>The last line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of the first <span class="tex-span"><i>l</i></span> small letters of the English alphabet.</p><p>It is guaranteed that no two rules are the same.</p></div><div class="output-specification"><p>Print a smallest word of a language that is lexicographically not smaller than <span class="tex-span"><i>s</i></span>. If such words does not exist (for example, if the language has no words at all), print <span class="tex-font-style-tt">"-1"</span> (without the quotes).</p></div>

## Input

<p>The first line contains a single line consisting of letters '<span class="tex-font-style-tt">V</span>' (Vowel) and '<span class="tex-font-style-tt">C</span>' (Consonant), determining which letters are vowels and which letters are consonants. The length of this string <span class="tex-span"><i>l</i></span> is the size of the alphabet of the new language (<span class="tex-span">1 ≤ <i>l</i> ≤ 26</span>). The first <span class="tex-span"><i>l</i></span> letters of the English alphabet are used as the letters of the alphabet of the new language. If the <span class="tex-span"><i>i</i></span>-th character of the string equals to '<span class="tex-font-style-tt">V</span>', then the corresponding letter is a vowel, otherwise it is a consonant.</p><p>The second line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4<i>n</i>(<i>n</i> - 1)</span>)&nbsp;— the number of letters in a single word and the number of rules, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe <span class="tex-span"><i>m</i></span> rules of the language in the following format: <span class="tex-span"><i>pos</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>pos</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>pos</i><sub class="lower-index">1</sub>, <i>pos</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span"><i>pos</i><sub class="lower-index">1</sub> ≠ <i>pos</i><sub class="lower-index">2</sub></span>, <img align="middle" class="tex-formula" src="file://Qe4Xr3LK.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">V</span>', '<span class="tex-font-style-tt">C</span>' <span class="tex-span">}</span>).</p><p>The last line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of the first <span class="tex-span"><i>l</i></span> small letters of the English alphabet.</p><p>It is guaranteed that no two rules are the same.</p>

## Output

<p>Print a smallest word of a language that is lexicographically not smaller than <span class="tex-span"><i>s</i></span>. If such words does not exist (for example, if the language has no words at all), print <span class="tex-font-style-tt">"-1"</span> (without the quotes).</p>





```input1
VC
2 1
1 V 2 C
aa

```




```input2
VC
2 1
1 C 2 V
bb

```




```input3
VCC
4 3
1 C 2 V
2 C 3 V
3 V 4 V
abac

```




```output1
ab

```




```output2
-1

```




```output3
acaa

```



## Note

<p>In the first test word <span class="tex-font-style-tt">"aa"</span> is not a word of the language, but word <span class="tex-font-style-tt">"ab"</span> is.</p><p>In the second test out of all four possibilities only word <span class="tex-font-style-tt">"bb"</span> is not a word of a language, but all other words are lexicographically less, so there is no answer.</p><p>In the third test, due to the last rule, <span class="tex-font-style-tt">"abac"</span> doesn't belong to the language (<span class="tex-font-style-tt">"a"</span> is a vowel, <span class="tex-font-style-tt">"c"</span> is a consonant). The only word with prefix <span class="tex-font-style-tt">"ab"</span> that meets the given rules is <span class="tex-font-style-tt">"abaa"</span>. But it is less than <span class="tex-font-style-tt">"abac"</span>, so the answer will be <span class="tex-font-style-tt">"acaa"</span></p>
