# Project

#### What everyone needs to know

* Each project within the Candybox protocol is represented as an ERC-721 NFT.
* Whoever is the owner of a project's NFT has access to [admin functionality](./operator.md#operatable-functionality) for that project within the protocol, which ultimately gives it control over the project's funds.

#### What you'll want to know if you're building

* Projects can be created either within the context of Candybox with a call to [`JBController.launchProjectFor(...)`](../../specifications/contracts/or-controllers/jbcontroller/write/launchprojectfor.md) which also configures its funding cycle properties and sets it up to receive payments, or by itself with a call to [`JBProjects.createFor(...)`](../../specifications/contracts/jbprojects/write/createfor.md). The `launchProjectFor` transaction calls `createFor` as part of its routine.
* A project can accomodate arbitrary metadata for any number of domains that can be updated by the project owner at any time using the [`JBProject.setMetadataOf(...)`](../../specifications/contracts/jbprojects/write/setmetadataof.md) transaction. This can be used by clients to store a reference to metadata stored on IPFS, or whatever. The protocol does not define standards for this metadata. A project's current metadata for any particular domain can be found by reading from [`JBProject.metadataContentOf(...)`](../../specifications/contracts/jbprojects/properties/metadatacontentof.md).
* Look through the [`JBProjects`](../../specifications/contracts/jbprojects/) contract for a complete list of relevant read functions, write functions, and emitted events.
