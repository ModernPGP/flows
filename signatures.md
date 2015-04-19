Signature Flows
===============

## Can't Verify

There are various states of signatures whereby a user is presented with something less than ideal that appears to be scary. A good interface SHOULD present the user with each to follow actions to remedy these situations or at least clearly.

#### Unknown Signature

This case is relatively common and whereby a message was received with a PGP signature, but the receiver does not have the PGP public key that signed the message.

* Attempt to autodiscover key from servers
* Provide user action to manually go discover key
* Provide option to manually import key


PGP Keys Flows
==============

## Discovery

The discovery & search aspect of finding the public which a user is hoping to communicate with is a major pain point. Since keyservers are usually write/update only, often times expired, revoked or otherwise unsuable keys show up. Learning how to decipher which key is the best key (for a contact you are hoping engage with) is a dark art, and oftentimes nigh impossible.

#### Humanizing Search

* Name & email addresses are given priority in UI
* Avatars are preferable
* Hiding technical "key specific" details
* Provide clear "rating" score of keys


## Importing

The action of importing a key to a users keychain is often a major pain point with PGP. Most standalone PGP applications offer some sort of "Import" functionality. However, oftentime this stands on top of other components & tools such as the OS's filesystem and copying & pasting to a clipboard.


#### Inline PGP Keys

Due to the maleable nature of email messages as well as various PGP compontents (keys, attachments, etc...) there are many different occurances that diffing PGP implementations do in an attempt to improve things.

* Extract key data between `BEGIN PGP PUBLIC KEY BLOCK` and `END PGP PUBLIC KEY BLOCK`
* Replace with an actionable button to import key
* * If key is in keychain, explain this to user
* * If key is in keychain, offer other helpful 'actions' like inspect or forward key

#### Attached PGP Keys

* Offer simple import button that imports the key
* Differentiate this from other attachments