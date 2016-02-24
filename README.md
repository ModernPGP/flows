UX Flows
========

- [Encryption Flows](encryption.md)
- [Decryption Flows](decryption.md)
- [Signature Flows](signatures.md)


**The following is dump of working session held at the OpenPGP Summit, April 19, 2015**


UX Flows 
Framework / schema of documenting ux that is friendly to design & devs


Working Scenarios:
- key generation
- this is a rare thing we do
- BUT this is the FIRST contact the user may have with pgp, 
- the aim of key generation is to become invisible 
- BUT at this moment we create an essential ASSET of the user (his private key)

come on agreed upon tasks the user need to perform when using our tools
(and not create a wizard)
"I want to send a message"
"I want to receive a secured message" ...


github commits to modernpgp 

Pain Points:
- key generation
- 
- key discovery
- a keyserver doesn't answer
- key synchronization
- sending message
- can't encrypt
- because doesn't have the key of one recipient

- receive message
- can't decrypt
- because doens't have private key ...




food for thoughts

a user "can" know
but he doesn't "need" to know
 (what a private key, a fingerprint, a revocation certificate... are)

wizards are really sketchy idea
"we hurt the user into doing something the developer wants him to do"

"stop annoying the user" 
> here a number of small things that will annoy the user at the ux level if we don't consider them

document our apps to obtain number on errors 
> usability statistics collection (possible in the opensource world) 

