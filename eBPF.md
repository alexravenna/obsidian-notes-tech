---
aliases:
  - extended Berkeley Packet Filter
tags:
  - kernel
  - linux
homepage:
  - https://ebpf.io/
---
- Process:
	- C code compiled to intermediate bytecode
		- BPF Compiler Collection (BCC)
		- bpftrace
	- Attached to kernel hooks
	- Bytecode is then verified and compiled [[JIT]]
- Kernel knowledge necessary