# What Is An IPVM?

To date, IPFS has been a project focused on data. IPVM is a specification for bringing content-addressed execution to content-addressed data on IPFS. To this end, the IPVM spec aims to be the easiest, fastest, most secure, and open way to run decentralized compute jobs everywhere.

Another way to describe IPVM would be "an open, decentralized, and local-first competitor to AWS Lambda".

The project leverages Wasm, content addressing, SPKI, and object capabilities to liberate computation from depending on specific prenegotiated services like the big cloud providers. Execution should scale flexibly from on-device by default all the way up to edge PoPs and data centers.

## 📋 High-Level Attributes

* Wasm-on-IPFS
* Declarative invocation (not an ABI, see section below)
* Captured results, re-ingested to IPFS
* A distributed scheduler
  * Single vs cron, local vs remote vs either, etc
* Matchmaking
  * Poster/acceptor 
  * Push-to-remote
* (Global) memoization table & adaptive optimization
* Managed effects (via an IPVM runtime)
* Mobile (ambient) computing, compute-to-data, and data-to-compute
* "The HTTP of Compute"
* Stretch: autonomous agents

# Implementations and Interop

* [Bacalhau](https://bacalhau.org)
* [Homestar](https://github.com/ipvm-wg/homestar/)
* [Web3Storage](https://web3.storage/)

# :no_good_woman: Antigoals: What An IPVM Is Not

* A replacement of IPFS internals — that's wasm-ipfs
* A language for distributed applications
* A WASI interface
* A new blockchain

## 🤹 Separate Projects

1. Autocodec
2. wasm-ipfs
3. IPVM

These are related, but separate. The relatedness comes from the fact that if we have one Wasm engine in IPFS, then the other components can rely on it too.

## 👩‍💻 Get Involved

* [Community Calls](https://lu.ma/ipvm)

## External Ressources

- [IPVM High-Level Spec](https://github.com/ipvm-wg/spec)
- [IPVM: The Long-Fabled Execution Layer](https://www.youtube.com/watch?v=3y1RB8wt_YY) by Brooklyn Zelenka
- [IPVM - IPFS and WASM](https://www.youtube.com/watch?v=rzJWk1nlYvs) by Brooklyn Zelenka
- [Breaking Down the Interplanetary Virtual Machine](https://fission.codes/blog/ipfs-thing-breaking-down-ipvm/)
- [IPVM Use Cases & System Designs](https://www.youtube.com/watch?v=FhwzEKNZEIA) by Juan Benet
- [Ucan-Invocation Spec](https://github.com/ucan-wg/invocation)
- [Homestar](https://github.com/ipvm-wg/homestar) - the core, Rust-based implementation of IPVM

- [Breaking Down the Interplanetary Virtual Machine](https://fission.codes/blog/ipfs-thing-breaking-down-ipvm/)
- [Ucan Invocation Spec](https://github.com/ucan-wg/invocation)
- [Homestar, the Rust-based implementation of IPVM](https://github.com/ipvm-wg/homestar)
