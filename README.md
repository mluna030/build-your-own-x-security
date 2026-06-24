# Build Your Own X — Security Edition

This repository is a compilation of well-written, step-by-step guides for re-creating security tools from scratch. Modeled on [build-your-own-x](https://github.com/codecrafters-io/build-your-own-x); the one difference is that every link here is verified and human-reviewed before it lands.

> *What I cannot create, I do not understand — Richard Feynman.*

It's a great way to learn. You understand a port scan far better after writing one than after reading about nmap, and each topic pairs an offensive build with its defensive counterpart where it makes sense.

For learning, authorized testing, CTFs, and defensive work only — build and run offensive projects against targets you own or are authorized to test, never against systems you are not.

New to the plumbing (sockets, binary formats, protocols)? Build the primitive first from the original build-your-own-x: the [Network Stack](https://github.com/codecrafters-io/build-your-own-x#build-your-own-network-stack), [Programming Language](https://github.com/codecrafters-io/build-your-own-x#build-your-own-programming-language), and [Web Server](https://github.com/codecrafters-io/build-your-own-x#build-your-own-web-server) tracks underpin most of what is here.

* [Port Scanner](#build-your-own-port-scanner)
* [Packet Sniffer](#build-your-own-packet-sniffer)
* [Fuzzer](#build-your-own-fuzzer)
* [Debugger](#build-your-own-debugger)
* [Intrusion Detection System](#build-your-own-intrusion-detection-system)
* [Password Cracker / Hashing](#build-your-own-password-cracker--hashing)
* [TLS / Cryptography](#build-your-own-tls--cryptography)
* [Binary Parser / Disassembler](#build-your-own-binary-parser--disassembler)
* [Honeypot](#build-your-own-honeypot)
* [C2 / EDR](#build-your-own-c2--edr)
* [Offensive Tooling](#build-your-own-offensive-tooling)* [Sandbox / Container](#build-your-own-sandbox--container)
* [Bytecode VM](#build-your-own-bytecode-vm)
* [UEFI / Bootloader](#build-your-own-uefi--bootloader)

## Contributing

Found a great from-scratch tutorial that's missing? Two ways to add it:

- Open an issue with the **Suggest a tutorial** form — no git required.
- Or fork, add your entry in the `* [**Language**: _Title_](url)` format, and open a pull request.

Entries must be written tutorials or courses with real code, not bare repos, libraries, or tool walkthroughs. See [CONTRIBUTING.md](CONTRIBUTING.md) for the full rules.

## Tutorials

#### Build your own `Port Scanner`

* [**Python**: _Building a Custom Port Scanner from Scratch_](https://blog.shellnetsecurity.com/posts/2025/building-custom-port-scanner-python/)
* [**Python**: _How to Make a Port Scanner in Python_](https://thepythoncode.com/article/make-port-scanner-python)

#### Build your own `Packet Sniffer`

* [**C**: _Programming with pcap_](https://www.tcpdump.org/pcap.html)
* [**Rust**: _Implementing a Packet Sniffer in Rust_](https://github.com/HighlyExistant/Packet-Sniffer)

#### Build your own `Fuzzer`

* [**Python**: _Writing a Simple Fuzzer from Scratch_](https://carstein.github.io/fuzzing/2020/04/18/writing-simple-fuzzer-1.html)
* [**Rust**: _Diving Into Coverage-Guided Fuzzing_](https://pierrezemb.fr/posts/diving-into-coverage-guided-fuzzing/)
#### Build your own `Debugger`

* [**C**: _How Debuggers Work: Part 1_](https://eli.thegreenplace.net/2011/01/23/how-debuggers-work-part-1)
* [**C**: _Demystifying ptrace: Building a Custom Debugger_](https://michaellaplante.com/blog/2026-05-24-demystifying-ptrace-building-a-custom-debugger-for-linux-binaries/)
* [**C++**: _Writing a Linux Debugger_](https://tartanllama.xyz/writing-a-linux-debugger-setup/)
* [**Rust**: _A Comprehensive Guide to System Call Tracing in Rust_](https://jakobwaibel.com/writing/ptrace/)

#### Build your own `Intrusion Detection System`

* [**Python**: _Build a Real-Time Intrusion Detection System_](https://www.freecodecamp.org/news/build-a-real-time-intrusion-detection-system-with-python/)
_Thin: the available guides lean on Scapy and scikit-learn rather than from-scratch packet inspection._

#### Build your own `Password Cracker / Hashing`

* [**Python**: _Build Your First Password Cracker_](https://dev.to/scofieldidehen/build-your-first-password-cracker-37ob)
* [**Rust**: _How to Hash Passwords in Rust (bcrypt, argon2)_](https://www.rustfaq.org/en/how-to-hash-passwords-in-rust-bcrypt-argon2/)

_Thin: no verified from-scratch bcrypt or argon2 implementation yet._

#### Build your own `TLS / Cryptography`

* [**Any**: _The Cryptopals Crypto Challenges_](https://cryptopals.com/)
* [**Reference**: _The Illustrated TLS 1.3 Connection_](https://tls13.xargs.org/)
* [**Reference**: _The Illustrated TLS 1.2 Connection_](https://tls12.xargs.org/)

#### Build your own `Binary Parser / Disassembler`

* [**C#**: _Creating an ELF from Scratch_](https://exploding-kitten.com/2025/04-elf-from-scratch)
_Thin: PE parsing and disassembly are not yet covered from scratch._

#### Build your own `Honeypot`

* [**Python**: _Build a Honeypot in Python_](https://www.freecodecamp.org/news/build-a-honeypot-with-python/)
* [**Rust**: _Building a Honeypot in Rust_](https://rust-trends.com/posts/building-a-honeypot-in-rust-and-deploy-it-to-oracle-for-free/)

#### Build your own `C2 / EDR`

* [**C**: _Build a Load Balancer with eBPF and XDP_](https://oneuptime.com/blog/post/2026-01-07-ebpf-xdp-load-balancer/view)
* [**C / C++**: _eBPF Developer Tutorial_](https://github.com/eunomia-bpf/bpf-developer-tutorial)
* [**C++**: _eBPF Security Programming: Beyond Hello World_](https://t0x1n.cc/posts/ebpf-security-programming-beyond-hello-world/)
* [**Go**: _Building a Real-Time Process Monitor with eBPF and Go_](https://ebpfchirp.substack.com/p/building-a-real-time-process-monitor)
* [**Go**: _Getting Started with cilium/ebpf_](https://ebpf-go.dev/guides/getting-started/)
* [**Rust**: _Writing an eBPF Tracepoint Program with Rust and Aya_](https://yuki-nakamura.com/2024/07/06/writing-ebpf-tracepoint-program-with-rust-aya-tips-and-example/)
#### Build your own `Offensive Tooling`

_Lab and authorized engagements only. Build these to understand and detect offensive tradecraft, not to deploy it._

* [**Rust**: _Rust for Malware Development_](https://bishopfox.com/blog/rust-for-malware-development)

#### Build your own `Sandbox / Container`

* [**C++**: _I Built a Container Runtime from Scratch in C++_](https://kaizakin.site/blogs/container-runtime-from-scratch)
* [**Go**: _Building a Homemade Container from Scratch with Go_](https://abdelouahabmbarki.com/building-a-homemade-container-with-go/)
* [**Rust**: _Building a Container from Scratch in Rust_](https://brianshih1.github.io/mini-container/)

#### Build your own `Bytecode VM`

* [**C**: _Crafting Interpreters: A Bytecode Virtual Machine_](https://craftinginterpreters.com/a-bytecode-virtual-machine.html)
* [**Go**: _Building a Minimal Virtual Machine in Go_](https://paoloo.github.io/2026/01/11/building-a-small-vm-in-go/)
* [**Rust**: _Create Your Own Programming Language: the Virtual Machine_](https://createlang.rs/01_calculator/vm.html)

#### Build your own `UEFI / Bootloader`

* [**Assembly**: _Writing My Own Boot Loader_](https://dev.to/frosnerd/writing-my-own-boot-loader-3mld)
* [**Assembly**: _Building a Bootloader from Scratch: an x86 Assembly Guide_](https://dev.to/aayushgid/building-a-bootloader-from-scratch-an-x86-assembly-guide-fpi)
* [**Rust**: _Creating a Bootloader from Scratch: RustyBoot_](https://dev.to/kushalmeghani1644/creating-a-boot-loader-from-scratch-meet-rustyboot-2n82)
