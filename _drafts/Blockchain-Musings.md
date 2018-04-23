It provides:

- Anonymity: transactions can't be linked to your real identity (unless you want them to be)
- Provability: each transaction comes with a mathematical proof that both parties agreed to it
- Immutability: the entire history of the blockchain is set in stone and can be audited
- Fault tolerance: the network's performance is not impacted by the failure of any single node
- DDOS resistant: as a corollary to fault-tolerance, it is not possible to take down the network with a denial of service attack
- Censorship resistant: it is not possible to prevent participants from submitting transactions

But if we dig into the components and attributes of blockchain, it becomes apparent that it's not without some very real drawbacks:

 - Low throughput: block times are around 10 minutes, and most merchants will wait at least six blocks to be sure a transaction has been committed to the chain.
 - High (and volatile) transaction costs: fees spiked to over $30 earlier in the year, and now sit around $0.60.
 - Wasted energy: Bitcoin mining consumes more power than the Republic of Ireland
 - Difficult to upgrade: there are 3 different Bitcoin forks
 - Large file sizes: the Bitcoin blockchain is 150Gb and counting

None of this is news to anybody, and
## The Blockchain Stack
When most people talk about "the blockchain," they're specifically referring to the public Bitcoin blockchain. This is really a combination of three core technologies: assymetric cryptography, Merkle trees, and proof of work. Each of these brings its own advantages and disadvantages.

#### Assymetric Cryptography
Public key cryptography has been around since the 1970s, and most of the modern internet depends on it.

__Pros__:
- Transactions can be anonymous
- Transactions can be mathematically proved

__Cons__:
- Not many

#### Merkle Trees
These have also been around since the late 1970s. They are a data structure that, among other things, lets us be certain that the blockchain hasn't been tampered with.

__Pros__:
- Immutable
- Auditable

__Cons__:
- Large file sizes (the Bitcoin blockchain is 150Gb and counting)

#### Proof of Work
This is what people mean when they talk about "mining," and it's the truly novel component of blockchain. It lets a decentralized network agree on the state of the blockchain.

__Pros__:
- Enables distributed consensus, which gives us:
    - Fault tolerance
    - DDOS resistance
    - Censorship resistance

__Cons__:
- Low throughput
- High transaction costs
- Wasted CPU cycles/energy
- Difficult to upgrade/potential to fork

#### Permissioned Blockchains
One obvious reaction to the many faults of proof of work is to do away with the decentralized network. It is possible to preserve many, but not all of the desirable attributes of blockchain while only allowing privileged nodes to add new blocks.

__Pros__:
- No need for proof of work, enabling:
    - High throughput
    - No wasted energy
- The system is still:
    - Anonymous
    - Auditable
    - Provable

__Cons__:
- Censorship: privileged actors can blacklist participants
- Transaction order can be manipulated
- Less DDOS resistant

## Proof of Work and Consensus
From the above, it's clear that many of blockchain's most glaring flaws come from proof of work. It's worth taking a brief digression to further understand what this is and why it's needed.

It is common to hear people claim that miners are "verifying" transactions. This is not true: every node in the network verifies transactions. Miners are competing to solve an arbitrary math problem that has only one purpose: to slow down the network. This turns out to be absolutely necessary for public blockchains to function. Slowness is a feature, not a bug.

To see why, think about what happens when a new block is added to the blockchain. Every miner in the world competes to solve this useless math problem and the one who solves it first gets to add the next block, rewarding themselves with a fixed amount of cryptocurrency in the process. But what happens when two people both solve the problem at the same time?

In this case, the blockchain forks. This would be a problem: if some people follow one fork, and some the other, then you end up with two groups of people who can't agree on the state of the blockchain. To fix this, participants vote with their feet. Immediately after a fork, a more-or-less random subset of miners will start working on each fork. After the next block, they will all look around to see if there is a longer chain out there. If there is, they switch to that one. The idea is that if more miners and more processing power are devoted to one fork, that one will grow faster than the others. The other forks get "pruned," and all the energy spent mining on them was wasted.

But what would happen if, after a branch takes place, each of those branches immediately branched again? The blockchain would quickly become a block-tree, and participants would disagree about the "true" state of the tree based on which branch they were on. To prevent this, the blockchain uses proof of work to enforce slowness. As long as the time it takes to add a new block is much longer than the time it takes for all participants to find out about the state of the network, we are able to prove that the network will always converge to a single longest chain given sufficient time.

These problems with proof of work are broadly acknowledged in the community, and alternative consensus algorithms are one of the most active areas of research.
