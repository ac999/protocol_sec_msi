# Security Protocols: Modelling and verification 2021 (teached by Lecturer, Ph.D. Cătălin Bîrjoveanu)
## Done during Master's in Information Security @ Faculty of Computer Science within Alexandru Ioan Cuza University of Iasi

Let be the following protocol:
A → B : { Na,A , B }Kb
B → A : {h(Kab, Na, B), Nb, Kab }Ka
A → B : {h(Nb, Na) }Kb
where, Na/Nb-nonce of A/B; Ka/Kb -public key of A/B; Kab -session key; h -hash function.

The protocol’s goals are secrecy of Kab and mutual authentication.
1. Model the protocol in Scyther including secrecy and non-injective synchronization properties.For session keys,introduce a user-defined type in Scyther. Verify the security properties using Scyther. Explain the results obtained. 
2. Find six improvements of the protocol in terms of message size or complexity and motivate each improvement. Test each suggested improvement using Scyther. If any of improvement fails, explain why.

2. a.  Moving the hash function outside of the encrypted message b/c hashing is irreversible
2. b. Removing the receiver's identity in the first step
