*This refers to the action of moderating a room, not the specific state of a moderated message or MUC. Please refer to the [Glossary](/Glossary) for more details.*

In this article, we will describe methods and solutions of protecting a public room, also known as a Channel.
### Best tips
Depending on the size of the room, you should have different security measures. In small but easily accessible rooms, you should almost certainly have moderated mode ON. This is where ![[noaffiliation.png]]Visitors cannot send messages into the MUC until they have been promoted to ![[noaffiliation.png]]Participant by a moderator. In order to do this, you will need to configure the room and set "Moderated" to true:
![[Pasted image 20250802152000.png]]

If your MUC is particularly large, it's advised you have multiple moderators in different time zones in order to deal with spam or other types of abuse:
![[Pasted image 20250802152212.png]]

If you do not own the server that your room is being hosted on, then this is essentially all you can do given today's tools and features. However, if you are the owner of the server, or you can communicate with the admin to enable features which make it easier to moderate.

### Server tips
These mainly revolve around blocking servers to prevent spam. However, you should only do this as a **last resort** because blocking servers decreases the strength of the network and impacts your own experience. If spammers are active on a particular server, please report 
1) Enable XMPPBL
XMPPBL is a service for enabling real-time blocklists of spammers for your server. When a spammer has been identified on the network, it's possible to add their JID onto the blocklist and have them simultaneously blocked from accessing multiple servers and rooms, including your own. You can read more about it [here](https://xmppbl.org).

However if you are concerned that this type of blocklist may be used for reasons other than simply blocking spammers, you can decide not to install it and block spammers on a case by case basis. In addition, anybody added to the list will automatically be removed after a set period of time.

2) S2S blocks
If you have identified a server as a particular source of spam or other unwanted contact, you can block it if you're sure that the server's administrators are either participating in the abuse or unresponsive. Both Prosody and ejabberd have tutorials and modules on how to block S2S communication.

An S2S block is the preferred method because you can set a reason for the block the admin of the blocked server will see it. This will allow them to negotiate with you about the disagreeable content, allowing you to resolve issues.

3) /etc/hosts
If spammers from a particular server are even bypassing these blocklists, it's possible to completely block all communication with a server by setting its IP address in /etc/hosts to 0.0.0.0, like so:
```
0.0.0.0 badserver.org
```

Keep in mind this is a complete two-way block. People from `badserver.org` won't be able to contact you and vice versa. In addition, the blocked server will not have any indication that they have been blocked, because this simply times out the connection instead of responding.

4)