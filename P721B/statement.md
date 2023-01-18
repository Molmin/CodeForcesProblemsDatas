## Description

<div><p>Vanya is managed to enter his favourite site Codehorses. Vanya uses <span class="tex-span"><i>n</i></span> distinct passwords for sites at all, however he can't remember which one exactly he specified during Codehorses registration.</p><p>Vanya will enter passwords in order of non-decreasing their lengths, and he will enter passwords of same length in arbitrary order. Just when Vanya will have entered the correct password, he is immediately authorized on the site. Vanya will not enter any password twice.</p><p>Entering any passwords takes one second for Vanya. But if Vanya will enter wrong password <span class="tex-span"><i>k</i></span> times, then he is able to make the next try only <span class="tex-span">5</span> seconds after that. Vanya makes each try immediately, that is, at each moment when Vanya is able to enter password, he is doing that.</p><p>Determine how many seconds will Vanya need to enter Codehorses in the best case for him (if he spends minimum possible number of second) and in the worst case (if he spends maximum possible amount of seconds).</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>)&nbsp;— the number of Vanya's passwords and the number of failed tries, after which the access to the site is blocked for <span class="tex-span">5</span> seconds.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains passwords, one per line&nbsp;— pairwise distinct non-empty strings consisting of latin letters and digits. Each password length does not exceed <span class="tex-span">100</span> characters.</p><p>The last line of the input contains the Vanya's Codehorses password. It is guaranteed that the Vanya's Codehorses password is equal to some of his <span class="tex-span"><i>n</i></span> passwords.</p></div><div class="output-specification"><p>Print two integers&nbsp;— time (in seconds), Vanya needs to be authorized to Codehorses in the best case for him and in the worst case respectively.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>)&nbsp;— the number of Vanya's passwords and the number of failed tries, after which the access to the site is blocked for <span class="tex-span">5</span> seconds.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains passwords, one per line&nbsp;— pairwise distinct non-empty strings consisting of latin letters and digits. Each password length does not exceed <span class="tex-span">100</span> characters.</p><p>The last line of the input contains the Vanya's Codehorses password. It is guaranteed that the Vanya's Codehorses password is equal to some of his <span class="tex-span"><i>n</i></span> passwords.</p>

## Output

<p>Print two integers&nbsp;— time (in seconds), Vanya needs to be authorized to Codehorses in the best case for him and in the worst case respectively.</p>





```input1
5 2
cba
abc
bb1
abC
ABC
abc

```




```input2
4 100
11
22
1
2
22

```




```output1
1 15

```




```output2
3 4

```



## Note

<p>Consider the first sample case. As soon as all passwords have the same length, Vanya can enter the right password at the first try as well as at the last try. If he enters it at the first try, he spends exactly <span class="tex-span">1</span> second. Thus in the best case the answer is <span class="tex-span">1</span>. If, at the other hand, he enters it at the last try, he enters another <span class="tex-span">4</span> passwords before. He spends <span class="tex-span">2</span> seconds to enter first <span class="tex-span">2</span> passwords, then he waits <span class="tex-span">5</span> seconds as soon as he made <span class="tex-span">2</span> wrong tries. Then he spends <span class="tex-span">2</span> more seconds to enter <span class="tex-span">2</span> wrong passwords, again waits <span class="tex-span">5</span> seconds and, finally, enters the correct password spending <span class="tex-span">1</span> more second. In summary in the worst case he is able to be authorized in <span class="tex-span">15</span> seconds.</p><p>Consider the second sample case. There is no way of entering passwords and get the access to the site blocked. As soon as the required password has length of <span class="tex-span">2</span>, Vanya enters all passwords of length <span class="tex-span">1</span> anyway, spending <span class="tex-span">2</span> seconds for that. Then, in the best case, he immediately enters the correct password and the answer for the best case is <span class="tex-span">3</span>, but in the worst case he enters wrong password of length <span class="tex-span">2</span> and only then the right one, spending <span class="tex-span">4</span> seconds at all.</p>
