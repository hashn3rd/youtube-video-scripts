# 01 Helium Hotspot vs Light Hotspot (Lightspot/DIY Packet Forwarder)

- Helium hotspot is currently the only device on the network capable of mining HNT
- Hotspot is currently responsible for all network processes
- Hotspot has a total of 5 features
    1. Issuing Challenges
    2. Transmitting Challenges
    3. Witnessing Challenges
    4. Packet Forwarding/Network Data Transfer
    5. Consensus group
- Features 1, 2 and 3 are part of proof of coverage
- A number of devices are currently approved to work as hotspots on the network
- The network is in the middle of a transition that will see the elimination of the hotspot
- In the new network, Hotspots will be downgraded to Light Hotspots and validators will be added to the network
- After the transition, conensus group activitie will move to the validators, and from then on validators will be in charge of writing new blocks to the blockchain
- Proof of Coverage will be handled by HIP 19 approved Light Hotspots
- Packet forwarding will be handled by approved Light Hotspots as well as DIY Light Hotspots running gateway-rs
- At the end of this transition all existing hotspots will be converted to light hotspots
- Whether these new converted light hotspots will be capable of participating in Proof of Coverage is dependent on manufacturer updates
