## Flashbots

* Flashbots is a research and development organization focused on mitigating the negative externalities of current MEV extraction techniques and avoiding the existential risks MEV could cause to state-rich blockchains like Ethereum.

* Flashbots try to move the problem to another area to prevent clogging up the Ethereum network and giving it more clarity. I works by reducing MEV's complexity by three fronts:
    - tools to inspect and quantize the impact of MEV. This helps reduce the information asymmetry and people can understand the problem and its impact better. (MEV-Inspect).
    - Democratize the extraction of MEV. The power to extract MEV exists in the hands of few people so they provide tools for everyone to start extracting MEV. (MEV-Geth)
    - Distribute the benefit of MEV. Currently, the miners and validators extract a disproportionate amount of benefits. So it’s important to redistribute these to all the participants.


### The auction architecture relies on 3 parties:

- searcher: bots looking for access to blockspace, users frontrunning protection on their transactions, and dappas with advanced use cases
- relay
- miner


## `mev-inspect-py`

Tool to inspect maximal extractable value for Ethereum: [mev-inspect-py](https://github.com/flashbots/mev-inspect-py).
If shows: miner payments, tokens transfers and profit, swaps and arbritages.

#### Pre-requisites: 

- [k8s's kind](https://kind.sigs.k8s.io/docs/user/quick-start/)
- docker
- [helm](https://helm.sh/docs/intro/install/)
- an `RPC_URL`

## MEV-geth

* Software which can be run by miners to mitgate negative externalities of MEV.
