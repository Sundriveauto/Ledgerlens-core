# Changelog

All notable changes to the oracle_aggregator contract are documented here.
Format based on Keep a Changelog (https://keepachangelog.com/en/1.0.0/).

## [0.2.0](https://github.com/Sundriveauto/Ledgerlens-core/compare/oracle-aggregator-v0.1.0...oracle-aggregator-v0.2.0) (2026-10-03)


### Features

* harden model loading, contract fuzz gate, SLO alerts, and metric cardinality ([#1077](https://github.com/Sundriveauto/Ledgerlens-core/issues/1077)) ([301afc8](https://github.com/Sundriveauto/Ledgerlens-core/commit/301afc8a5232ee8ba3238b7efce37b08a5b9bb30)), closes [#1000](https://github.com/Sundriveauto/Ledgerlens-core/issues/1000) [#1001](https://github.com/Sundriveauto/Ledgerlens-core/issues/1001) [#1002](https://github.com/Sundriveauto/Ledgerlens-core/issues/1002) [#1003](https://github.com/Sundriveauto/Ledgerlens-core/issues/1003)


### Bug Fixes

* cargo-fuzz manifests can't inherit workspace.dependencies from themselves ([f46e9b3](https://github.com/Sundriveauto/Ledgerlens-core/commit/f46e9b3afb469b45ddb5fd024402c5f1fdd6459f))
* **contracts:** make both Soroban crates build and test again ([c1ad377](https://github.com/Sundriveauto/Ledgerlens-core/commit/c1ad377f47b4c102df0eb5a2bb6fd1f295352b36))
* distributed per-API-key rate limiting shared by REST and gRPC ([2e1f791](https://github.com/Sundriveauto/Ledgerlens-core/commit/2e1f79106719c4b3f64765a439bb3c09f037c4a5))
* enable testutils feature and fix asset_pair type in fuzz harnesses ([8b98f63](https://github.com/Sundriveauto/Ledgerlens-core/commit/8b98f63416ca9d70e81c732ced317b9d1ea40195))
* **oracle_aggregator:** make contract compile, fix quorum bypass and wire format ([3022933](https://github.com/Sundriveauto/Ledgerlens-core/commit/3022933479cbf8bb998110928b7f59a8b88b03c0))
* **oracle_aggregator:** unblock the fuzz CI job so zk_verifier's targets actually run ([fd64c34](https://github.com/Sundriveauto/Ledgerlens-core/commit/fd64c347ad8d9c53b92c092bb9e15e93940f6a8c))
* **oracle:** require auth on OracleAggregator::initialize (issue [#688](https://github.com/Sundriveauto/Ledgerlens-core/issues/688)) ([05cd9cd](https://github.com/Sundriveauto/Ledgerlens-core/commit/05cd9cd1801c95b90d74df7e04624f35603ede7f))
* **oracle:** require auth on OracleAggregator::initialize (issue [#688](https://github.com/Sundriveauto/Ledgerlens-core/issues/688)) ([3c3f49e](https://github.com/Sundriveauto/Ledgerlens-core/commit/3c3f49e1f8124dd3bb3620c00cb648e986b38fda))
* pin ed25519-dalek/rand/rand_core in contract manifests for fuzz build ([dcf69dd](https://github.com/Sundriveauto/Ledgerlens-core/commit/dcf69dd4b9d5b5fc882b67867c2adbe2c04da566))
* repair CI-breaking compile errors and corrupted scaffold files ([cba4033](https://github.com/Sundriveauto/Ledgerlens-core/commit/cba4033054758eabc5c1385bf6b6fa16a7d61967))
* resolve repo-wide ruff lint errors, regenerate OpenAPI schema, fix fuzz Cargo.toml ([b99100d](https://github.com/Sundriveauto/Ledgerlens-core/commit/b99100d70a44530f9396319131c41b694047f13a))
* wire quorum scores to registry ([#684](https://github.com/Sundriveauto/Ledgerlens-core/issues/684)) ([6030f39](https://github.com/Sundriveauto/Ledgerlens-core/commit/6030f39306cfce32693b14970d9d04f768ba7563))
* **zk_verifier:** make contract compile and actually verify proofs ([390ff46](https://github.com/Sundriveauto/Ledgerlens-core/commit/390ff46fcebaf2379dc3c907b9df987faf4cd51f))
* **zk_verifier:** make contract compile and actually verify proofs ([bbc4958](https://github.com/Sundriveauto/Ledgerlens-core/commit/bbc4958a44e622837e70a10388606ce6b52e42c8))


### Documentation

* document Docker build steps, panic messages, and add CHANGELOGs ([#791](https://github.com/Sundriveauto/Ledgerlens-core/issues/791), [#792](https://github.com/Sundriveauto/Ledgerlens-core/issues/792), [#793](https://github.com/Sundriveauto/Ledgerlens-core/issues/793), [#794](https://github.com/Sundriveauto/Ledgerlens-core/issues/794)) ([3325df4](https://github.com/Sundriveauto/Ledgerlens-core/commit/3325df4c536bb183e36b8881d522b73277915d07))
* document Docker build steps, panic messages, and add CHANGELOGs… ([c229d88](https://github.com/Sundriveauto/Ledgerlens-core/commit/c229d882a2848eef62b5201b43170491a5f0179e))


### CI

* build and test both Soroban contract crates on every push and PR ([a481cbf](https://github.com/Sundriveauto/Ledgerlens-core/commit/a481cbf5afc3a187dfc85ae70288acec25716f6a))

## [Unreleased]

### Fixed
- Unblocked the fuzz CI job so zk_verifier's fuzz targets actually run.
- Made the contract compile; fixed quorum bypass and wire format issues.
- Enabled testutils feature and fixed asset_pair type in fuzz harnesses.
- Pinned ed25519-dalek/rand/rand_core versions in contract manifests for fuzz build.
- Resolved repo-wide lint errors and regenerated OpenAPI schema.

### Added
- Built a fuzzing and symbolic-execution harness for the Soroban contract.
- Implemented multi-signature oracle quorum for tamper-resistant on-chain score publication.
- Initial contract scaffold for oracle network feature.
