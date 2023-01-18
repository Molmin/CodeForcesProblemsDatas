## Description

<div><p>A widely known among some people Belarusian sport programmer Lesha decided to make some money to buy a one square meter larger flat. To do this, he wants to make and carry out a Super Rated Match (SRM) on the site Torcoder.com. But there's a problem — a severe torcoder coordinator Ivan does not accept any Lesha's problem, calling each of them an offensive word "duped" (that is, duplicated). And one day they nearely quarrelled over yet another problem Ivan wouldn't accept.</p><p>You are invited to act as a fair judge and determine whether the problem is indeed <span class="tex-font-style-underline">brand new</span>, or Ivan is right and the problem bears some resemblance to those used in the previous SRMs.</p><p>You are given the descriptions of Lesha's problem and each of Torcoder.com archive problems. The description of each problem is a sequence of words. Besides, it is guaranteed that Lesha's problem has no repeated words, while the description of an archive problem may contain any number of repeated words.</p><p>The "similarity" between Lesha's problem and some archive problem can be found as follows. Among all permutations of words in Lesha's problem we choose the one that occurs in the archive problem as a subsequence. If there are multiple such permutations, we choose the one with the smallest number of inversions. Then the "similarity" of a problem can be written as <img align="middle" class="tex-formula" src="file://lYRYejw3.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>n</i></span> is the number of words in Lesha's problem and <span class="tex-span"><i>x</i></span> is the number of inversions in the chosen permutation. Note that the "similarity" <span class="tex-span"><i>p</i></span> is always a positive integer.</p><p>The problem is called <span class="tex-font-style-underline">brand new</span> if there is not a single problem in Ivan's archive which contains a permutation of words from Lesha's problem as a subsequence.</p><p>Help the boys and determine whether the proposed problem is new, or specify the problem from the archive which resembles Lesha's problem the most, otherwise.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4</span>) — the number of words in Lesha's problem. The second line contains <span class="tex-span"><i>n</i></span> space-separated words — the short description of the problem.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>) — the number of problems in the Torcoder.com archive. Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the problems as "<span class="tex-span"><i>k</i></span> <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span>", where <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>) is the number of words in the problem and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a word of the problem description.</p><p>All words from all problem descriptions contain no more than 10 lowercase English letters. </p></div><div class="output-specification"><p>If Lesha's problem is <span class="tex-font-style-underline">brand new</span>, print string "<span class="tex-font-style-tt">Brand new problem!</span>" (without quotes). </p><p>Otherwise, on the first line print the index of the archive problem which resembles Lesha's problem most. If there are multiple such problems, print the one with the smallest index. On the second line print a string consisting of characters <span class="tex-font-style-tt">[:</span>, character <span class="tex-font-style-tt">|</span> repeated <span class="tex-span"><i>p</i></span> times, and characters <span class="tex-font-style-tt">:]</span>, where <span class="tex-span"><i>p</i></span> is the "similarity" between this problem and Lesha's one. The archive problems are numbered starting from one in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4</span>) — the number of words in Lesha's problem. The second line contains <span class="tex-span"><i>n</i></span> space-separated words — the short description of the problem.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>) — the number of problems in the Torcoder.com archive. Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the problems as "<span class="tex-span"><i>k</i></span> <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span>", where <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>) is the number of words in the problem and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a word of the problem description.</p><p>All words from all problem descriptions contain no more than 10 lowercase English letters. </p>

## Output

<p>If Lesha's problem is <span class="tex-font-style-underline">brand new</span>, print string "<span class="tex-font-style-tt">Brand new problem!</span>" (without quotes). </p><p>Otherwise, on the first line print the index of the archive problem which resembles Lesha's problem most. If there are multiple such problems, print the one with the smallest index. On the second line print a string consisting of characters <span class="tex-font-style-tt">[:</span>, character <span class="tex-font-style-tt">|</span> repeated <span class="tex-span"><i>p</i></span> times, and characters <span class="tex-font-style-tt">:]</span>, where <span class="tex-span"><i>p</i></span> is the "similarity" between this problem and Lesha's one. The archive problems are numbered starting from one in the order in which they are given in the input.</p>





```input1
4
find the next palindrome
1
10 find the previous palindrome or print better luck next time

```




```input2
3
add two numbers
3
1 add
2 two two
3 numbers numbers numbers

```




```input3
4
these papers are formulas
3
6 what are these formulas and papers
5 papers are driving me crazy
4 crazy into the night

```




```input4
3
add two decimals
5
4 please two decimals add
5 decimals want to be added
4 two add decimals add
4 add one two three
7 one plus two plus three equals six

```




```output1
1
[:||||||:]

```




```output2
Brand new problem!

```




```output3
1
[:||||:]

```




```output4
3
[:|||:]

```



## Note

<p>Let us remind you that the number of inversions is the number of pairs of words that follow in the permutation not in their original order. Thus, for example, if the original problem is "add two numbers", then permutation "numbers add two" contains two inversions — pairs of words "numbers" and "add", "numbers" and "two". </p><p>Sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>,  <i>b</i><sub class="lower-index">2</sub>,  ...,  <i>b</i><sub class="lower-index"><i>k</i></sub></span> is a subsequence of sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span> if there exists such a set of indices <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt;  <i>i</i><sub class="lower-index">2</sub> &lt; ...   &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span> that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub>  =  <i>b</i><sub class="lower-index"><i>j</i></sub></span> (in other words, if sequence <span class="tex-span"><i>b</i></span> can be obtained from <span class="tex-span"><i>a</i></span> by deleting some of its elements).</p><p>In the first test case the first problem contains the "find the palindrome next" permutation as a subsequence, in which the number of inversions equals 1 (words "palindrome" and "next").</p><p>In the second test case there is no problem that contains a permutation of words from Lesha's problem as a subsequence.</p>
