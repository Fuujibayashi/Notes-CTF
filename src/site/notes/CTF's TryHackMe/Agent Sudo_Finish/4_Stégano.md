---
{"dg-home":true,"dg-publish":true,"permalink":"/ctf-s-try-hack-me/agent-sudo-finish/4-stegano/","tags":"gardenEntry","dgHomeLink":true,"dgPassFrontmatter":true}
---


### Binwalk

``binwalk cute-alien.jpg 

DECIMAL       HEXADECIMAL     DESCRIPTION
0             0x0             JPEG image data, JFIF standard 1.01

____________________________________________

``binwalk cutie.png 

DECIMAL       HEXADECIMAL     DESCRIPTION
0             0x0             PNG image, 528 x 528, 8-bit colormap, non-interlaced
869           0x365           Zlib compressed data, best compression
34562         0x8702          Zip archive data, encrypted compressed size: 98, uncompressed size: 86, name: To_agentR.txt
34820         0x8804          End of Zip archive, footer length: 22

_________________________________________________
``binwalk + namefile -e / Extrait le zip

_________________________________________________

### Steghide

``steghide --extract -sf cute-alien.jpg -p Area51 -v

Ecriture des données extraites dans "message.txt"... terminé.

___________________________________
``cat message.txt

*Hi james,
Glad you find this message. Your login password is **hackerrules** !
Don't ask me why the password look cheesy, ask agent R who set this password for you.
Your buddy,
chris 
_______________________________

### Reverse Image
Reverse "Autospy.jpg" => Roswell Alien Autopsy