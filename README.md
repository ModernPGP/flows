Flows
=====

These UX flows exist to help applications implement a more standardized and better user experience of interacting with PGP and the numerous situations that arise.

## Can't Encrypt

There is the case where a user is trying to encrypt data and is unable to due to not having keys for all the intended receipients. In the case of being unable to encrypt, a tool SHOULD help the user figure out why this is and what can be done in order to encrypt.

* Offer UI feedback (colors & icons) that hint at why encrypting is not possible
* Explain the problem via clear and short status message
* Offer easy to perform actions to remove blocks
* Offer UI feedback that signals once encryption is possible


## Can't Decrypt

When the case arises that PGP encrypted data CANNOT be decrypted by a user, the reasons being usually one of the following

#### Missing Key

This is perhaps the most common case user encounter, and the status message of **missingkey** is misleading, as what it means is the the receiver is "missing" one of the "keys" to which the data was encrypted. The most common real world scenario of this happening is that the sender used a key owned by the recipient that is either expired, revoked, or has lost the private key.

* Analyze the UID's of all the keys which data was encrypted to
* Compare UID's if any of these values match receivers current key
	* If yes, explain this to receiver
* Provide an easy method for receiver to send current key to sender

