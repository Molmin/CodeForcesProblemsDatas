## Description

<div><p>We just discovered a new data structure in our research group: a <span class="tex-font-style-bf">suffix three</span>!</p><p>It's very useful for natural language processing. Given three languages and three suffixes, a suffix three can determine which language a sentence is written in.</p><p>It's super simple, 100% accurate, and doesn't involve advanced machine learning algorithms.</p><p>Let us tell you how it works.</p><ul> <li> If a sentence ends with "<span class="tex-font-style-tt">po</span>" the language is Filipino. </li><li> If a sentence ends with "<span class="tex-font-style-tt">desu</span>" or "<span class="tex-font-style-tt">masu</span>" the language is Japanese. </li><li> If a sentence ends with "<span class="tex-font-style-tt">mnida</span>" the language is Korean. </li></ul><p>Given this, we need you to implement a suffix three that can differentiate Filipino, Japanese, and Korean.</p><p>Oh, did I say three suffixes? I meant four.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 30$) denoting the number of test cases. The next lines contain descriptions of the test cases. </p><p>Each test case consists of a single line containing a single string denoting the sentence. Spaces are represented as underscores (the symbol "<span class="tex-font-style-tt">_</span>") for ease of reading. The sentence has at least $1$ and at most $1000$ characters, and consists only of lowercase English letters and underscores. The sentence has no leading or trailing underscores and no two consecutive underscores. It is guaranteed that the sentence ends with one of the four suffixes mentioned above.</p></div><div class="output-specification"><p>For each test case, print a single line containing either "<span class="tex-font-style-tt">FILIPINO</span>", "<span class="tex-font-style-tt">JAPANESE</span>", or "<span class="tex-font-style-tt">KOREAN</span>" (all in uppercase, without quotes), depending on the detected language.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 30$) denoting the number of test cases. The next lines contain descriptions of the test cases. </p><p>Each test case consists of a single line containing a single string denoting the sentence. Spaces are represented as underscores (the symbol "<span class="tex-font-style-tt">_</span>") for ease of reading. The sentence has at least $1$ and at most $1000$ characters, and consists only of lowercase English letters and underscores. The sentence has no leading or trailing underscores and no two consecutive underscores. It is guaranteed that the sentence ends with one of the four suffixes mentioned above.</p>

## Output

<p>For each test case, print a single line containing either "<span class="tex-font-style-tt">FILIPINO</span>", "<span class="tex-font-style-tt">JAPANESE</span>", or "<span class="tex-font-style-tt">KOREAN</span>" (all in uppercase, without quotes), depending on the detected language.</p>





```input1
8
kamusta_po
genki_desu
ohayou_gozaimasu
annyeong_hashimnida
hajime_no_ippo
bensamu_no_sentou_houhou_ga_okama_kenpo
ang_halaman_doon_ay_sarisari_singkamasu
si_roy_mustang_ay_namamasu
```




```output1
FILIPINO
JAPANESE
JAPANESE
KOREAN
FILIPINO
FILIPINO
JAPANESE
JAPANESE
```



## Note

<p>The first sentence ends with "<span class="tex-font-style-tt">po</span>", so it is written in Filipino.</p><p>The second and third sentences end with "<span class="tex-font-style-tt">desu</span>" and "<span class="tex-font-style-tt">masu</span>", so they are written in Japanese.</p><p>The fourth sentence ends with "<span class="tex-font-style-tt">mnida</span>", so it is written in Korean.</p>
