# Challenge: <Hidden in Plain Sight>

## Problem
We've heard tell of a hidden message that's been placed somewhere nearby. Can you find it?

## Solution
At first, the challenge seemed confusing because there was no file to download or message to decrypt. Upon further inspection, it was noticed that there was a unusual gap in the title, between "Hidden" and "in". Putting that in CyberChef, there were a lot of characters between those two words. Converting those characters to hexdump, it was obvious that there were hidden characters which had a repeating sequence within them, Upon researching the repeating sequence, it was found to be a special tag which made those characters invisible. Upon removing that tag and converting back from hexdump, the flag was indeed there in plain sight.

## Flag
utflag{1nv1s1bl3_un1c0d3}
