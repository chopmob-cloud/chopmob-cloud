## AlgoVoi: the open substrate for agentic payments

We built the evidence layer that lets an agent payment, a credential, or an audit record mean the same thing no matter who issued it. We built it so others could use it.

Canonicalisation, receipts, settlement attestation, and verification, byte-for-byte cross-validated across ten independent implementations in ten languages, specified in the IETF, and running in production.

It is open. Apache-2.0. **Adopt it, reference us, and build whatever you are building on top of it.**

### Adopt the substrate (open, Apache-2.0)

- [Adopt the substrate](https://docs.algovoi.co.uk/canonicalisation-substrate), the invitation and what is open
- [`algovoi-substrate`](https://github.com/chopmob-cloud/algovoi-substrate), the core, Apache-2.0
- [Conformance vectors](https://github.com/chopmob-cloud/algovoi-jcs-conformance-vectors), 45 sets, 374 vectors, 1226/1226 byte-for-byte across ten languages
- [IETF Internet-Drafts](https://datatracker.ietf.org/doc/draft-hopley-x402-canonicalisation-jcs-v1/), the normative specs
- [Adopters registry](https://docs.algovoi.co.uk/adopters), who is already building on it

The only ask the open core makes is the one the licence already makes: keep the NOTICE, name who authored the substrate. Then build.

### Build on it with the Keystone toolchain (open, Apache-2.0)

The [Keystone](https://docs.algovoi.co.uk/keystone) composes the whole agentic trust chain (identity, authority, policy, decision, execution, verdict) into one recomputable sequence. The open Keystone tooling is how you build on the substrate. Start with the Control Panel:

- [The Keystone](https://docs.algovoi.co.uk/keystone), the trust chain and the `execution_ref` primitive
- [SDK and Control Panel](https://docs.algovoi.co.uk/keystone-sdk), the umbrella toolchain (`algovoi-keystone`) plus `algovoi-keystone-control`, the open browser Control Panel for installed bolt-ons
- [Runtime and journal](https://docs.algovoi.co.uk/keystone-runtime), run a chain and persist every reference to a tamper-evident journal
- [Agent layer](https://docs.algovoi.co.uk/keystone-agent), rules, triggers, and behaviours, each firing a `behaviour_ref`
- [Connect](https://docs.algovoi.co.uk/keystone-connect) and [Connectors](https://docs.algovoi.co.uk/keystone-connectors), bind live operations across databases, message buses, HTTP services, and object storage
- [Proof](https://docs.algovoi.co.uk/keystone-proof), offline verification against a published key

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
- [Verifiable Compliance Suite](https://docs.algovoi.co.uk/verifiable-compliance-suite), the verifiable long-term evidence estate for regulated records: 25 post-quantum-signed components on one perpetual licence, air-gap capable, no PyPI and no phone-home
- [`algovoi-vcs`](https://github.com/chopmob-cloud/algovoi-vcs), public documentation and the addon interfaces (`StorageBackend`, `Signer`) for the Verifiable Archive engine, so you can extend it with your own storage backend or key custodian
- [Application suite](https://api.algovoi.co.uk/suite-store), production apps you can license and run

Christopher Hopley / AlgoVoi
