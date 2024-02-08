## ICP

Internet Computer Protocol tokens (ICP tokens) are a native utility token with a value determined on the open market. ICP tokens play a key role in both the governance and the economics of the Internet Computer.

How to get ICP tokens
There are a few different ways you might acquire ICP tokens. For example, you might:

Purchase ICP tokens directly through an exchange that lists ICP tokens available for trade.

Create tokens from rewards (maturity) obtained for participating in the governance of the Internet Computer.

Receive tokens from the protocol as remuneration for being a node provider and operating a Internet Computer node.

Receive a grant of tokens by the DFINITY Foundation.

![icp-tokens-how-to-use-e5d3978a16b2c0cb05834e12a2dad036](https://github.com/Kushite-ICP-HUb-East-Africa/Introduction-to-ckBTC-Token/assets/81568615/77792cc9-5dbe-4e70-9266-8f3f6401608d)


## Cycles
The Internet Computer Protocol runs on a network of nodes owned and operated by a growing community of independent node providers (NPs) distributed across the globe. NPs spend money for running nodes, e.g. they purchase hardware and require electricity and network bandwidth. The Internet Computer Protocol compensates NPs on a monthly basis by minting and distributing rewards in the form of ICP tokens.


To make ICP sustainable, canister smart contracts are required to pay for the resources they consume, e.g. storage and compute. Resource consumption is not paid in ICP tokens but cycles. It’s typically the canister’s developer who charges the canister with cycles. As the canister is used, its cycle balance is continuously reduced. Eventually, the canister needs to be “topped up” with more cycles. The default way to get cycles is to convert ICP tokens to cycles. When doing so, the protocol burns the ICP tokens.

Cycles are measured in very large numbers, such as billions and trillions. When you talk about cycle transfers and replenishment, you will usually operate with trillions of cycles.

Cycles have a fixed price where 1 trillion cycles is equal to 1 XDR, an official group of currencies maintained by IMF. This means that running costs of canisters are decoupled from price fluctuations of ICP.

 Cycles reflect the operational cost of communication, computation, and storage that dapps consume.

Unlike ICP tokens, cycles are only associated with canisters and not with user or developer principals. Because only canisters require cycles to perform operations and pay for the resources they use, users and developers manage the distribution and ownership of cycles through a special type of canister called a cycles wallet. The cycles wallet holds the cycles required to perform operations such as creating new canisters. These operations are executed using the canister principal of the cycles wallet instead of your user principal.

You should keep in mind, however, that calls to the cycles wallet canister are executed using the cycles wallet principal associated with the currently selected user identity. Depending on your currently selected identity and whether the principal associated with that identity has been added as a controller or a custodian for a wallet, you might see different results or be denied access to a specific method.