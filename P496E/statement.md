## Description

<div><p>You are an assistant director in a new musical play. The play consists of <span class="tex-span"><i>n</i></span> musical parts, each part must be performed by exactly one actor. After the casting the director chose <span class="tex-span"><i>m</i></span> actors who can take part in the play. Your task is to assign the parts to actors. However, there are several limitations.</p><p>First, each actor has a certain voice range and there are some parts that he cannot sing. Formally, there are two integers for each actor, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the pitch of the lowest and the highest note that the actor can sing. There also are two integers for each part&nbsp;— <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub></span>)&nbsp;— the pitch of the lowest and the highest notes that are present in the part. The <span class="tex-span"><i>i</i></span>-th actor can perform the <span class="tex-span"><i>j</i></span>-th part if and only if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub></span>, i.e. each note of the part is in the actor's voice range.</p><p>According to the contract, the <span class="tex-span"><i>i</i></span>-th actor can perform at most <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> parts. Besides, you are allowed not to give any part to some actors (then they take part in crowd scenes).</p><p>The rehearsal starts in two hours and you need to do the assignment quickly!</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of parts in the play (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>&nbsp;— the range of notes for the <span class="tex-span"><i>j</i></span>-th part (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of actors (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers each, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the range of the <span class="tex-span"><i>i</i></span>-th actor and the number of parts that he can perform (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>If there is an assignment that meets all the criteria aboce, print a single word "<span class="tex-font-style-tt">YES</span>" (without the quotes) in the first line.</p><p>In the next line print <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer should be the number of the actor who should perform the <span class="tex-span"><i>i</i></span>-th part. If there are multiple correct assignments, print any of them.</p><p>If there is no correct assignment, print a single word "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of parts in the play (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>&nbsp;— the range of notes for the <span class="tex-span"><i>j</i></span>-th part (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of actors (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers each, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the range of the <span class="tex-span"><i>i</i></span>-th actor and the number of parts that he can perform (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>If there is an assignment that meets all the criteria aboce, print a single word "<span class="tex-font-style-tt">YES</span>" (without the quotes) in the first line.</p><p>In the next line print <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer should be the number of the actor who should perform the <span class="tex-span"><i>i</i></span>-th part. If there are multiple correct assignments, print any of them.</p><p>If there is no correct assignment, print a single word "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
3
1 3
2 4
3 5
2
1 4 2
2 5 1

```




```input2
3
1 3
2 4
3 5
2
1 3 2
2 5 1

```




```output1
YES
1 1 2

```




```output2
NO

```


