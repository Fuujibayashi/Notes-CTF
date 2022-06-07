---
{"dg-home":true,"dg-publish":true,"permalink":"/ctf-s-try-hack-me/agent-sudo-finish/5-zip/","tags":"gardenEntry","dgHomeLink":true,"dgPassFrontmatter":true}
---


``zip2john 8702.zip > zip.hashes 

``john zip.hashes

Using default input encoding: UTF-8
Loaded 1 password hash (ZIP, WinZip [PBKDF2-SHA1 128/128 AVX 4x])
Cost 1 (HMAC size) is 78 for all loaded hashes
Will run 2 OpenMP threads
Proceeding with single, rules:Single
Press 'q' or Ctrl-C to abort, almost any other key for status
Almost done: Processing the remaining buffered candidate passwords, if any.
Proceeding with wordlist:/usr/share/john/password.lst
``alien``            (8702.zip/To_agentR.txt)

__________________________
*Agent C,
We need to send the picture to 'QXJlYTUx' as soon as possible!
By,
Agent R*

QXJlYTUx = Area51 (base64)
_________________________________________

