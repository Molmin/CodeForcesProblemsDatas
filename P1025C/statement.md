## Description

<div><p>Is there anything better than going to the zoo after a tiresome week at work? No wonder Grisha feels the same while spending the entire weekend accompanied by pretty striped zebras. </p><p>Inspired by this adventure and an accidentally found plasticine pack (represented as a sequence of black and white stripes), Grisha now wants to select several consequent (contiguous) pieces of alternating colors to create a zebra. Let's call the number of selected pieces the length of the zebra.</p><p>Before assembling the zebra Grisha can make the following operation $0$ or more times. He splits the sequence in some place into two parts, then reverses each of them and sticks them together again. For example, if Grisha has pieces in the order "<span class="tex-font-style-tt">bwbbw</span>" (here '<span class="tex-font-style-tt">b</span>' denotes a black strip, and '<span class="tex-font-style-tt">w</span>' denotes a white strip), then he can split the sequence as <span class="tex-font-style-tt">bw|bbw</span> (here the vertical bar represents the cut), reverse both parts and obtain "<span class="tex-font-style-tt">wbwbb</span>".</p><p>Determine the maximum possible length of the zebra that Grisha can produce.</p></div><div class="input-specification"><p>The only line contains a string $s$ ($1 \le |s| \le 10^5$, where $|s|$ denotes the length of the string $s$) comprised of lowercase English letters '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">w</span>' only, where '<span class="tex-font-style-tt">w</span>' denotes a white piece and '<span class="tex-font-style-tt">b</span>' denotes a black piece.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible zebra length.</p></div>

## Input

<p>The only line contains a string $s$ ($1 \le |s| \le 10^5$, where $|s|$ denotes the length of the string $s$) comprised of lowercase English letters '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">w</span>' only, where '<span class="tex-font-style-tt">w</span>' denotes a white piece and '<span class="tex-font-style-tt">b</span>' denotes a black piece.</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible zebra length.</p>





```input1
bwwwbwwbw

```




```input2
bwwbwwb

```




```output1
5

```




```output2
3

```



## Note

<p>In the first example one of the possible sequence of operations is <span class="tex-font-style-tt">bwwwbww|bw</span> $\to$ <span class="tex-font-style-tt">w|wbwwwbwb</span> $\to$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">wbwbw</span>wwbw</span>, that gives the answer equal to $5$.</p><p>In the second example no operation can increase the answer.</p>
