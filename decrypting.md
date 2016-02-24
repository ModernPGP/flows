Decrypting Flows
================

These flows exist in respect to situations that arise while successfully or unsuccessfully **decrypting** data whereby a user does or does not contain private key.

## Can't Decrypt

When the case arises that PGP encrypted data CANNOT be decrypted by a user, the reasons being usually one of the following

#### Missing Key

This is perhaps the most common case user encounter, and the status message of **missingkey** is misleading, as what it means is the the receiver is "missing" one of the "keys" to which the data was encrypted. The most common real world scenario of this happening is that the sender used a key owned by the recipient that is either expired, revoked, or has lost the private key.

* Analyze the UID's of all the keys which data was encrypted to
* Compare UID's if any of these values match receivers current key
* * If yes, explain this to receiver
* Provide an easy method for receiver to send current key to sender

![Image of Mailpile missing key UX](images/missing-key-mailpile.png)

* Visual missing key UX in [Mailpile](https://mailpile.is8)*

