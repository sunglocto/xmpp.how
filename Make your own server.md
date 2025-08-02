*This article will refer to XMPP as Jabber in order to prevent acronym overload. They mean the exact same thing.*

*This is recommended for people who either already have skills in system administration or server management. Making and maintaining a Jabber server requires a domain, server, security knowledge, free time and overall determination. If you do not wish to make a Jabber server, you do not have to do so in order to join the network. We have [multiple articles explaining how to discover and register on servers on the network](/servers). Please do so instead of going in head-first into the ecosystem, or else you are likely to have a very bad time.*

*We also cannot give you advice for every single scenario you might be put into. If you are going to go down this route, please learn how to use a Linux server or another *NIX family operating system before you do this.*

Creating and hosting a Jabber server is a way to become fully independent from a single instance administrator. It allows you to become the boss of your own communications, essentially becoming your own mailman and post office. You'll be able to make any changes you want, and can have as much users on your user as your specs will allow. You also can't be taken off your own server by any one person, because you're the administrator! You also don't rely on anyone else, and if you're the only user of the instance, you can shut it down at any time without any warning and have zero secondary impacts on other users. 

You can also use the infrastructure to host other things, maybe a website or a Jellyfin server can be added alongside your Jabber server. The opportunities of self-hosting are very beneficial, and as chat platforms such as Discord begin the process of [enshittification](https://en.wikipedia.org/wiki/Enshittification), it makes perfect sense to become more independent.

### What do I need
The shopping list for a Jabber server is as follows:
- A Virtual Private Server (VPS) 
  OR
- A server connected to the internet that is ***NOT*** behind CGNAT
- A domain
- An SSH terminal on a separate computer

### Can I host from home?
Yes, but your ISP may not let you.  
- Many ISPs will not allow you to access port 80 and 443, which is required to obtain TLS certificates.  
- Some ISPs don't give you a connection capable of port forwarding, like those behind CGNAT.  
- Even if an ISP does seem to allow you to port forward, if you become too well known, your ISP may demand you purchase a business plan, which is more expensive.  
Furthermore, even if your ISP lets you (or simply does nothing to you), and you can port forward, there are certain UX and privacy implications.  
- Your IP address may point to your place of residence through GeoIP.  
- Residential connections are usually optimized for consumption, not hosting. You will likely have very poor upload speed compared to download speed. While this doesn't affect the XMPP protocol itself, it does affect things like file uploading.  
- You might only have an IPv6 or IPv4 address, which means some people cannot connect to you.  
- Some public networks disallow connecting to residential IPs.  
- Residential connections are usually not attached to big internet hubs that can heavily optimize speed when making cross-country connections.  
- If your power goes out, your server is down.  
  
If you still want to run a server at home, we highly recommend running one in conjunction with a VPS if you can. Use the VPS server for public stuff and connecting with whom you don't know well, and use your home server for people you trust very well.

Once you have all of these things, it's time for you to pick a Jabber server implementation.

There are five main XMPP Server Implementations. All of them support roughly the same XEPs, so you don't have to worry about server support; instead, the pros and cons will focus on their use as a server operator. 
  
## Ejabberd
 
### Pros:  
- Strong out of the box experience; contains most XEPs you want, and has a built in turn-server that support user authentication with XMPP.  
- Supports PLAINTEXT, SCRAM-SHA-1, SCRAM-SHA-256, SCRAM-SHA-512, etc for authentication. Has the option of allowing multiple options for maximum client accessibility, clients usually choose the most strong option they support. I use SCRAM-SHA-256(-PLUS) which is supported by older clients and SCRAM-SHA-512(-PLUS) which is supported by newer clients, both of which are secure options.  
- Incredibly flexible configuration.  
- Built in HTTP REST API, useful for making very simple bots and other functions.  
- high availability; can be clustered  
- multi-threaded by default, so it's fast by default even with something like SQLite3. (But pairs well with an equally multi-threaded DB like Postgresql)  
- the developer of Conversations specifically targets ejabberd as a benchmark for compliance.  
- Mature and historically well designed, has existed since 2002. Used by a lot of companies.  
- Managed by a for-profit company with a good track record. If you like the stability of companies, this is an advantage.  
  
### Cons:  
- A couple of terrible defaults in the example configuration, mainly that the default authentication is plaintext.  
- Some parts of it need to be automated, but it is fairly easy to do so.  
- A database is required. SQLite3 is the easiest to use. Supports many options.  
- Documentation reads like a manual; it'll tell you what things do and explains them fairly well, but it doesn't tell you _how_ things ought to be used, besides the example configuration. You'll need some understanding of XMPP to understand the documentation.  
- If you need to extend ejabberd itself and Jabber Component Protocol or its API is not enough for you, you'll need to know Erlang, which is a somewhat uncommon language.  
- Licensed under the GPL with a CLA. (Would be better licensed as AGPL)  
- Managed by a for-profit company. If you distrust companies, this is a flaw.  
  
### Prosody 
### Pros:  
- Great to develop on, easy to extend. Lua is a simple programming language, and you might already know it if you've developed for GMod, Roblox, etc.  
- The basic prosody package contains most of the XEPs you need, but it has a wealth of community made modules to further extend prosody's functionality.  
- Great documentation.  
- Doesn't require a database, but one is highly recommended. You can use PostgreSQL or SQLite3, among others.  
- Authored by a collective of volunteer developers. Trust in the community!  
- Licensed under MIT. You have free reign to do what you like.  
  
### Cons:  
- Single-threaded. It is still quite fast.  
- Modifying the configuration without restarting is slightly more involved.  
- Changing certain modules _requires_ a restart.  
- Licensed as MIT. Pushover license.  
- Authored by a collective of volunteer developers, meaning that support might be few and far between.

Once you have a server, let's learn [How to use XMPP!](/How%20To%20Use%20XMPP)