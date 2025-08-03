A Multi-User Chat is a chatroom on the XMPP network that can hold multiple members. MUCs are similar to a singular channel in a Discord server, where all messages belong in a single room. MUCs are now one of the foundational structures of XMPP communication, and you will almost certainly experience them during your time on the network.

A MUC is not decentralized as you may believe. MUCs are hosted on a single server which is fully authoritative. This also means that if the server running the MUC goes down, the MUC will die. This is unlike other chat platforms such as Matrix, where only the servers who run the users' accounts need to be online, the server running the original room could die and the room would still exist.

MUCs also are not like typical rooms in conventional chat platforms. Joining a MUC does not mean you are permanently in that MUC. When you see participants in a MUC, they are actively connected to that MUC at any one time. This is similar to people playing a Minecraft server for example. You can leave the server at any one time, and join back with your original identity, items and position in the world. It works the exact same way in XMPP.

## Affiliations and roles
We've been referring to Visitors, Participants, Members, Moderators, Administrators and Owners as their own separate permission structures. This is actually a lie.

The majority of conventional chat platforms simply have a flat permission structure. Power levels for Matrix, Roles for Discord and Administrator and Owner statuses for WhatsApp are examples. This is actually not the case, and there is a difference between a user's **role** in a chatroom and their **affiliation** in the chatroom.

Affiliations retain with the users JID, whereas roles retain with the users Nickname.
There are four affiliations that a user can be, and a user can be unaffiliated:
![[outcast.png]] Outcast
![[noaffiliation.png]] Unaffiliated
![[member.png]] Member
![[admin.png]] Administrator
![[owner.png]] Owner

There are 3 roles that a user can be:
![[noaffiliation.png]] Visitor
![[noaffiliation.png]]/![[member.png]] Participant
![[admin.png]]/![[owner.png]] Moderator

As stated before, a users role is tied to their nick, whereas their affiliation is tied to their JID. However, the affiliation of a user dictates their role, or an action that takes place.

For example, if your affiliation is ![[outcast.png]]Outcast, then you cannot join the room, because you have been banned.

If your affiliation is ![[noaffiliation.png]] non-existent, then your role is determined by the **Moderated** status of the room. Moderated refers to whether or not newcomers will have to be given Voice by moderators when they join the room.

If the room IS moderated, then your role will be a Visitor, meaning you will be muted.

If the room IS NOT moderated, then your role will be a Participant.

If your affiliation is ![[member.png]]Member, then you will automatically be a participant regardless of the room's moderated status.

If your affiliation is ![[admin.png]]Administator, you will automatically be a moderator, but will NOT be able to configure a room.

If your affiliation is ![[owner.png]], you will automatically be a moderator, but you WILL be able to configure a room.

