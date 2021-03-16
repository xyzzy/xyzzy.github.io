---
layout: post
title: "Show HN: Smile - executable ASCII art (2011 remastered)"
---

*When ASCII art is the executable*

Executables consisting exclusively of alpha-numeric characters. The digits "0123456789" are used for dark, the letters "acemnorsuvwxz" for light.

Removing instructions that are not alpha-numerical, strips functionality down to the minimum:

- 4.5 of the 7 registers available (%bx, %si, %di, %bp, %ah)
- 4 of the ~80 instructions groups available (XOR,IMUL,CMP,Jcc)
- constant values start from 48, (only range 0x30-0x39,0x61-0x79)

By cosmic coincidence, the 2 instructions needed to jailbreak are available. On top of that, self-modifying code and radix13 encoding.

This should have been released a decade ago. As compensation, it has been remastered. The reward was making it 30% smaller. 

[https://news.ycombinator.com/item?id=26125820](https://news.ycombinator.com/item?id=26125820)
