# Rizwan Alam

I am a systems and telecom engineer at C-DOT, where I have worked since 2013. My focus is C/C++ and Rust software on Linux, with a background in IMS, SIP and Diameter. I am interested in protocol integration, debugging, concurrency and failure handling.

## Engineering focus

- SIP/VoIP and Diameter protocol behaviour, routing and integration.
- C/C++ and Rust systems programming on Linux, including concurrency and network communication.
- Reliability and systems security: explicit failure handling, regression tests, memory safety and bounded resource use.

My public projects are separate from my professional deployment experience. The telecom repositories document their implemented scope and remaining work; the older C repositories are coursework.

## C and Rust telecom contributions

Two of my changes to [rsipstack](https://github.com/restsend/rsipstack), a Rust SIP stack, were merged upstream:

- [Service-Route support (#142)](https://github.com/restsend/rsipstack/pull/142): parse the SIP header and retain the route set returned during registration.
- [Preloaded routing (#143)](https://github.com/restsend/rsipstack/pull/143): use that route set on outgoing requests, with tests for ordering and the default behaviour.

C contribution in progress: [Kamailio #4937](https://github.com/kamailio/kamailio/pull/4937) proposes rejecting malformed SIP Contact URIs during REGISTER handling in the registrar and IMS S-CSCF registrar modules. This PR is open, not merged.

## Projects and exercises

- [ro-camel-iwf](https://github.com/rizwan3659/ro-camel-iwf) — IMSCAP interworking prototype in Rust: TAS Diameter Ro to CAMEL CAP v2. Includes a charging state machine and an in-process simulator; CAP wire transport and clustered failover remain to be implemented.

- [ims-5gc-iwf](https://github.com/rizwan3659/ims-5gc-iwf) — Diameter-to-5G Core service interworking in Rust. Includes a protocol codec, routing, translation rules and integration tests. The README lists remaining integration work.
- [IPC](https://github.com/rizwan3659/IPC) — C client/server exercises using UNIX domain sockets, FIFOs and System V message queues.
- [IITD kernel assignments](https://github.com/rizwan3659/IITD_kernel_assignments) — older C coursework, including scheduler changes and system-call experiments.
- [linux-hardening-audit](https://github.com/rizwan3659/linux-hardening-audit) — Python checks for Linux hardening settings, with offline rule tests.
- [tls-audit](https://github.com/rizwan3659/tls-audit) — Python tooling for TLS and certificate configuration checks.

The coursework repositories are learning exercises; they are separate from my professional telecom work.

[LinkedIn](https://www.linkedin.com/in/rizwan-alam-03304636/)