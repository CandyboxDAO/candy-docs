# Splits

#### What everyone needs to know

* A project can store splits for an arbitrary number of groups, such as for payout distributions or for reserved token distributions.
* A split can specify an address, a candybox project, or a contract that adheres to the [`IJBSplitAllocator`](../../specifications/interfaces/ijbsplitallocator.md) interface as its recipient.
* By default, splits can be changed at any time for any funding cycle configuration. A project's owner can also independently lock a split to a funding cycle configuration for a customizable duration.

#### What you'll want to know if you're building

* Splits can be set for a funding cycle configuration during the [`JBController.launchProjectFor(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/launchprojectfor.md) or [`JBController.reconfigureFundingCyclesOf(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/reconfigurefundingcyclesof.md) transactions, or separately using [`JBSplitStore.set(...)`](../../specifications/contracts/jbsplitsstore/write/set.md).
