# Changelog

All notable changes to the `zk_verifier` contract are documented here.
Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [0.2.0](https://github.com/Sundriveauto/Ledgerlens-core/compare/zk-verifier-v0.1.0...zk-verifier-v0.2.0) (2026-10-03)


### Features

* harden model loading, contract fuzz gate, SLO alerts, and metric cardinality ([#1077](https://github.com/Sundriveauto/Ledgerlens-core/issues/1077)) ([301afc8](https://github.com/Sundriveauto/Ledgerlens-core/commit/301afc8a5232ee8ba3238b7efce37b08a5b9bb30)), closes [#1000](https://github.com/Sundriveauto/Ledgerlens-core/issues/1000) [#1001](https://github.com/Sundriveauto/Ledgerlens-core/issues/1001) [#1002](https://github.com/Sundriveauto/Ledgerlens-core/issues/1002) [#1003](https://github.com/Sundriveauto/Ledgerlens-core/issues/1003)
* implement overlapping validity secret rotation for keys and web… ([b0ea0d8](https://github.com/Sundriveauto/Ledgerlens-core/commit/b0ea0d8f4ddf936214b79ff951aa31b74f335f8f))
* zk-snark backend ([cd79d5c](https://github.com/Sundriveauto/Ledgerlens-core/commit/cd79d5c6d511d9f19083bf88ca5dc8f81d5bfaad))
* zk-snark backend ([c2dae81](https://github.com/Sundriveauto/Ledgerlens-core/commit/c2dae8154cce8a772ec5742909c7ad1b6cccbf56))


### Bug Fixes

* cargo-fuzz manifests can't inherit workspace.dependencies from themselves ([f46e9b3](https://github.com/Sundriveauto/Ledgerlens-core/commit/f46e9b3afb469b45ddb5fd024402c5f1fdd6459f))
* **contracts:** make both Soroban crates build and test again ([c1ad377](https://github.com/Sundriveauto/Ledgerlens-core/commit/c1ad377f47b4c102df0eb5a2bb6fd1f295352b36))
* distributed per-API-key rate limiting shared by REST and gRPC ([2e1f791](https://github.com/Sundriveauto/Ledgerlens-core/commit/2e1f79106719c4b3f64765a439bb3c09f037c4a5))
* enable testutils feature and fix asset_pair type in fuzz harnesses ([8b98f63](https://github.com/Sundriveauto/Ledgerlens-core/commit/8b98f63416ca9d70e81c732ced317b9d1ea40195))
* pin ed25519-dalek/rand/rand_core in contract manifests for fuzz build ([dcf69dd](https://github.com/Sundriveauto/Ledgerlens-core/commit/dcf69dd4b9d5b5fc882b67867c2adbe2c04da566))
* resolve zk_verifier build errors by adding Fq::is_valid and converting from_bytes calls ([5e63d60](https://github.com/Sundriveauto/Ledgerlens-core/commit/5e63d605257173b9d95923f36b26e6d79ed83fae))
* store admin identity for ZkVerifier submit_score ([a8c9182](https://github.com/Sundriveauto/Ledgerlens-core/commit/a8c91826780921c056d858f0926fb6979832e80a))
* **zk_verifier:** correct Fp12 inversion (pairing) for BN254 pairing ([0e90ec3](https://github.com/Sundriveauto/Ledgerlens-core/commit/0e90ec3b83c33c799281b270501a1254ed3f5884))
* **zk_verifier:** correct Fp12 inversion so BN254 pairing works ([f053da1](https://github.com/Sundriveauto/Ledgerlens-core/commit/f053da14065c8a9c13643393f5e90dbbbeb6b944))
* **zk_verifier:** make contract compile and actually verify proofs ([390ff46](https://github.com/Sundriveauto/Ledgerlens-core/commit/390ff46fcebaf2379dc3c907b9df987faf4cd51f))
* **zk_verifier:** make contract compile and actually verify proofs ([bbc4958](https://github.com/Sundriveauto/Ledgerlens-core/commit/bbc4958a44e622837e70a10388606ce6b52e42c8))


### Documentation

* clarify Alembic workflow and zk test fixtures ([d753bc4](https://github.com/Sundriveauto/Ledgerlens-core/commit/d753bc4c61fc9f7710c4a24bbc22163f5cfd01e2))
* clarify migrations and zk test fixtures ([4849396](https://github.com/Sundriveauto/Ledgerlens-core/commit/484939625a6d9272d85a900c537f497f9789561f))
* cross-link ZK score-threshold proof system components ([8d4d972](https://github.com/Sundriveauto/Ledgerlens-core/commit/8d4d972b58599d346981434548c8014ace11b05e))
* cross-link ZK score-threshold proof system components ([a876cd9](https://github.com/Sundriveauto/Ledgerlens-core/commit/a876cd9c23533d7d6068d6f3a2f72c2e8e80ec4d))
* document Docker build steps, panic messages, and add CHANGELOGs ([#791](https://github.com/Sundriveauto/Ledgerlens-core/issues/791), [#792](https://github.com/Sundriveauto/Ledgerlens-core/issues/792), [#793](https://github.com/Sundriveauto/Ledgerlens-core/issues/793), [#794](https://github.com/Sundriveauto/Ledgerlens-core/issues/794)) ([3325df4](https://github.com/Sundriveauto/Ledgerlens-core/commit/3325df4c536bb183e36b8881d522b73277915d07))
* document Docker build steps, panic messages, and add CHANGELOGs… ([c229d88](https://github.com/Sundriveauto/Ledgerlens-core/commit/c229d882a2848eef62b5201b43170491a5f0179e))


### CI

* build and test both Soroban contract crates on every push and PR ([a481cbf](https://github.com/Sundriveauto/Ledgerlens-core/commit/a481cbf5afc3a187dfc85ae70288acec25716f6a))

## [Unreleased]

### Fixed
- Made the contract compile and actually verify proofs.
- Resolved build errors by adding Fq::is_valid and fixing from_bytes conversions.
- Pinned ed25519-dalek/rand/rand_core versions in contract manifests for fuzz build.
- Enabled testutils feature and fixed harness types for fuzzing.

### Added
- Implemented zero-knowledge risk score proofs.
- Built a fuzzing and symbolic-execution harness for the Soroban contract.
- Added zk-SNARK backend.
