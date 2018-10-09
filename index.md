---
title: Development of Scalable Communication Library with Technologies for Memory Saving and Runtime Optimization
---

# Team Description

* Pl: Takeshi Nanri (Kyushu University)
* co-Pl: Shinji Sumimoto (Fujitsu Ltd.) and Hidetomo Shibamura (ISIT)
* Research Period: 2011 - 2017
* Research website: [http://ace-project.kyushu-u.ac.jp/](http://ace-project.kyushu-u.ac.jp/)

# Published Software

* [Advanced Communication Primitives (ACP) Library](https://github.com/project-ace/ACP)

---

# PGAS-based Scalable Communication Library ACP, and it's Applications


## ACP (Advanced Communication Primitives): a PGAS-based Communication Library

ACP supports a communication model that transfers data via "Global Memory", that is a virtual memory space managed by the library. Each process can expose a region of its local memory to other processes by registering that region to the global memory.

![Global and Local Memory of ACP]({{ site.baseurl }}/images/1.png)

* Basic Layer: Global Memory Access Operations of ACP
-	Copy operation
Copy data from one place in the Global Memory to another. Internally, the library performs appropriate communication operations for each copy operation so that the data is transferred between corresponding registered regions of local memories.

-	Atomic operation
Permutation, increment/decrement and logarithmic operations, on the value stored in the specified place of the Global Memory.
