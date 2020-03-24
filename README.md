# Stem: A distributed infrastructure

*read in other language: [简体中文](zh/README.md)*

## Table of Contents

- [Overview](#Overview)
- [Project Design](#project-design)
  - [Paper and Documents](#paper-and-documents)
- [State of project](#state-of-project)
  - [Implementation](#Implementation)
- [License](#License)

## Overview

![](img/stem.png)

## Project Design

To learn more design detail for this project, please read [Paper and Documents](#Paper and Documents). 

### Paper and Documents

- [Whitepaper](en/whitepaper.md): Describe `Stem`'s aims and design principle.
- [RFCs](en/rfcs/index.md): Describe the detail of project.

## State of project

***Yinet is a work in process!***

### Implementation

- Rust
  - [addr-hal](#) Hal for abstract for address in `no_std`.
  - [net-hal](#): Hal for network in `no_std`.
  - [manager-hal](#): Hal for network device manager in `no_std`.
  - [lwip-net](#): Hal implementation for `net-hal`
  - [udp-reuse](#): Reusable udp package.
  - [discovery](#): distributed network discovery using DHT.
  - [tunnel](#): Nat travelling.
  - [keymanager](#): Key management for Node.
  - [kv-hal](#): Hal for kv storage.

We persent project's roadmap here.

## License

MIT