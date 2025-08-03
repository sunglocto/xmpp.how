Here are all of the clients we're going to be talking about in this article.
Don't understand the terms used in this article? Check out the [Glossary](/Glossary). If you just want a recommendation for what client to use depending on your platform, see [Clients](/Clients).
![[cheogram.png]] Cheogram
![[conversations.png]] Conversations
![[dino.png]] Dino
![[gajim.png]] Gajim
![[monocles.png]] Monocles chat
![[movim.png]] Movim
![[profanity.png]] Profanity
![[psiplus.png]] Psi+

This covers the vast majority of users on the network.
 
 #TODO: Add monal
### Beginning
In networking, a client is a computer which contacts the central authoritative server. The client requests information from the server as well as respond to requests from the server and vice versa. Whilst the technologies used to make a client and their features may differ, all XMPP clients are capable of sending basic text messages to other users. The differences in these clients is far too length for us to describe in this article, so we instead will write articles based on each of these clients. We'll compare typical features that you would expect on the XMPP network between these clients and briefly explain why they exist.

# MUC (Multi User Chat)
*Does this client support joining and messaging MUCs?*
https://xmpp.org/extensions/xep-0045.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity ✅
![[psiplus.png]] Psi+ ✅

*Does this client support basic MUC history?*
https://xmpp.org/extensions/xep-0045.html#enter-history
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ❌
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity ✅
![[psiplus.png]] Psi+ ✅

*Does this client support advanced MUC history (MAM)?*
https://xmpp.org/extensions/xep-0313.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity ❌
![[psiplus.png]] Psi+ ❌

*Does this client support replies in MUCs? (not just quoting)* 
https://xmpp.org/extensions/xep-0313.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity ❌
![[psiplus.png]] Psi+ ❌

*Does this client support Reactions in MUCs?*
https://xmpp.org/extensions/xep-0444.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino (UNKNOWN)
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim (UNKNOWN)
![[profanity.png]] Profanity ❌
![[psiplus.png]] Psi+ ℹ️
*Reactions made on Psi+ do not show up on other clients*.

*Does this client support whispering in MUCs?*
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim (UNKNOWN)
![[profanity.png]] Profanity ✅
![[psiplus.png]] Psi+ ✅

*Does this client respect corrections?*
https://xmpp.org/extensions/xep-0308.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity ✅
![[psiplus.png]] Psi+ ✅

*Does this client respect retractions?*
https://xmpp.org/extensions/xep-0424.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim (UNKNOWN)
![[profanity.png]] Profanity (UNKNOWN)
![[psiplus.png]] Psi+ ❌

*Does this client respect moderations?*
https://xmpp.org/extensions/xep-0425.html
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim (UNKNOWN)
![[profanity.png]] Profanity (UNKNOWN)
![[psiplus.png]] Psi+ ❌
# Media handling
*Does this client show media in the chat window?*
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino ✅
![[gajim.png]] Gajim ℹ️
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅
![[profanity.png]] Profanity N/A
![[psiplus.png]] Psi+ ✅
*Images sent from Psi+ or monocles chat users do not appear on Gajim*

*Does this client show images by default? (This is not a good thing)*
![[cheogram.png]] Cheogram (UNKNOWN)
![[conversations.png]] Conversations  (UNKNOWN)
![[dino.png]] Dino ❌
![[gajim.png]] Gajim ❌ 
![[monocles.png]] Monocles chat ❌
![[movim.png]] Movim  (UNKNOWN)
![[profanity.png]] Profanity N/A
![[psiplus.png]] Psi+ ✅

*Can this client play videos in the chat window?*
![[cheogram.png]] Cheogram (UNKNOWN)
![[conversations.png]] Conversations  (UNKNOWN)
![[dino.png]] Dino  (UNKNOWN)
![[gajim.png]] Gajim (UNKNOWN)
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim  (UNKNOWN)
![[profanity.png]] Profanity N/A
![[psiplus.png]] Psi+ ✅ (with webview enabled)

# Security
*Does your client store credentials on the Internet?*
![[cheogram.png]] Cheogram ❌
![[conversations.png]] Conversations ❌
![[dino.png]] Dino ❌
![[gajim.png]] Gajim ❌
![[monocles.png]] Monocles chat ❌
![[movim.png]] Movim  ✅
![[profanity.png]] Profanity ❌
![[psiplus.png]] Psi+ ❌
Movim is a web client. This wouldn't be particularly bad if all of the application's logic was done client-side, such as with Matrix clients like Cinny. However it sends your credentials to the server running Movim on it. This server then contacts your XMPP server. If this server were to get hacked, your XMPP credentials could be compromised.

We recommend only using Movim instances that you or your XMPP server admin hosts.
# Encryption
*Does this client support OMEMO?*
![[cheogram.png]] Cheogram ✅
![[conversations.png]] Conversations ✅
![[dino.png]] Dino (UNKNOWN)
![[gajim.png]] Gajim ✅
![[monocles.png]] Monocles chat ✅
![[movim.png]] Movim ✅ (Disabled by default)
![[profanity.png]] Profanity ✅
![[psiplus.png]] Psi+✅ (with plugin)
