## Description

<div><center> <img class="tex-graphics" src="file://7WNXVQrB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It's the end of July&nbsp;– the time when a festive evening is held at Jelly Castle! Guests from all over the kingdom gather here to discuss new trends in the world of confectionery. Yet some of the things discussed here are not supposed to be disclosed to the general public: the information can cause discord in the kingdom of Sweetland in case it turns out to reach the wrong hands. So it's a necessity to not let any uninvited guests in.</p><p>There are 26 entrances in Jelly Castle, enumerated with uppercase English letters from <span class="tex-font-style-tt">A</span> to <span class="tex-font-style-tt">Z</span>. Because of security measures, each guest is known to be assigned an entrance he should enter the castle through. The door of each entrance is opened right before the first guest's arrival and closed right after the arrival of the last guest that should enter the castle through this entrance. No two guests can enter the castle simultaneously.</p><p>For an entrance to be protected from possible intrusion, a candy guard should be assigned to it. There are <span class="tex-span"><i>k</i></span> such guards in the castle, so if there are more than <span class="tex-span"><i>k</i></span> opened doors, one of them is going to be left unguarded! Notice that a guard can't leave his post until the door he is assigned to is closed.</p><p>Slastyona had a suspicion that there could be uninvited guests at the evening. She knows the order in which the invited guests entered the castle, and wants you to help her check whether there was a moment when more than <span class="tex-span"><i>k</i></span> doors were opened.</p></div><div class="input-specification"><p>Two integers are given in the first string: the number of guests <span class="tex-span"><i>n</i></span> and the number of guards <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p><p>In the second string, <span class="tex-span"><i>n</i></span> uppercase English letters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> are given, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the entrance used by the <span class="tex-span"><i>i</i></span>-th guest.</p></div><div class="output-specification"><p>Output «<span class="tex-font-style-tt">YES</span>» if at least one door was unguarded during some time, and «<span class="tex-font-style-tt">NO</span>» otherwise.</p><p>You can output each letter in arbitrary case (upper or lower).</p></div>

## Input

<p>Two integers are given in the first string: the number of guests <span class="tex-span"><i>n</i></span> and the number of guards <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p><p>In the second string, <span class="tex-span"><i>n</i></span> uppercase English letters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> are given, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the entrance used by the <span class="tex-span"><i>i</i></span>-th guest.</p>

## Output

<p>Output «<span class="tex-font-style-tt">YES</span>» if at least one door was unguarded during some time, and «<span class="tex-font-style-tt">NO</span>» otherwise.</p><p>You can output each letter in arbitrary case (upper or lower).</p>





```input1
5 1
AABBB

```




```input2
5 1
ABABB

```




```output1
NO

```




```output2
YES

```



## Note

<p>In the first sample case, the door A is opened right before the first guest's arrival and closed when the second guest enters the castle. The door B is opened right before the arrival of the third guest, and closed after the fifth one arrives. One guard can handle both doors, as the first one is closed before the second one is opened.</p><p>In the second sample case, the door B is opened before the second guest's arrival, but the only guard can't leave the door A unattended, as there is still one more guest that should enter the castle through this door. </p>
