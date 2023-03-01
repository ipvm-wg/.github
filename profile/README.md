# What Is An IPVM?

To date, IPFS has been a project focused on data. IPVM is a specification for bringing execution to content addresses data on IPFS. To this end, the IPVM spec aims to be the easiest, fastest, most secure, and open way to run decentralized compute jobs.

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

* Bacalhau
* Web3Storage
* Homestar

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
