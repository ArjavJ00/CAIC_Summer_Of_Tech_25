Classic Caesar:
Would start with dcCTF{ , noticing gfFWI{ , meant a shift of 3. Applied decryption with a shift of -3 on an online site.

Oui Oui Secret:
Realised that it needs to be some other classical cipher. Started with vigenere. First tried doing it manually, struggled a bit. Then ended up using dCode's decryption, giving it the starting , dcCTF{ , and then just chose the obvious option.

Fair Enough:
Wordplay on Fair gives Playfair, so went ahead with it straight away. Again just used dCode's to decrypt it. 

XOR:
involved a bit more thought, but thankful to have gotten it fast enough. Realised that it was hex encoded, and should be split as 17 02 2d 30 .... . Converted them to integer to remove hex envryption, took the form 23 2 45 48 53 ...
Also , should start with dcCTF , corresponding ASCII being 100 99 67 84 70. Now from hint in qn title, our encryption works as message[i] ^ key[i] = crypted[i] , so we need to figure out key to decode whole string, on applying xor message[i] both sides 
for first 5 , we have key[i] = crypted[i] ^ message[i] , where we get the ASCII values of key[i] . Doing so gives 115 97 110 100 115, giving s a n d s , reasonably implying that sand is the key, and getting repeated. wrote code to 
figure the whole message. 

Hidden in Plain Sight:
Took so much time, couldnt get it without hint. Tried all the sites, and so many different techniques. RGB values of cells, File type analysis, tried to extract metadata, exif viewers etc. , nothing worked.

Chameleon Image:
While trying the same stuff for this as for the previous problem, I opened https://georgeom.net/StegOnline/checklist . Started trying all techniques out of desperation, and boom, got a hit on binwalk. 

Sound of Secrets:
Listened to the audio, felt like morse code, so generated spectrogram. Decoded Morse in that image as r34l fl4g dtc0y (smth like this), obv removed decoy, and first submitted r34l_fl4g, only to realise much later that it is meant to be
without an underscore :)

