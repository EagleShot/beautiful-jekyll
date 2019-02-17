---
layout: post
title: Tivoization:GPLv2 and GPLv3
categories: Senior_Seminar
---
The GNU General Public License (or GPL) is one of the most common licenses in FOSS projects. It has been crucial in establishing the FOSS ecosystem and keeping projects FOSS with its strict copyleft language (a codebase that uses GPL code has to be GPL). It requires the code base to be open source and grants others the right to redistribute and modify the software.

A vendor found a loophole in the license. The used the Linux kernel to build an operating system for their DVR and released its code as open source, but they digitally signed their version and thus prevented others from running a modified version of the OS in their DVRs. Thus the term Tivoization was created as TiVo sold the DVRs.

Richard Stallman, the Free Software Foundation and several other FOSS advocates found this unacceptable that hardware patents were used to prevent modification to the hardware without which the restrictions to the software could not be removed. Digital signatures were used to provide security, but this time it was to curtail freedom. The code was released under GPLv2. Thus GPLv3 was born. It includes many modifications that help with compatibility with other licenses and a host of other features, but one of its primary goals to prevent Tivoization.

GPLv3 contains language that grants users the required patent rights to use and modify the code:
>The GPLv3 contains an explicit patent license, according to which people who license a program under the GPL license both copyrights as well as patents to the extent that this is necessary to use the code licensed by them.  A comprehensive patent license is not thereby granted.  Furthermore, the new patent clause attempts to protect the user from the consequences of agreements between patent owners and licensees of the GPL that only benefit some of the licensees (corresponding to the Microsoft/Novell deal).  The licensees are required to ensure that every user enjoys such advantages (patent license or release from claims), or that no one can profit from them.
[Source](http://www.ifross.org/en/what-difference-between-gplv2-and-gplv3)

Linus Torvalds argues against the restriction that GPLv3 imposes. The supports digital signatures and the strategy used by TiVo as he believes that some systems need to be protected from modification (eg safe internet search for kids). As long as it is possible to use a modified version of the code base in *any* system and not necessarily the same system the code was made for, it is acceptable. The Linux kernel is still in GPLv2. Linus argues that anti-Tivoization is taking away freedom from the manufactures who are also customers and he does not want any freedom to be taken away for the Linux kernel.
