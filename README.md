# Semeru
Semeru: A Memory-Disaggregated Managed Runtime (OSDI 2020)

## Summary of Semeru  
Resource-disaggregated architectures have risen in popularity for large datacenters. However, prior disaggregation systems are designed for native applications; in addition, all of them require applications to possess excellent locality to be efficiently executed. In contrast, programs written in managed languages are subject to periodic garbage collection (GC), which is a typical graph workload with poor locality. Although most datacenter applications are written in managed languages, current systems are far from delivering acceptable performance for these applications.

This paper presents Semeru, a distributed JVM that can dramatically improve the performance of managed cloud applications in a memory-disaggregated environment. Its design possesses three major innovations: (1) a universal Java heap, which provides a unified abstraction of virtual memory across CPU and memory servers and allows any legacy program to run without modifications; (2) a distributed GC, which offloads object tracing to memory servers so that tracing is performed closer to data; and (3) a swap system in the OS kernel that works with the runtime to swap page data efficiently. An evaluation of Semeru on a set of widely-deployed systems shows very promising results.
## Team 
This project is done in collaboration with Professor [Harry Xu](http://web.cs.ucla.edu/~harryxu/)'s group at UCLA. Please visit [Semeru project at UCLA Systems](https://github.com/uclasystem/Semeru).

https://github.com/uclasystem/Semeru

## How to cite 
Please refer to our OSDI'20 paper, [Semeru: A Memory-Disaggregated Managed Runtime](https://www.usenix.org/conference/osdi20/presentation/wang) for more details. 
### Bibtex  
@inproceedings {258846,
author = {Chenxi Wang and Haoran Ma and Shi Liu and Yuanqi Li and Zhenyuan Ruan and Khanh Nguyen and Michael D. Bond and Ravi Netravali and Miryung Kim and Guoqing Harry Xu},
title = {Semeru: A Memory-Disaggregated Managed Runtime},
booktitle = {14th {USENIX} Symposium on Operating Systems Design and Implementation ({OSDI} 20)},
year = {2020},
isbn = {978-1-939133-19-9},
pages = {261--280},
url = {https://www.usenix.org/conference/osdi20/presentation/wang},
publisher = {{USENIX} Association},
month = nov,
}

## Video
You can watch a OSDI'20 presentation video [here](https://youtu.be/MFA3MmNDKaM)
 
