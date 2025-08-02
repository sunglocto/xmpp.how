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

Once you have all of these things, it's time for you to pick a Jabber server implementation. As of writing, the best two implementations are **Prosŏdy** and **ejabberd**.

# TODO - Add chart comparing differences between Prosŏdy and ejabberd

Once you have a server, let's learn [How to use XMPP!](/How%20To%20Use%20XMPP)