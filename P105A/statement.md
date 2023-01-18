## Description

<div><p>In Disgaea as in most role-playing games, characters have skills that determine the character's ability to use certain weapons or spells. If the character does not have the necessary skill, he cannot use it. The skill level is represented as an integer that increases when you use this skill. Different character classes are characterized by different skills. </p><p>Unfortunately, the skills that are uncommon for the given character's class are quite difficult to obtain. To avoid this limitation, there is the so-called transmigration. </p><p>Transmigration is reincarnation of the character in a new creature. His soul shifts to a new body and retains part of his experience from the previous life. </p><p>As a result of transmigration the new character gets all the skills of the old character and the skill levels are reduced according to the <span class="tex-span"><i>k</i></span> coefficient (if the skill level was equal to <span class="tex-span"><i>x</i></span>, then after transmigration it becomes equal to <span class="tex-span">[<i>kx</i>]</span>, where <span class="tex-span">[<i>y</i>]</span> is the integral part of <span class="tex-span"><i>y</i></span>). If some skill's levels are <span class="tex-font-style-bf">strictly less</span> than <span class="tex-span">100</span>, these skills are forgotten (the character does not have them any more). After that the new character also gains the skills that are specific for his class, but are new to him. The levels of those additional skills are set to <span class="tex-span">0</span>. </p><p>Thus, one can create a character with skills specific for completely different character classes via transmigrations. For example, creating a mage archer or a thief warrior is possible. </p><p>You are suggested to solve the following problem: what skills will the character have after transmigration and what will the levels of those skills be?</p></div><div class="input-specification"><p>The first line contains three numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the number of skills the current character has, the number of skills specific for the class into which the character is going to transmigrate and the reducing coefficient respectively; <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are integers, and <span class="tex-span"><i>k</i></span> is a real number with exactly two digits after decimal point (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>, <span class="tex-span">0.01 ≤ <i>k</i> ≤ 0.99</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of which describes a character's skill in the form "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>exp</i></span>" — the skill's name and the character's skill level: <span class="tex-span"><i>name</i></span> is a string and <span class="tex-span"><i>exp</i></span> is an integer in range from <span class="tex-span">0</span> to <span class="tex-span">9999</span>, inclusive. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines each of which contains names of skills specific for the class, into which the character transmigrates. </p><p>All names consist of lowercase Latin letters and their lengths can range from <span class="tex-span">1</span> to <span class="tex-span">20</span> characters, inclusive. All character's skills have distinct names. Besides the skills specific for the class into which the player transmigrates also have distinct names.</p></div><div class="output-specification"><p>Print on the first line number <span class="tex-span"><i>z</i></span> — the number of skills the character will have after the transmigration. Then print <span class="tex-span"><i>z</i></span> lines, on each of which print a skill's name and level, separated by a single space. The skills should be given in the lexicographical order.</p></div>

## Input

<p>The first line contains three numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the number of skills the current character has, the number of skills specific for the class into which the character is going to transmigrate and the reducing coefficient respectively; <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are integers, and <span class="tex-span"><i>k</i></span> is a real number with exactly two digits after decimal point (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>, <span class="tex-span">0.01 ≤ <i>k</i> ≤ 0.99</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of which describes a character's skill in the form "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>exp</i></span>" — the skill's name and the character's skill level: <span class="tex-span"><i>name</i></span> is a string and <span class="tex-span"><i>exp</i></span> is an integer in range from <span class="tex-span">0</span> to <span class="tex-span">9999</span>, inclusive. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines each of which contains names of skills specific for the class, into which the character transmigrates. </p><p>All names consist of lowercase Latin letters and their lengths can range from <span class="tex-span">1</span> to <span class="tex-span">20</span> characters, inclusive. All character's skills have distinct names. Besides the skills specific for the class into which the player transmigrates also have distinct names.</p>

## Output

<p>Print on the first line number <span class="tex-span"><i>z</i></span> — the number of skills the character will have after the transmigration. Then print <span class="tex-span"><i>z</i></span> lines, on each of which print a skill's name and level, separated by a single space. The skills should be given in the lexicographical order.</p>





```input1
5 4 0.75
axe 350
impaler 300
ionize 80
megafire 120
magicboost 220
heal
megafire
shield
magicboost

```




```output1
6
axe 262
heal 0
impaler 225
magicboost 165
megafire 0
shield 0

```


