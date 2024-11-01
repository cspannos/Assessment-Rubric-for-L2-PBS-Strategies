# WIP: Assessment Rubric for L2 PBS Strategies

This rubric provides a comprehensive framework for assessing the effectiveness, fairness, and security of PBS strategies in Layer 2 blockchains. Each category and criterion can be tailored further to align with the specific goals and architecture of your Layer 2 protocol.

| Category                         | Criteria                              | Description                                                                                                                     | Scoring Guidelines                                                                                                                |
|----------------------------------|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| Sequencers                       | Centralized                           | Sequencers are centralized, leading to potential risks in terms of control and single points of failure.                        | Low score for centralization due to risks; high score for decentralization.                                                       |
| Sequencers                       | Shared                                | Sequencers are shared among multiple entities, providing a balance between centralization and decentralization.                 | Moderate score for shared sequencers, depending on the level of decentralization achieved.                                        |
| Sequencers                       | Decentralized                         | Fully decentralized sequencers, minimizing risks associated with central control.                                               | High score for fully decentralized sequencers, as it supports network security and resilience.                                    |
| Proposers                        | Single                                | A single proposer is responsible for block proposals, which could centralize power.                                             | Low score for single proposers due to centralization concerns.                                                                    |
| Proposers                        | Round-Robin                           | Proposers are selected in a round-robin manner, distributing power more evenly among participants.                              | Moderate score for round-robin, as it helps distribute power but may still have limitations.                                      |
| Proposers                        | Random Selection                      | Proposers are selected randomly, reducing predictability and centralization.                                                     | High score for random selection, as it reduces centralization and enhances fairness.                                              |
| Proposers                        | Delegated                             | Proposers are delegated by token holders, introducing potential governance risks.                                                | Score depends on how delegation is implemented and whether it avoids concentration of power.                                      |
| Builders                         | Single                                | A single builder is responsible for constructing blocks, which may lead to centralization.                                      | Low score for single builders due to centralization concerns.                                                                     |
| Builders                         | Multiple                              | Multiple builders are involved in block construction, promoting competition and decentralization.                               | Higher score for multiple builders, as it promotes a healthy competitive environment.                                             |
| Builders                         | Distributed Block Building            | Block building is distributed among many entities, minimizing risks of centralization.                                          | High score for distributed block building, as it supports decentralization and fairness.                                          |
| Inclusion Lists                  | Static                                | Inclusion lists are static, which could limit flexibility in transaction selection.                                              | Low score for static inclusion lists, unless they provide significant benefits for security or fairness.                          |
| Inclusion Lists                  | Dynamic                               | Inclusion lists are dynamic, allowing for more flexibility and adaptability in transaction selection.                           | High score for dynamic inclusion lists, as they enhance adaptability and efficiency.                                              |
| Slashing Conditions              | WIP                                   | Evaluate the conditions under which proposers or builders may be penalized (slashed) to ensure alignment with network incentives. | Score depends on how slashing conditions align incentives and deter malicious behavior.                                           |
| Proving                          | Proving Market                        | Proving is handled by a market-driven approach, potentially encouraging innovation but also introducing competition risks.      | Score based on how the proving market affects decentralization and security.                                                      |
| Proving                          | Multi-Prover Setup                    | Multiple provers are involved, enhancing security but possibly at the cost of increased complexity and coordination.            | Higher score for multi-prover setups that enhance security while maintaining efficiency.                                          |
| Proving                          | TEEs (Trusted Execution Environments) | Provers use TEEs, which could offer strong security guarantees but might raise concerns about centralization or vendor control. | Score based on the trade-offs between security, centralization, and openness.                                                     |
| On-Chain vs. Off-Chain Solutions | On-Chain                              | The PBS implementation relies on on-chain mechanisms, which offer greater transparency and decentralization.                    | High score for on-chain solutions, as they enhance transparency, security, and decentralization.                                  |
| On-Chain vs. Off-Chain Solutions | Off-Chain                             | The PBS implementation uses off-chain solutions, which might improve performance but introduce centralization risks.            | Lower score for off-chain solutions, unless strong decentralization and security measures are in place.                           |
| Auctions                         | Block                                  | Auctions are held for each block, allowing builders to bid for inclusion.                                                       | Score depends on transparency and fairness of the auction process.                                                                |
| Auctions                         | Timing Games                          | Auctions may involve timing games, potentially leading to inefficiencies.                                                        | Lower score if timing games introduce inefficiencies or unfair advantages.                                                        |
| Auctions                         | Bidding                               | WIP                                                                                                                             |                                                                                                                                   |
| Auctions                         | Just-In-Time                          | WIP                                                                                                                             |                                                                                                                                   |
| Auctions                         | Ahead-Of-Time                         | Execution Tickets (Execution Auctions)                                                                                          |                                                                                                                                   |

### Grant Acknowledgment
This work is made possible by a grant from the PBS Foundation and support from Blockdaemon.

This rubric aims to help Layer 2 developers and the broader blockchain community enhance fairness, efficiency, and decentralization in PBS approaches, particularly in relation to equitable MEV distribution.

### Usage
You can use this rubric as a reference to evaluate the PBS strategies within your Layer 2 blockchain protocol. It helps identify strengths and areas for improvement to ensure a balanced approach to decentralization and efficiency.

### Contributing
We welcome contributions to improve this rubric. Please feel free to submit your suggestions via a pull request or open an issue to discuss improvements.

### License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
