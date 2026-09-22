# Rizwan Alam

Systems and telecom engineer at C-DOT since 2013. I write C/C++ and Rust on Linux, with a background in IMS, SIP and Diameter. My work sits where four areas meet: **telecom protocols**, **systems programming**, **systems security** and **AI agents**, with a focus on failure handling, bounded resource use and safe defaults.

## Engineering focus

- **Telecom:** SIP/VoIP, IMS and Diameter behaviour, routing and interworking with the 5G Core.
- **Systems programming:** C/C++ and Rust on Linux: concurrency, network I/O, kernel interfaces, parsers for untrusted input.
- **Security:** memory safety, Linux and TLS hardening, protocol input validation.
- **AI agents:** tool-using agents that always terminate, least-privilege tool registries, and defences against agent attacks (prompt injection, SSRF, exfiltration).

My public projects are separate from my professional deployment experience. Each repository states its implemented scope and remaining work; the older C repositories are coursework.

## Open-source contributions

Merged:

- [rsipstack #142](https://github.com/restsend/rsipstack/pull/142): typed Service-Route header (RFC 3608), with the route set retained from REGISTER.
- [rsipstack #143](https://github.com/restsend/rsipstack/pull/143): preload that route set as Route headers on out-of-dialog requests, with tests for ordering and default behaviour.

Open, under review:

- [Kamailio #4937](https://github.com/kamailio/kamailio/pull/4937): registrar and IMS S-CSCF registrar validate every Contact URI in REGISTER (the first Contact header was skipped).
- [Kamailio #4943](https://github.com/kamailio/kamailio/pull/4943): dialog module option to replicate the timeout-BYE flag over DMQ, for HA pairs.
- [curl-rust #663](https://github.com/alexcrichton/curl-rust/pull/663): fix an i32 overflow in `Multi::timeout_i32`, with boundary tests.
- [hampi #145](https://github.com/ystero-dev/hampi/pull/145): ASN.1 compiler skips deriving `Eq` for types containing REAL.
- [aya #1716](https://github.com/aya-rs/aya/pull/1716), [#1717](https://github.com/aya-rs/aya/pull/1717): corrected eBPF object parser docs.

## Projects

**Telecom**

- [ims-5gc-iwf](https://github.com/rizwan3659/ims-5gc-iwf): IMS Diameter to 5G Core interworking in Rust: zero-copy Diameter codec, RFC 6733 peer state machine, declarative translation rules, NRF discovery, integration tests. The README lists the remaining work.
- [ro-camel-iwf](https://github.com/rizwan3659/ro-camel-iwf): Diameter Ro to CAMEL CAP v2 charging prototype in Rust, with a charging state machine and an in-process simulator. CAP wire transport and HA are not built yet.
- [sip-rtp-diagnostics](https://github.com/rizwan3659/sip-rtp-diagnostics): offline SIP/RTP capture diagnostics in C with bounded PCAP parsing. Initial scope.

**Systems programming**

- [linux-kernel-eventqueue](https://github.com/rizwan3659/linux-kernel-eventqueue): kernel lab: bounded misc-device queue with blocking I/O, poll and backpressure. Runtime VM validation is pending.
- [IPC](https://github.com/rizwan3659/IPC), [IITD kernel assignments](https://github.com/rizwan3659/IITD_kernel_assignments): older C coursework.

**Security**

- [agent-security-lab](https://github.com/rizwan3659/agent-security-lab): six agent attacks (eval RCE, path traversal, SSRF, excess privilege, prompt injection, secret exfiltration), each shown against vulnerable code and blocked by hardened code, as a test suite.
- [linux-hardening-audit](https://github.com/rizwan3659/linux-hardening-audit): Python checks for Linux hardening settings, with offline rule tests.
- [tls-audit](https://github.com/rizwan3659/tls-audit): Python checks for TLS and certificate configuration.

**AI agents**

- [agentkit-rs](https://github.com/rizwan3659/agentkit-rs): small Rust agent framework: step-bounded loop, tool failure returned as data, SSRF-hardened HTTP tool, execution tracing.
- [agentkit-py](https://github.com/rizwan3659/agentkit-py): the same design in Python, with no dependencies.

[LinkedIn](https://www.linkedin.com/in/rizwan-alam-03304636/)
