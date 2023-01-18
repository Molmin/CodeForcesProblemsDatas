## Description

<div><p>There are some ambiguities when one writes Berland names with the letters of the Latin alphabet.</p><p>For example, the Berland sound <span class="tex-font-style-it">u</span> can be written in the Latin alphabet as "<span class="tex-font-style-tt">u</span>", and can be written as "<span class="tex-font-style-tt">oo</span>". For this reason, two words "<span class="tex-font-style-tt">ulyana</span>" and "<span class="tex-font-style-tt">oolyana</span>" denote the same name.</p><p>The second ambiguity is about the Berland sound <span class="tex-font-style-it">h</span>: one can use both "<span class="tex-font-style-tt">h</span>" and "<span class="tex-font-style-tt">kh</span>" to write it. For example, the words "<span class="tex-font-style-tt">mihail</span>" and "<span class="tex-font-style-tt">mikhail</span>" denote the same name.</p><p>There are <span class="tex-span"><i>n</i></span> users registered on the Polycarp's website. Each of them indicated a name represented by the Latin letters. How many distinct names are there among them, if two ambiguities described above are taken into account?</p><p>Formally, we assume that two words denote the same name, if using the replacements "<span class="tex-font-style-tt">u</span>"&nbsp;<img align="middle" class="tex-formula" src="file://4ot8PCTP.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;"<span class="tex-font-style-tt">oo</span>" and "<span class="tex-font-style-tt">h</span>"&nbsp;<img align="middle" class="tex-formula" src="file://3g0lvbQS.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;"<span class="tex-font-style-tt">kh</span>", you can make the words equal. One can make replacements in both directions, in any of the two words an arbitrary number of times. A letter that resulted from the previous replacement can participate in the next replacements.</p><p>For example, the following pairs of words denote the same name:</p><ul> <li> "<span class="tex-font-style-tt">koouper</span>" and "<span class="tex-font-style-tt">kuooper</span>". Making the replacements described above, you can make both words to be equal: "<span class="tex-font-style-tt">koouper</span>" <img align="middle" class="tex-formula" src="file://ynMfW3xw.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">kuuper</span>" and "<span class="tex-font-style-tt">kuooper</span>" <img align="middle" class="tex-formula" src="file://VwGtg07s.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">kuuper</span>". </li><li> "<span class="tex-font-style-tt">khun</span>" and "<span class="tex-font-style-tt">kkkhoon</span>". With the replacements described above you can make both words to be equal: "<span class="tex-font-style-tt">khun</span>" <img align="middle" class="tex-formula" src="file://yVMAvHCH.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">khoon</span>" and "<span class="tex-font-style-tt">kkkhoon</span>" <img align="middle" class="tex-formula" src="file://kjnKE1vL.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">kkhoon</span>" <img align="middle" class="tex-formula" src="file://8k8Me8qt.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">khoon</span>". </li></ul><p>For a given list of words, find the minimal number of groups where the words in each group denote the same name.</p></div><div class="input-specification"><p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>) — number of the words in the list.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain words, one word per line. Each word consists of only lowercase Latin letters. The length of each word is between <span class="tex-span">1</span> and <span class="tex-span">20</span> letters inclusive.</p></div><div class="output-specification"><p>Print the minimal number of groups where the words in each group denote the same name.</p></div>

## Input

<p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>) — number of the words in the list.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain words, one word per line. Each word consists of only lowercase Latin letters. The length of each word is between <span class="tex-span">1</span> and <span class="tex-span">20</span> letters inclusive.</p>

## Output

<p>Print the minimal number of groups where the words in each group denote the same name.</p>





```input1
10
mihail
oolyana
kooooper
hoon
ulyana
koouper
mikhail
khun
kuooper
kkkhoon

```




```input2
9
hariton
hkariton
buoi
kkkhariton
boooi
bui
khariton
boui
boi

```




```input3
2
alex
alex

```




```output1
4

```




```output2
5

```




```output3
1

```



## Note

<p>There are four groups of words in the first example. Words in each group denote same name:</p><ol> <li> "<span class="tex-font-style-tt">mihail</span>", "<span class="tex-font-style-tt">mikhail</span>" </li><li> "<span class="tex-font-style-tt">oolyana</span>", "<span class="tex-font-style-tt">ulyana</span>" </li><li> "<span class="tex-font-style-tt">kooooper</span>", "<span class="tex-font-style-tt">koouper</span>" </li><li> "<span class="tex-font-style-tt">hoon</span>", "<span class="tex-font-style-tt">khun</span>", "<span class="tex-font-style-tt">kkkhoon</span>" </li></ol><p>There are five groups of words in the second example. Words in each group denote same name:</p><ol> <li> "<span class="tex-font-style-tt">hariton</span>", "<span class="tex-font-style-tt">kkkhariton</span>", "<span class="tex-font-style-tt">khariton</span>" </li><li> "<span class="tex-font-style-tt">hkariton</span>" </li><li> "<span class="tex-font-style-tt">buoi</span>", "<span class="tex-font-style-tt">boooi</span>", "<span class="tex-font-style-tt">boui</span>" </li><li> "<span class="tex-font-style-tt">bui</span>" </li><li> "<span class="tex-font-style-tt">boi</span>" </li></ol><p>In the third example the words are equal, so they denote the same name.</p>
