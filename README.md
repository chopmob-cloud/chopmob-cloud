## AlgoVoi: the open substrate for agentic payments

We built the evidence layer that lets an agent payment, a credential, or an audit record mean the same thing no matter who issued it. We built it so others could use it.

Canonicalisation, receipts, settlement attestation, and verification, byte-for-byte cross-validated across 8 independent implementations in 8 languages, specified in the IETF, and running in production.

It is open. Apache-2.0. **Adopt it, reference us, and build whatever you are building on top of it.**

### Adopt the substrate (open, Apache-2.0)

- [Adopt the substrate](https://docs.algovoi.co.uk/canonicalisation-substrate), the invitation and what is open
- [`algovoi-substrate`](https://github.com/chopmob-cloud/algovoi-substrate), the core, Apache-2.0
- [Conformance vectors](https://github.com/chopmob-cloud/algovoi-jcs-conformance-vectors), 21 sets, 166 vectors, 832/832 byte-for-byte across 8 languages
- [IETF Internet-Drafts](https://datatracker.ietf.org/doc/draft-hopley-x402-canonicalisation-jcs-v1/), the normative specs
- [Adopters registry](https://docs.algovoi.co.uk/adopters), who is already building on it

The only ask the open core makes is the one the licence already makes: keep the NOTICE, name who authored the substrate. Then build.

### Already in the substrate, validated and built in

The capabilities being worked out across the agentic-payments ecosystem are already specified, shipped, and byte-for-byte validated here:

- freeze-at-acceptance mandate evaluation, admission-gated, with a settlement window a later mandate lapse cannot shorten
- the closed-enum signed cancellation receipt, with `EXPIRED` as the unambiguous terminal-lapse artifact
- a shared receipt envelope with a `receipt_type` discriminator (`authorization` or `cancellation`)
- content-addressed binding, JCS (RFC 8785) canonicalisation, and Ed25519 verification

Adopters get all of it. Our commitment: the substrate is maintained, and verifiable additions are ongoing. L2 builders are more than welcome.

### Substrate 2 (the enhanced, commercial tier)

Built on the same canonical evidence format and fully interoperable with the open substrate. Post-quantum receipts, zero-knowledge reputation, cross-issuer federation, and a self-serve on-premise bundle.

- [Substrate 2](https://docs.algovoi.co.uk/substrate-2), the commercial tier and what it adds
- [Application suite](https://api.algovoi.co.uk/suite-store), production apps you can license and run

Christopher Hopley / AlgoVoi
