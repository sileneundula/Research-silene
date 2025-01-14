# Onion Router Extension (Ring Signatures, Verifiable Random Functions, Identical Nodes)

## Introduction

The Onion Router, while powerful, comes with inherent problems to the gateway node and exit node. The Exit Node is where the final hop takes place to deliver the encrypted payload to the destination. It is a common place for attacks to occur.

## Proposed System (Tor Ring Signatures and VRF)

The proposed method to enhance security is to let all nodes be identical rather than distinguishing between exit nodes and gateway nodes. Instead, the traffic should be routed through a group of users wihout prioir knowledge of who is the exit node and gateway node. This prevents the nodes from knowing who they are in the relay.

Using a public key, a Verifiable Random Function can be derived from the public key to choose who becomes which node.
