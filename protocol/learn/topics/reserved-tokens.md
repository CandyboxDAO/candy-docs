# Reserved tokens

#### What everyone needs to know

* Reserved tokens allow a project to guarantee that a percentage of all newly minted tokens from payments will be reserved to a list of preprogrammed [`JBSplit`](../../specifications/data-structures/jbsplit.md)s. This percentage is referred to as the reserved rate.
* A project's reserved rate and reserved token splits can be reconfigured each funding cycle.
* Reserved token splits can be routed to addresses, the owners of other Candybox projects, or to contracts that adhered to the [`IJBSplitAllocator`](../../specifications/interfaces/ijbsplitallocator.md) interface.
* Reserved tokens do not get minted automatically when a new payment is received, they instead must be explicitly distributed during the funding cycle which contains the reserved rate and splits that should be applied. If a funding cycle's reserved rate or splits change before the allocation is distributed, the new values will apply.

#### What you'll want to know if you're building

* A reserved rate can be specified in a funding cycle through the [`JBController.launchProjectFor(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/launchprojectfor.md) or [`JBController.reconfigureFundingCyclesOf(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/reconfigurefundingcyclesof.md) transactions.
* Distributing currently allocated reserved tokens is done by calling [`JBController.distributeReservedTokensOf(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/distributereservedtokensof.md). Doing so will distribute the allocation according to the current funding cycle's reserved rate.
