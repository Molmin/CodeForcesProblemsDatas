## Description

<div><p>Ilya is a very clever lion, he lives in an unusual city ZooVille. In this city all the animals have their rights and obligations. Moreover, they even have their own bank accounts. The state of a bank account is an integer. The state of a bank account can be a negative number. This means that the owner of the account owes the bank money.</p><p>Ilya the Lion has recently had a birthday, so he got a lot of gifts. One of them (the gift of the main ZooVille bank) is the opportunity to delete the last digit or the digit before last from the state of his bank account no more than once. For example, if the state of Ilya's bank account is -123, then Ilya can delete the last digit and get his account balance equal to -12, also he can remove its digit before last and get the account balance equal to -13. Of course, Ilya is permitted not to use the opportunity to delete a digit from the balance.</p><p>Ilya is not very good at math, and that's why he asks you to help him maximize his bank account. Find the maximum state of the bank account that can be obtained using the bank's gift.</p></div><div class="input-specification"><p>The single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(10 ≤ |<i>n</i>| ≤ 10<sup class="upper-index">9</sup>)</span> — the state of Ilya's bank account.</p></div><div class="output-specification"><p>In a single line print an integer — the maximum state of the bank account that Ilya can get. </p></div>

## Input

<p>The single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(10 ≤ |<i>n</i>| ≤ 10<sup class="upper-index">9</sup>)</span> — the state of Ilya's bank account.</p>

## Output

<p>In a single line print an integer — the maximum state of the bank account that Ilya can get. </p>





```input1
2230

```




```input2
-10

```




```input3
-100003

```




```output1
2230

```




```output2
0

```




```output3
-10000

```



## Note

<p>In the first test sample Ilya doesn't profit from using the present.</p><p>In the second test sample you can delete digit 1 and get the state of the account equal to 0.</p>
