# Microsoft Exchange Autodiscover Flaw
These domains are part of an autodiscover flaw in Microsoft Exchange.
* [Reddit post](https://www.reddit.com/r/sysadmin/comments/pt8097/microsoft_exchange_autodiscover_bugs_leak_100k/?utm_source=share&utm_medium=ios_app&utm_name=iossmf) for more information
* [Original Article](https://www.guardicore.com/labs/autodiscovering-the-great-leak/)
* Domains taken from official repo [here](https://github.com/guardicore/labs_campaigns/tree/master/Autodiscover)

_A snippet from the article:_

* Autodiscover, a protocol used by Microsoft Exchange for automatic configuration of clients such as Microsoft Outlook, has a design flaw that causes the protocol to “leak” web requests to Autodiscover domains outside of the user’s domain but in the same TLD (i.e. Autodiscover.com).

* Guardicore Labs acquired multiple Autodiscover domains with a TLD suffix and set them up to reach a web server that we control. Soon thereafter, we detected a massive leak of Windows domain credentials that reached our server.

* Between April 16th, 2021 to August 25th, 2021 we have captured:
    * **372,072 Windows domain credentials** in total.
    * **96,671 UNIQUE** credentials that leaked from various applications such as Microsoft Outlook, mobile email clients and other applications interfacing with Microsoft’s Exchange server.
* This is a severe security issue, since if an attacker can control such domains or has the ability to “sniff” traffic in the same network, they can capture domain credentials in plain text (HTTP basic authentication) that are being transferred over the wire. Moreover, if the attacker has DNS-poisoning capabilities on a large scale (such as a nation-state attacker), they could systematically syphon out leaky passwords through a large-scale DNS poisoning campaign based on these Autodiscover TLDs.

* Additionally, we have developed an attack – “The ol’ switcheroo” – which downgrades a client’s authentication scheme from a secure one (OAuth, NTLM) to HTTP Basic Authentication where credentials are sent in clear text.

