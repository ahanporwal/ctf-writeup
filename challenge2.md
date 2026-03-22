# Challenge: <QRecreate>

## Problem
I managed to bypass the IPS to exfiltrate the secrets you wanted from the target's intranet. I just hope you remember the encoding structure we agreed on. by Emmett

## Solution
Upon downloading the file, I notice a folder with 100 different folders, each having a different peculiar name. Each folder contained a part of a QR code. The first instinct was to try and make an algorithm to match up the edges of these 100 individual parts, and then merge them together. However, upon trying this, it was painstakingly difficult and the challenge seemed like it was intended to be solved in a different way. Upon taking a closer look at the folder names, they looked like base32/base64 encodings of something. Decrypting these in base64, it was found that the folders were named 1-100 with padded zeros, which was their order in the final image. All it took was a simple algorithm to reconstruct the image, scan the QR code and the decode the flag.

## Flag
utflag{s3cr3ts_@re_@lw@ys_w1th1n_s3cr3ts}
