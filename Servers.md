XMPP is not like traditional instant messaging platforms. Most platforms simply allow you to create an account with an email address/phone number and a password and you're instantly connected to a centralized service. Because of the nature of XMPP, you must **choose an instance** to keep your account and sessions on. This instance will then connect to other servers on your behalf, allowing you to communicate with others across the XMPP network.

XMPP servers are like mailboxes that you sign up to be a recipient of. You can receive mail from that mailbox and use that mailbox to send mail to others. This means that if other servers die, you won't be able to contact people on those servers, but you will still be able to use the network. However, if your own server dies, you will have to migrate to another server. If you wish to become more independent, you should [host your own server](/Make%20your%20own%20server).

## How to choose

# Using a Friend's Server

If a friend of yours runs a server (or is interested in running one and has the know-how), it is highly recommended to ask for an account on their server, for the following reasons:
- Higher Limits; private server owners will often set the usage limits of the server much higher than public servers, such as how large files can be, how long messages are stored, and how many sessions you can run on one account.
- Know Your SysOp; because you know your systems operator, you can directly ask them for help, including for things a public server owner might refuse (i.e. manually resetting your password, provisioning more accounts).
- Management; if you want to just chat and don't care to learn, your SysOp is probably willing to manage some aspects for XMPP for you.
- Roster Groups; a more specific feature. The SysOp can put you and some other users of the server in a roster group, which automatically adds all users of that group as contacts of each other. Extremely useful for families or tight friend groups.
- Low-Profile; The chances of a private server getting any sort of spam is effectively 0, as it is not well known. More hardline systems operators can disable federation outright to prevent all spam.
- Decentralization; More servers = more decentralization = more robust network over all. Also, that means that outages will usually not affect you.

# Choosing a Public Server

There are multiple websites online which catalog servers on the network as well as their ease of use, registration policy (how much work you have to do to make an account), uptime and general server quality. A server that you as a beginner should choose should have the following characteristics:
- Easy to register
- High uptime/Low downtime
- Located in a privacy-respecting country
- Low or affordable cost

We have information about individual servers in the **Server Information** category.

*xmpp.how does not endorse nor recommend any individual servers shown in these screenshots.*

### 1) https://providers.xmpp.net/

XMPP Providers is a **curated list of publicly available XMPP servers**. It ranks servers based on ease of registration, cost, compatibility and more factors. XMPP Providers does not show that many servers by default as many of them are D-tier or below, mainly due to closed registration, low compatibility and not being able to register in XMPP apps.

Here is what the site looks like, with the list of servers that are available (D-tier has been omitted for reasons above):

![[Pasted image 20250801124303.png]]

### 2) https://list.jabber.at/
list.jabber.at is a list of XMPP servers sorted in alphabetical information. Unfortunately this list does not show advanced information about the servers other than the certificate authority, country and contact information. Despite this, list.jabber.at shows more servers than XMPP providers, so if you want to have a wider variety of servers to pick, this might be a good option.
![[Pasted image 20250801124725.png]]

### 3) https://jabberworld.info/servers/
This is probably the most advanced server list in this article, and is not recommended for XMPP beginners. It shows an automatic list of discovered XMPP servers in alphabetical order. Instead of showing their ease of registering, it instead shows the features that the server supports, such as hosting MUCs or storing files. If you are an advanced user and do not mind the site being outdated, this could be a good choice.
![[Pasted image 20250801125241.png]]

Once you've installed a client and picked a server, it's [time to create your XMPP account](/Creating%20an%20account)!