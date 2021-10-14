---
description: Stores ETH for terminals.
---

# JBETHVault

## Constructor

```solidity
constructor(IJBDirectory _directory) {
  directory = _directory;
}
```

* Arguments:
  * `_directory` is an [`IJBDirectory`](../interfaces/ijbdirectory.md) contract storing directories of terminals and controllers for each project.