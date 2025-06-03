Welcome flag:
First step ls, then saw the flag.txt file , then echo flag to get changes made.

Process hunter:
first step ls, then saw readme.md, saw that we need to check processes, so ran ps aux to check all processes, realised PID 1's cmd line had the flag, so executed the cmd ps -p 1 -o args to get it

Hidden in the crowd:
ls showed a bunch of random files, tried grep dcCTF{ * , to no avail, then realised hidden implies hidden files, ran ls -a , and saw the flag file.



