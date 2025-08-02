XMPP usages varies wildly depending the client that one is using. However, there are usually similarities in how every single client does things. We do not want this article to be a glorified Gajim tutorial, so we will be using a variety of clients to visualize our points. The name of the client will be shown before the section.

You need a client and a relevant registered account on a server in order to use XMPP. If you do not have those, then please go to the previous articles to begin that process.
[Clients](/clients)
[Servers](/servers)
[Creating an account](/Creating%20an%20account)

***Gajim***
An XMPP client usually presents you with a start screen, showing a number of UI elements:
![[Pasted image 20250801183111.png]]
*(personal information has been blurred for obvious reasons)*

We'll put numbers on each element of the UI and describe them:
![[Pasted image 20250801183526.png]]
1) Allows you to configure your account, including its personal details
2) Where your chats and MUCs are kept. This is called the "roster" or "contact list" in some clients.
3) Allows you to add another profile where you can separate chats. Think of this like folders in Discord. In Gajim, they are known as Workspaces.
4) Allows you to configure the settings of the application itself.
5) Allows you to join a MUC or begin a conversation with a brand new user.
6) Functionally identical to 5.
7) Allows you to send the program to the background or close or minimize it.
8) The help menu of the program, which provides a Wiki, keybinds or other information that makes using the client easier.
## Adding a DM or MUC
***Psi+***
The majority of clients have separate ways to add a user or MUC. If  you decide to add a user, you must know their JID. Once you retrieve this JID, you can then press on the available button for adding a user.
![[Pasted image 20250801184458.png]]
Enter their JID, add an optional nickname (they won't see it on their side) and you can also add their contact to a group if you want to organize your contacts.

Your client should automatically request authorization from the user. Think of this as sending a friend request to a user.

Once the user is added, it may take some time for them to authorize you. In the meantime, you can send them messages, however you won't be able to see the user's status and be aware that some servers and clients block messages from unauthorized users.

In order to join a MUC, you must use your clients respective UI for adding one. A MUC may be referred to as a groupchat, channel or room in your client, however all of these terms are completely interchangeable. [For more information on the terms used on the XMPP network, see the Glossary](/glossary).

You will usually see the option to add a new MUC in the Contacts page, or in a separate menu for generally adding MUCs and users:
***monocles chat***
![[Pasted image 20250801205744.png]]

It is also possible to use a basic room searcher in some clients (pictured here as Discover channels) this feature usually uses a third party room finder service. More on these types of services will be explained in another section.

JIDs of rooms usually look like this:
`roomname@muc.server.org`
`muc` may be `conference` , `group`, `room`, `channel`,  `chat` or any other term which refers to a MUC. There are also MUCs which have JIDs that don't have a MUC subdomain, and simply look like this:
`roomname@server.org`

Always be sure to verify the JID of the MUC you're trying to join.

Once you've hit join on a MUC, you should automatically join it and can now begin chatting freely. There are in fact MUCs where you need to be given voice before chatting. Think of this as just being verified by a moderator.

Here is how being in a room will usually look like:
![[Pasted image 20250801211553.png]]
The experience from here is usually identical to that of a typical chat platform, aside from typical quirks such as:
- Only being able to correct (edit) your latest message
- Unable to view the profiles of others in semi-anonymous rooms if you are not a moderator or above
- Messages moderated by moderators are edited, not deleted
### Chatting with users

***Gajim***
![[Pasted image 20250801185346.png]]
You might be wondering what the green shield is next to the people's usernames. Well, that's OMEMO encryption, which is end-to-end encryption used to secure communications and make sure that they are not intercepted. You can turn on or off OMEMO in most clients like so:
***monocles chat***
![[Pasted image 20250801185634.png]]
OpenPGP is also an alternative protocol that can be used, however this is not recommended.

Your client should either blindy trust encryption keys from OMEMO or prompt you to individually accept each key.

If you do not like any of the client's implementations, you can simply use your own encryption algorithms and keys and exchange them manually.

If you wish to stop talking with this user at any time, simply remove them from your contacts.
### Guide for safety when chatting in online MUCs
It's the Internet. People do not have the best intentions around. And that goes for XMPP. Due to the decentralized nature of the network it's advised that in public MUCs, especially those that are more rowdy with their moderation (or lack there of) that you take caution when opening media, websites and other third party content. If a user asks you for your JID in a semi-anonymous MUC, and you don't know who they are, they may send you unwanted material or spam.

When you see spam or other nefarious content on the network, simply ignore the user or remove them from your contacts and do not engage with them. If the content is severe enough or even illegal, it might be worth it to report the content to the user's instance administrator in order to keep everyone on the network safe.

If a user sends you illegal material on XMPP, you should immediately record any personal information about the user, such as their JID. If you accidentally opened the material, you should clear your cache of the app and ignore the user.

The majority of clients do not automatically show media when it is sent to you, which heavily decreases the chance of abuse. However, we should all stay alert to potential abuse and protect each other when we can.

Of course the potential of what you can do on XMPP is gigantic and we haven't even scratched the surface of how you can use it to its fullest extent. The best way is to learn by using. In addition, we have multiple other articles that explain how these technologies actually work, and little oddities in them.

Common questions you may have include:
> Why does the amount of members in a MUC fluctuate, why do people join and leave repeatedly?

> What's the difference between a member and a participant?

> If some rooms are semi-anonymous, are there any fully anonymous rooms?

>  How do I call a user on the XMPP network?

> How do I make my own room?

There are many things about XMPP which do not apply to typical chat platforms. Clients do a good job obscuring these quirks, but they tend to rear their ugly head once you use the protocol extensively.

We've covered all you need to know in order to get on XMPP and begin chatting. But if you want to know the ex