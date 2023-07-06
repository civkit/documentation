The CivKit Node is an experimental Nostr relay, complemented by the ongoing development of communications
gateways for [BOLT8](https://github.com/lightning/bolts/blob/master/08-transport.md) Noise transport and
[BOLT4](https://github.com/lightning/bolts/blob/master/04-onion-routing.md) sphinx onion routing, thus
enabling Nostr services to be accessed over the Lightning network.

The main service supported by the CivKit node is a market board, where multiple connected nodes can
form a peer-to-peer market system. 

```

		    `civkit-cli`
			|
			|			
	- - - - - - - - | - - - - - - - - - - - - - - - - - - - - - - - - - - - 
		        |					`civkitd`
			|
			|	   ----------------------  credentials
		        |	   | CredentialsHandler |<----
		        |	   ----------------------    |	   -----------------        
			V			     	     |---->| ClientHandler |-------- "NostrClients" (`civkit-sample`)
		------------------	   events	     |	   -----------------
		| ServiceManager |<--------------------------|
		------------------			     |---->---------------
	           /		\       -----------------          | PeerHandler |\
		 /		 \	| GossipHandler |--------->---------------  \
	       /		  \	-----------------			      \
	      V		           V							"NoisePeers"
	----------------------	 ------------------					
	| AttestationManager |   | StorePersister |
	----------------------	 ------------------

```

The CivKit Node is relaying on few building blocks.

## BOLT12 Offers

[BOLT12](https://bolt12.org/) is a next-generation payment protocol simplifying the process of requesting
and making Lightning Network payments. For the CivKit, offers allows selective revealment of fields for trade
intermediation and extensible format to add new custom information for each type of trades, among other advantages.

## Onion Messaging

[Onion messaging](https://github.com/lightning/bolts/pull/759) is an onion-routing network already builted in the
Lightning Network, initially used to carry on HTLC payments. For the CivKit, onion messaging can be used to
transport offers in a privacy-preserving fashion, while benefiting from the anonymous set constitutes by the Lightning
network nodes.

## Nostr Relay/Client

[Nostr](https://github.com/nostr-protocol/nips) is a communication protocol to transport data notes between
relays and clients, with the fundamental feature of moving the key-management and state on the client-side
compared to traditional communication protocol like HTTP. For the CivKit, Nostr architecture enables clients
to switch from a market board to another with low-migration cost, and thus react to market dynamics.

## Mainstay

[Mainstay](https://commerceblock.readthedocs.io/en/latest/mainstay/) is a notarization protocol based on
the Bitcoin blockchain, where the attestation issuer can have their data payload stamped into the chain, with
a unique history of attestion (i.e a `proof-of-immutable-state`). For the CivKit, notarization of offers enable
to verify the board offers history and therefore its quality as a board in a trust-minimized fashion. Compared
to other notarization protocol, market boards cannot equivocate on their history, and selectively reveal
advantageous offers.

## Staking Credentials

[Staking Credentials](https://github.com/civkit/staking-credentials-spec) are anti-DoS tokens enabling a
server to protect its ressources by requesting the client a pre-payment in an exchange of a privacy-preserving
credentials. For the CivKit, this enables the market board to manage their publication space ressources in a
fashion aligned with the clients incentives.

CivKit aims to offer good interfaces for clients softwares, where they can access market board
services over standard Nostr or Lightning communication channels.

Authored July 2023.

Expected Q4 2023.
