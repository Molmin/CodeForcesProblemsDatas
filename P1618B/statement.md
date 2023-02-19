## Description

<div><p>Polycarp has come up with a new game to play with you. He calls it "A missing bigram".</p><p>A <span class="tex-font-style-it">bigram</span> of a word is a sequence of two adjacent letters in it.</p><p>For example, word "<span class="tex-font-style-tt">abbaaba</span>" contains bigrams "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">bb</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">ba</span>".</p><p>The game goes as follows. First, Polycarp comes up with a word, consisting only of lowercase letters 'a' and 'b'. Then, he writes down all its bigrams on a whiteboard <span class="tex-font-style-bf">in the same order as they appear in the word</span>. After that, he wipes one of them off the whiteboard.</p><p>Finally, Polycarp invites you to guess what the word that he has come up with was.</p><p>Your goal is to find any word such that it's possible to write down all its bigrams and remove one of them, so that the resulting sequence of bigrams is the same as the one Polycarp ended up with.</p><p>The tests are generated in such a way that the answer exists. If there are multiple answers, you can print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($3 \le n \le 100$)&nbsp;— the length of the word Polycarp has come up with.</p><p>The second line of each testcase contains $n-2$ bigrams of that word, separated by a single space. Each bigram consists of two letters, each of them is either 'a' or 'b'.</p><p><span class="tex-font-style-bf">Additional constraint on the input: there exists at least one string such that it is possible to write down all its bigrams, except one, so that the resulting sequence is the same as the sequence in the input. In other words, the answer exists.</span></p></div><div class="output-specification"><p>For each testcase print a word, consisting of $n$ letters, each of them should be either 'a' or 'b'. It should be possible to write down all its bigrams and remove one of them, so that the resulting sequence of bigrams is the same as the one Polycarp ended up with.</p><p>The tests are generated in such a way that the answer exists. If there are multiple answers, you can print any of them. </p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($3 \le n \le 100$)&nbsp;— the length of the word Polycarp has come up with.</p><p>The second line of each testcase contains $n-2$ bigrams of that word, separated by a single space. Each bigram consists of two letters, each of them is either 'a' or 'b'.</p><p><span class="tex-font-style-bf">Additional constraint on the input: there exists at least one string such that it is possible to write down all its bigrams, except one, so that the resulting sequence is the same as the sequence in the input. In other words, the answer exists.</span></p>

## Output

<p>For each testcase print a word, consisting of $n$ letters, each of them should be either 'a' or 'b'. It should be possible to write down all its bigrams and remove one of them, so that the resulting sequence of bigrams is the same as the one Polycarp ended up with.</p><p>The tests are generated in such a way that the answer exists. If there are multiple answers, you can print any of them. </p>





```input1
4
7
ab bb ba aa ba
7
ab ba aa ab ba
3
aa
5
bb ab bb
```




```output1
abbaaba
abaabaa
baa
bbabb
```



## Note

<p>The first two testcases from the example are produced from the word "<span class="tex-font-style-tt">abbaaba</span>". As listed in the statement, it contains bigrams "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">bb</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">ba</span>".</p><p>In the first testcase, the $5$-th bigram is removed. </p><p>In the second testcase, the $2$-nd bigram is removed. However, that sequence could also have been produced from the word "<span class="tex-font-style-tt">abaabaa</span>". It contains bigrams "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>" and "<span class="tex-font-style-tt">aa</span>". The missing bigram is the $6$-th one.</p><p>In the third testcase, all of "<span class="tex-font-style-tt">baa</span>", "<span class="tex-font-style-tt">aab</span>" and "<span class="tex-font-style-tt">aaa</span>" are valid answers.</p>
