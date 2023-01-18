## Description

<div><p>The ship crashed into a reef and is sinking. Now the entire crew must be evacuated. All <span class="tex-span"><i>n</i></span> crew members have already lined up in a row (for convenience let's label them all from left to right with positive integers from 1 to <span class="tex-span"><i>n</i></span>) and await further instructions. However, one should evacuate the crew properly, in a strict order. Specifically:</p><p>The first crew members to leave the ship are rats. Then women and children (both groups have the same priority) leave the ship. After that all men are evacuated from the ship. The captain leaves the sinking ship last.</p><p>If we cannot determine exactly who should leave the ship first for any two members of the crew by the rules from the previous paragraph, then the one who stands to the left in the line leaves the ship first (or in other words, the one whose number in the line is less).</p><p>For each crew member we know his status as a crew member, and also his name. All crew members have different names. Determine the order in which to evacuate the crew.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of people in the crew (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then follow <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of those lines contains two words — the name of the crew member who is <span class="tex-span"><i>i</i></span>-th in line, and his status on the ship. The words are separated by exactly one space. There are no other spaces in the line. The names consist of Latin letters, the first letter is uppercase, the rest are lowercase. The length of any name is from 1 to 10 characters. The status can have the following values: <span class="tex-font-style-tt">rat</span> for a rat, <span class="tex-font-style-tt">woman</span> for a woman, <span class="tex-font-style-tt">child</span> for a child, <span class="tex-font-style-tt">man</span> for a man, <span class="tex-font-style-tt">captain</span> for the captain. The crew contains exactly one captain.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the name of the crew member who must be the <span class="tex-span"><i>i</i></span>-th one to leave the ship.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of people in the crew (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then follow <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of those lines contains two words — the name of the crew member who is <span class="tex-span"><i>i</i></span>-th in line, and his status on the ship. The words are separated by exactly one space. There are no other spaces in the line. The names consist of Latin letters, the first letter is uppercase, the rest are lowercase. The length of any name is from 1 to 10 characters. The status can have the following values: <span class="tex-font-style-tt">rat</span> for a rat, <span class="tex-font-style-tt">woman</span> for a woman, <span class="tex-font-style-tt">child</span> for a child, <span class="tex-font-style-tt">man</span> for a man, <span class="tex-font-style-tt">captain</span> for the captain. The crew contains exactly one captain.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the name of the crew member who must be the <span class="tex-span"><i>i</i></span>-th one to leave the ship.</p>





```input1
6
Jack captain
Alice woman
Charlie man
Teddy rat
Bob child
Julia woman

```




```output1
Teddy
Alice
Bob
Julia
Charlie
Jack

```


