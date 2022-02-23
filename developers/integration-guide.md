# Integration Guide

## Hooking up your contract to a Candybox project

This guide is for users who would like to hook up their contract to a pre-existing Candybox project. Right now, the primary use case for this is to route funds to a Candybox project when certain events occur (e.g., minting an ERC721 token).

Add the Candybox contract dependency to your project:

```
$ yarn add @candyboxdao/contracts-v1
```

Inherit from `CandyboxProject` in your contract. You will need to provide a `Project ID` and [`Terminal Directory`](../protocol-v1/terminal-directory.md) address to the `CandyboxProject` constructor.

```
// SPDX-License-Identifier: MIT
pragma solidity 0.8.6;

import "@candyboxdao/contracts-v1/contracts/abstract/CandyboxProject.sol";

contract HelloWorldContract is CandyboxProject {
  ...

  constructor(
      uint256 _projectID,
      ITerminalDirectory _terminalDirectory
    ) CandyboxProject(_projectID, _terminalDirectory) {}

  ...
}
```