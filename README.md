# Rizwan Alam

I write systems and telecom software in C, C++ and Rust. I have worked at C-DOT since 2013, mainly on IMS and voice-network software. My interests include Linux internals, protocol implementation, concurrency and systems security.

## Rust and telecom contributions

Two of my changes to [rsipstack](https://github.com/restsend/rsipstack), a Rust SIP stack, were merged upstream:

- [Service-Route support (#142)](https://github.com/restsend/rsipstack/pull/142): parse the SIP header and retain the route set returned during registration.
- [Preloaded routing (#143)](https://github.com/restsend/rsipstack/pull/143): use that route set on outgoing requests, with tests for ordering and the default behaviour.

## Projects and exercises

- [ro-camel-iwf](https://github.com/rizwan3659/ro-camel-iwf) — IMSCAP interworking prototype in Rust: TAS Diameter Ro to CAMEL CAP v2. Includes a charging state machine and an in-process simulator; CAP wire transport and clustered failover remain to be implemented.

- [ims-5gc-iwf](https://github.com/rizwan3659/ims-5gc-iwf) — Diameter-to-5G Core service interworking in Rust. Includes a protocol codec, routing, translation rules and integration tests. The README lists remaining integration work.
- [IPC](https://github.com/rizwan3659/IPC) — C client/server exercises using UNIX domain sockets, FIFOs and System V message queues.
- [IITD kernel assignments](https://github.com/rizwan3659/IITD_kernel_assignments) — older C coursework, including scheduler changes and system-call experiments.
- [linux-hardening-audit](https://github.com/rizwan3659/linux-hardening-audit) — Python checks for Linux hardening settings, with offline rule tests.
- [tls-audit](https://github.com/rizwan3659/tls-audit) — Python tooling for TLS and certificate configuration checks.

The coursework repositories are learning exercises; they are separate from my professional telecom work.

[LinkedIn](https://www.linkedin.com/in/rizwan-alam-03304636/)