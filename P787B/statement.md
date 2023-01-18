## Description

<div><p>Since the giant heads have appeared in the sky all humanity is in danger, so <span class="tex-font-style-bf">all</span> Ricks and Mortys from all parallel universes are gathering in groups to find a solution to get rid of them. </p><p>There are <span class="tex-span"><i>n</i></span> parallel universes participating in this event (<span class="tex-span"><i>n</i></span> Ricks and <span class="tex-span"><i>n</i></span> Mortys). I. e. each of <span class="tex-span"><i>n</i></span> universes has one Rick and one Morty. They're gathering in <span class="tex-span"><i>m</i></span> groups. Each person can be in many groups and a group can contain an arbitrary number of members.</p><p>Ricks and Mortys have registered online in these groups. So, a person can have joined a group more than once (developer of this website hadn't considered this possibility).</p><center> <img class="tex-graphics" src="file://LLH0WPUq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Summer from universe #1 knows that in each parallel universe (including hers) exactly one of Rick and Morty from that universe is a traitor and is loyal, but no one knows which one. She knows that we are doomed if there's a group such that every member in that group is a traitor (they will plan and destroy the world). </p><p>Summer knows that if there's a possibility that world ends (there's a group where all members are traitors) she should immediately cancel this event. So she wants to know if she should cancel the event. You have to tell her yes if and only if there's at least one scenario (among all <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> possible scenarios, <span class="tex-span">2</span> possible scenarios for who a traitor in each universe) such that in that scenario the world will end.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — number of universes and number of groups respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the information about the groups. <span class="tex-span"><i>i</i></span>-th of them first contains an integer <span class="tex-span"><i>k</i></span> (number of times someone joined <span class="tex-span"><i>i</i></span>-th group, <span class="tex-span"><i>k</i> &gt; 0</span>) followed by <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>v</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>v</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>. If <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is negative, it means that Rick from universe number <span class="tex-span"> - <i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> has joined this group and otherwise it means that Morty from universe number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> has joined it.</p><p>Sum of <span class="tex-span"><i>k</i></span> for all groups does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>In a single line print the answer to Summer's question. Print "<span class="tex-font-style-tt">YES</span>" if she should cancel the event and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — number of universes and number of groups respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the information about the groups. <span class="tex-span"><i>i</i></span>-th of them first contains an integer <span class="tex-span"><i>k</i></span> (number of times someone joined <span class="tex-span"><i>i</i></span>-th group, <span class="tex-span"><i>k</i> &gt; 0</span>) followed by <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>v</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>v</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>. If <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is negative, it means that Rick from universe number <span class="tex-span"> - <i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> has joined this group and otherwise it means that Morty from universe number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> has joined it.</p><p>Sum of <span class="tex-span"><i>k</i></span> for all groups does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>In a single line print the answer to Summer's question. Print "<span class="tex-font-style-tt">YES</span>" if she should cancel the event and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
4 2
1 -3
4 -2 3 2 -3

```




```input2
5 2
5 3 -2 1 -1 5
3 -5 2 5

```




```input3
7 2
3 -1 6 7
7 -5 4 2 4 7 -3 4

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample testcase, <span class="tex-span">1</span>st group only contains the Rick from universe number <span class="tex-span">3</span>, so in case he's a traitor, then all members of this group are traitors and so Summer should cancel the event.</p>
