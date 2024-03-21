---
homepage:
  - https://ebpf.io/
aliases:
  - extended Berkeley Packet Filter
tags:
  - linux
  - kernel
---
- Process:
	- C code compiled to intermediate bytecode
		- BPF Compiler Collection (BCC)
		- bpftrace
	- Attached to kernel hooks
	- Bytecode is then verified and compiled [[JIT]]
- Kernel knowledge necessary