---
layout: default
---

so how do i do level 1 anyway?
==============================

Finally! Some real reversing! Just what you tried retrograde for. If you picked
up anything from the last challenge, you should have tried `ls` and seen some
file called `checker`. If you tried to be a sensible person and `cat checker`,
you were rewarded with a ton of gibberish all at once. This is because `checker`
is a binary file, meaning it is meant to be read by machines instead of people,
and it is a well-known fact that computers are dumb and can't even speak
English.

However, the inherent English-ness of the program's creator often shines through
in the form of strings of text in the binary, and as luck would have it, unix
systems have a tool to list these, creatively called `strings`. Tragically, even
after you find or run this, your problems are still not over. The binary is
quite large, and manually searching through the strings proves an unpleasant and
time-consuming task. Our alert reader, will, however, notice a hint delivered
upon the first use of strings, and perhaps leverage their google-fu to find some
more enjoyable method of searching for the password.
