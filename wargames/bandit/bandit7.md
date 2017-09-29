---
layout: default
gamename: bandit
level: 7
---
Level Goal
----------
The password for the next level is stored **somewhere on the
server** and has all of the following properties:
-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

Commands you may need to solve this level
-----------------------------------------
ls, cd, cat, file, du, find, grep

<hr />

# Solution
```
find / -size 33c -group bandit6 -user bandit7 2>/dev/null
```
Password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
