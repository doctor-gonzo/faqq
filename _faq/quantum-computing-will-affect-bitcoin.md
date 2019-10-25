---
title: "It's going to affect Bitcoin"
category: 'statement'
---

## And this is a problem that needs to be addressed sooner rather than later

- A powerful quantum computer can reverse Bitcoin public keys into private keys in a matter of minutes[^QUANTUMATTACK]
- 36% of all BTC are on addresses with exposed public keys[^EXPOSEDKEYS]
- 100% of addresses can be hacked during transactions - and every address would have to submit a transaction in order to transition their BTC to a new quantum-proof address format[^QUANTUMTX]

[^QUANTUMATTACK]: A powerful quantum computer can reverse Bitcoin public keys into private keys in a matter of minutes

	**Reversing Bitcoin keys:**

	If someone knows your public key, they can also calculate your private key with a sufficiently powerful quantum computer — which is unthinkable using even today’s most powerful classical computers. In the era of quantum computers, the public-private ECDSA keypair will be the weak link. Quantum computers have the potential to perform specific kinds of calculations significantly faster than any classical computer. Additionally, quantum computers will be able to run algorithms that take fewer steps to produce an output, leveraging quantum phenomena like entanglement and superposition. 

	Most blockchains use Elliptic Curve Digital Signature Algorithm (ECDSA) for address security. Using a sufficiently powerful quantum computer, [Shor's algorithm](https://arxiv.org/abs/quant-ph/0301141) can be used to break ECDSA.  Specifically: an attacker will be able to an associated private key from a given public key. So any QC-armed adversary who knows your public key will be able to derive your private key and create a transaction which empties your wallet.
	
	The paper [Quantum Attacks on Bitcoin and how to protect against them](https://arxiv.org/pdf/1710.10377.pdf) states that "by our most optimistic estimates, as early as 2027 a quantum computer  could  exist  that  can  break  the  elliptic  curve  signature  scheme  in  less  than  10 minutes, the block time used in Bitcoin."

[^EXPOSEDKEYS]: Exposed public keys

	"So together (as of 2018 June 4): 19% addresses (4,242,958 of 22,275,753) that hold 36% bitcoins (6,080,090 of 17,072,361) reveal their public keys." - [How many bitcoins are vulnerable to a hypothetical quantum attack](https://medium.com/@sashagnip/how-many-bitcoins-are-vulnerable-to-a-hypothetical-quantum-attack-3e59e4172e8)


[^QUANTUMTX]: 100% of the addresses can be hacked during transactions:

	"After a transaction has been broadcast to the network, but before it  is  placed  on  the  blockchain,  it  is  at  risk  from  a  quantum  attack. If the secret key can be derived from the broadcast public key before the transaction is placed on the blockchain, then an attacker could use this secret key to broadcast a new transaction from the same address to his own address. If the attacker then ensures that this new transaction is placed on the blockchain first, then he can effectively steal all the bitcoin behind the original address." - [Quantum attacks on Bitcoin, and how to protect against them](https://arxiv.org/pdf/1710.10377.pdf)
