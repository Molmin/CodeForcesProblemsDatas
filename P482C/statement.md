## Description

<div><p>You play the game with your friend. The description of this game is listed below. </p><p>Your friend creates <span class="tex-span"><i>n</i></span> distinct strings of the same length <span class="tex-span"><i>m</i></span> and tells you all the strings. Then he randomly chooses one of them. He chooses strings equiprobably, i.e. the probability of choosing each of the <span class="tex-span"><i>n</i></span> strings equals <img align="middle" class="tex-formula" src="file://LhMaMZrC.png" style="max-width: 100.0%;max-height: 100.0%;">. You want to guess which string was chosen by your friend. </p><p>In order to guess what string your friend has chosen, you are allowed to ask him questions. Each question has the following form: «What character stands on position <span class="tex-span"><i>pos</i></span> in the string you have chosen?» A string is considered guessed when the answers to the given questions uniquely identify the string. After the string is guessed, you stop asking questions. </p><p>You do not have a particular strategy, so as each question you equiprobably ask about a position that hasn't been yet mentioned. Your task is to determine the expected number of questions needed to guess the string chosen by your friend.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of strings your friend came up with.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the strings that your friend has created. It is guaranteed that all the strings are distinct and only consist of large and small English letters. Besides, the lengths of all strings are the same and are between <span class="tex-span">1</span> to <span class="tex-span">20</span> inclusive.</p></div><div class="output-specification"><p>Print the single number — the expected value. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of strings your friend came up with.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the strings that your friend has created. It is guaranteed that all the strings are distinct and only consist of large and small English letters. Besides, the lengths of all strings are the same and are between <span class="tex-span">1</span> to <span class="tex-span">20</span> inclusive.</p>

## Output

<p>Print the single number — the expected value. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
2
aab
aac

```




```input2
3
aaA
aBa
Caa

```




```input3
3
aca
vac
wqq

```




```output1
2.000000000000000

```




```output2
1.666666666666667

```




```output3
1.000000000000000

```



## Note

<p>In the first sample the strings only differ in the character in the third position. So only the following situations are possible: </p><ul> <li> you guess the string in one question. The event's probability is <img align="middle" class="tex-formula" src="file://7FV8DWVh.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> you guess the string in two questions. The event's probability is <img align="middle" class="tex-formula" src="file://yWKOeNFw.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <img align="middle" class="tex-formula" src="file://9CoW7i8z.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://VhlhGwwf.png" style="max-width: 100.0%;max-height: 100.0%;"> (as in this case the first question should ask about the position that is other than the third one); </li><li> you guess the string in three questions. The event's probability is <img align="middle" class="tex-formula" src="file://mjNKe4nG.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <img align="middle" class="tex-formula" src="file://Fk5BHAVv.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <img align="middle" class="tex-formula" src="file://Vc925K7k.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://TwxlOEhQ.png" style="max-width: 100.0%;max-height: 100.0%;">; </li></ul><p>Thus, the expected value is equal to <img align="middle" class="tex-formula" src="file://bX0QKYWp.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second sample we need at most two questions as any pair of questions uniquely identifies the string. So the expected number of questions is <img align="middle" class="tex-formula" src="file://L0W2KfLV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample whatever position we ask about in the first question, we immediately identify the string.</p>
