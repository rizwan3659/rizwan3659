# Rizwan Alam

**Senior systems and telecom engineer | C/C++, Rust, Linux networking | IMS, IPsec/XFRM | Performance and reliability**

I have worked at C-DOT since 2013, building telecom software across IMS, SIP, Diameter and charging integration. My focus is understanding protocol behaviour, debugging failures across components, and making Linux services reliable under load.

## Engineering focus

- **Linux networking and systems:** C/C++, Rust, concurrency, network I/O, IPC and kernel interfaces, including IPsec/XFRM.
- **Telecom integration:** SIP/VoIP, IMS, Diameter and charging state machines; tracing call flows and handling peer failures.
- **Performance and reliability:** bounded queues, backpressure, timeout handling, profiling and reproducible tests.
- **Systems security:** memory safety, protocol input validation, Linux hardening and TLS configuration.

My public projects are separate from my professional deployment experience. I distinguish prototypes, lab measurements and tested behaviour from production claims.

## Selected engineering projects

- **[xfrm-async-sa](https://github.com/rizwan3659/xfrm-async-sa)** — C userspace control of Linux IPsec SAs over NETLINK_XFRM. Compares synchronous installation with a windowed pipeline. The [review and study guide](https://github.com/rizwan3659/xfrm-async-sa/pull/1) add ACK-correlation, timeout and cleanup fixes with mock, sanitizer and real-kernel namespace tests. This is kernel-interface programming, not a kernel module or a full IPsec controller.
- **[ims-5gc-iwf](https://github.com/rizwan3659/ims-5gc-iwf)** — IMS Diameter to 5G Core service interworking in Rust, with a codec, routing, translation rules and integration tests. See the README for implemented scope and remaining work.
- **[linux-kernel-eventqueue](https://github.com/rizwan3659/linux-kernel-eventqueue)** — C kernel lab: a bounded misc-device queue with blocking I/O, poll and backpressure. Runtime VM validation remains pending.
- **[ro-camel-iwf](https://github.com/rizwan3659/ro-camel-iwf)** — Rust IMSCAP charging prototype connecting TAS Diameter Ro semantics to CAMEL CAP v2. Includes a charging state machine and simulator; CAP wire transport and clustered HA remain unimplemented.
- **[sip-rtp-diagnostics](https://github.com/rizwan3659/sip-rtp-diagnostics)** — C capture-analysis lab with bounded PCAP parsing and RTP diagnostics. Initial scope is documented in the repository.
- **[linux-hardening-audit](https://github.com/rizwan3659/linux-hardening-audit)** and **[tls-audit](https://github.com/rizwan3659/tls-audit)** — Python assessment tools with offline tests for Linux and TLS configuration rules.

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

## Further experiments and coursework

I also explore tool-execution safety in [agent-security-lab](https://github.com/rizwan3659/agent-security-lab) and small agent frameworks in [Rust](https://github.com/rizwan3659/agentkit-rs) and [Python](https://github.com/rizwan3659/agentkit-py). These are secondary experiments alongside my systems and telecom work.

[IPC](https://github.com/rizwan3659/IPC) and [IITD kernel assignments](https://github.com/rizwan3659/IITD_kernel_assignments) are older C coursework.

[LinkedIn](https://www.linkedin.com/in/rizwan-alam-03304636/)
