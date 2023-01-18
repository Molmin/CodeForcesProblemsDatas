## Description

<div><p>Sometimes some words like "<span class="tex-font-style-tt">localization</span>" or "<span class="tex-font-style-tt">internationalization</span>" are so long that writing them many times in one text is quite tiresome.</p><p>Let's consider a word <span class="tex-font-style-it">too long</span>, if its length is <span class="tex-font-style-bf">strictly more</span> than <span class="tex-span">10</span> characters. All too long words should be replaced with a special abbreviation.</p><p>This abbreviation is made like this: we write down the first and the last letter of a word and between them we write the number of letters between the first and the last letters. That number is in decimal system and doesn't contain any leading zeroes.</p><p>Thus, "<span class="tex-font-style-tt">localization</span>" will be spelt as "<span class="tex-font-style-tt">l10n</span>", and "<span class="tex-font-style-tt">internationalization</span>» will be spelt as "<span class="tex-font-style-tt">i18n</span>".</p><p>You are suggested to automatize the process of changing the words with abbreviations. At that all too long words should be replaced by the abbreviation and the words that are not too long should not undergo any changes.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains one word. All the words consist of lowercase Latin letters and possess the lengths of from <span class="tex-span">1</span> to <span class="tex-span">100</span> characters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain the result of replacing of the <span class="tex-span"><i>i</i></span>-th word from the input data.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains one word. All the words consist of lowercase Latin letters and possess the lengths of from <span class="tex-span">1</span> to <span class="tex-span">100</span> characters.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain the result of replacing of the <span class="tex-span"><i>i</i></span>-th word from the input data.</p>





```input1
4
word
localization
internationalization
pneumonoultramicroscopicsilicovolcanoconiosis

```




```output1
word
l10n
i18n
p43s

```


