This is a collection of terms that are used frequently on the XMPP network as well as in the articles in xmpp.how.

- XMPP: E**x**tensible **M**essaging and **P**resence **P**rotocol. The chat protocol that allows for decentralized communication. It uses **XML** across the network.
- Jabber: Historical term for XMPP. XMPP and Jabber are interchangeable terms.
- MUC: Multi-User Chat. A single chatroom that can hold multiple users. These rooms have multiple permission structures of Moderators, Administrators and Owners.
- Group Chat. a MUC that is members only. Mainly used by certain clients. Comes from [https://docs.modernxmpp.org/client/groupchat/](https://docs.modernxmpp.org/client/groupchat/)  
- Channel. a MUC that is public. Mainly used by certain clients. Comes from [https://docs.modernxmpp.org/client/groupchat/](https://docs.modernxmpp.org/client/groupchat/)
- Room: Interchangeable term for MUC.
- Conference: Interchangeable term for MUC.
- Server: where your account lives. Your server communicates with itself as well as other servers in order to send messages.
- Instance: Interchangeable term for server.
- Client: An application which communicates with an XMPP server and provides a user interface for chatting with others.
- Application/program: Interchangeable term for client.
- OMEMO: End to end encryption protocol used by the majority of the network.
- OTR Encryption: Historical end to end encryption protocol. Largely replaced by OMEMO.
- MAM: Message Archive Management. Refers to the ability to read messages sent in the past by other users. These messages are stored on the server the MUC is being hosted on and is usually deleted after a set period of time.
- Moderated MUC: A MUC that automatically makes new members Visitors and requires a Moderator to make them a Participant. In Moderated MUCs, moderators can make users Visitors in order to mute them.
- Moderated message: not to be confused with the term above. When a message is moderated, it has been altered or deleted by a moderator. Some legacy clients such as Psi+ do not have support for moderations.
- Corrected message: When a message has been corrected, it has been altered by the user who sent it.
- Edited message: Interchangeable term for corrected message.
- Retracted message: When a message has been retracted, the user has deleted its contents.
- Deleted message: Interchangeable but incorrect term for retracted message. Retracted messages are not deleted.
- Voice: Historical term which simply means that a user is not muted. A user that does not have voice is muted and cannot talk and vice versa.
- Ban: Self-explanatory.
- Kick: To forcefully disconnect a user from a room. A kicked user can rejoin as long as they have not been banned.
- ![[outcast.png]]Outcast: A banned user.
- ![[noaffiliation.png]]Visitor: A user that can read messages but cannot reply, chat or react to any messages. In most MUCs, visitors can still private message users.
- ![[noaffiliation.png]]Participant: A user that can read messages, reply, chat, react and private message users in the MUC. They cannot moderate messages, configure the room or kick and ban users.
- ![[member.png]]Member(ship): A user that has been granted membership. In most cases there are little to no differences between a member and a normal participant. In rooms that have CAPTCHAs, members do not have to fill out the CAPTCHA when they join. All members are participants but not all participants are members.
- ![[admin.png]]Moderator. A user that can do everything Members can do as well as moderate messages, ban users and perform other tasks. They can see the JIDs of people in semi-anonymous rooms.
- ![[admin.png]]Administrator: Functionally identical to a moderator.
- ![[owner.png]]Owner: A user that can do everything administrators can do as well as configure and Destroy the room. This is technically a misnomer, as there can be multiple Owners in a MUC.
- JID:  Shorthand for Jabber ID. An identifier for users, MUCs, server nodes and servers on the network. They are identical to e-mail addresses, where the first part is the username and the second part is the domain:
  `user@server.org`
  JIDs of other cannot be viewed by ![[noaffiliation.png]]non-moderators in semi-anonymous rooms.
- Semi-anonymous. A room where people who are ![[noaffiliation.png]]non-moderators cannot see the JIDs of their peers. Nearly all public rooms are semi-anonymous.
- Private message: Not to be confused with direct message. Also known as whispering in some clients. This is when you can message someone in a MUC independent of whether you have them added as a Contact or not. Certain MUCs disable private messaging. If you are set as ![[noaffiliation.png]]visitor in a MUC, it may be possible to private message others.
- Contact: In virtually all XMPP clients, MUCs and individual users can be added as contacts, allowing you to chat with them. When opening a client after its been disconnected, it will automatically join rooms that are in your contacts.
- Bookmark: Interchangeable term for contact.
- Favorite: Interchangeable term for contact. Favorited rooms in some clients are automatically joined whilst those that are not aren't.
- SIMS: Stateless Inline Media Sharing: A legacy implementation of sharing images. Most clients do not support this.
- Nick(name): What you are known as in a MUC. Nicknames can be changed by the user if the MUC has the permission to do so turned on.
- Service Discovery: A part of the XMPP protocol which allows clients to query the abilities and nodes of clients and servers. Some clients such as Psi+ allow for manual service discovery.
- Disco: Interchangeable (and correct) term for service discovery.
- Avatar: The picture which is associated with a user or room on the network.
- Profile picture (PFP): Interchangeable term for avatar.
- Authorization: In order to begin a 1:1 conversation with a user, they must authorize you first. Authorization can be granted and revoked at any time.
- Ignore: Ignoring a user hides all of their chats and automatically revokes Authorization from them.
- Block: Interchangeable term for ignore.
- Mute: Interchangeable term for ignore.
- Server-to-server communication (S2S): refers to the communication between servers on the XMPP network.
- Federation: Interchangeable and inaccurate term for S2S.
- S2S block: When a server cannot contact another server, usually due to spam or other nefarious activities.
- Defederation: Interchangeable and inaccurate term for an S2S block.
- Topic: In MUCs, topics are a short description of what a MUC entails. Legacy term from the IRC era.
- Bridge: A service that allows you to communicate with other chat platforms and protocols from and to XMPP. For example, bridges that allow you to communicate with Discord or Matrix users.  

Whilst clients may refer to these using different words, we've covered most of the alternative terms used in their place in this document. The XMPP community thinks of new terms in order to replace old ones in order to make the platform more accessible to those who have never used XMPP. Check the [Modern XMPP](https://docs.modernxmpp.org/client/groupchat/) website for more information.