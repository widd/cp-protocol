# Club Penguin Protocol
---
### Info
This is a project dedicated to reverse engineering the network protocol of the popular (but now defunct) online game __Club Penguin__.
It attempts to document all of the relevant network messages in their entirety as well as the general control flow of the game server(s).

This documentation is separated into __two__ distinct branches/versions:
__AS2__ and __AS3__ - the names represent the original protocol and when the protocol underwent major changes between 2008 and 2012, respectively.

### Structure
The Club Penguin network protocol revolves around a string-based packet format. The server sends extra precursory information with each packet while the client sends (generally) shorter messages in response. The login scheme also makes use of XML for a few initial checks, but the vast majority of network operations use this format (the __game server format__, or __SmartFoxServer format__).

### Glossary
TODO: Write a glossary table that includes a client and server packet/message reference.