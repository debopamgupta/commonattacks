# Public Network Safety

The internet plays a gargantuan role in modern life, with most people being connected in some way virtually constantly. As such, most public spaces (e.g. cafés, restaurants, public transport) are fully equipped with public WiFI to let people catch up on email (or, equally likely, play the latest hit mobile game). What many people don't realise is that expecting public WiFi to be available can prove to be very dangerous indeed.

Public WiFi, whilst incredibly handy, also gives an attacker ideal opportunities to attack other users' devices or simply intercept and record traffic to steal sensitive information. This latter technique can be as simple as exploiting the fact that most people expect to see public networks available. The attacker can quickly set up a network of their own and monitor the traffic of everyone who connects; this is referred to as a "man-in-the-middle" attack and is very easy to carry out. For example, if you were to connect to a network belonging to an attacker then logged into an account for a website that doesn't use an encrypted (HTTPS) connection, the attacker could simply pluck your credentials out of the network traffic and use them to log into your account for themselves. This scenario will be explored in more detail in the interactive element to this task; however, it is fortunately significantly less likely to occur with modern websites which implement Transport Layer Security (TLS) to encrypt traffic between their servers and users as standard.

Equally, being connected to any network (regardless of whether you trust it or not) makes your device visible to others on the network. You never know who else is on a public network or what their intentions might be!

---

The Solutions

The ideal solution to this problem is simply not connecting to untrusted networks. Beneficial though public wireless connections are, it will always be safer to use a mobile hotspot or private network. Unfortunately, the ideal solution is not always feasible; when this is the case, we must rely on other methods of staying safe.

Virtual Private Networks (VPNs) encrypt all traffic leaving and re-entering your machine, rendering any interception techniques useless as the intercepted data will simply look like gibberish. Whilst it is possible to host your own VPN server for free, most people prefer to use one of the many online solutions. Some of these commercial solutions are free, but be warned: free VPNs tend not to provide the best security and often harvest your data themselves to make a profit. That said, the price of a good VPN is more than worth it for the increased safety when operating on untrusted networks. There are many good options around, including ProtonVPN and Mullvad VPN, to name two.

## Website Connection Security

In addition to the actions that you take to protect yourself, it is also important to be aware of the measures that online services take to protect you.

All websites should now only serve information in the safety of an encrypted connection. As with using a VPN, this prevents an attacker from reading, or modifying your web traffic if they intercept it. The encrypted connection used to create HTTPS (Hyper Text Transfer Protocol Secure) is referred to as TLS (Transport Layer Security), and in most browsers is represented by a padlock to the left of the search bar, which indicates that the connection is secure:

With this in place, your traffic can only be decrypted in very select circumstances: namely, if it is a work or school managed device and you are connected to a work/school network.

Note: The presence of the padlock indicates that the connection is secure; it does not guarantee that the website itself is safe. In other words, a malicious website can still easily have a TLS cert (meaning that your traffic with the server is encrypted), but that doesn't stop the site from having a malicious purpose.

If you are accessing a website without the padlock symbol, never enter any credentials or sensitive information — especially if you are using an untrusted network.

In some instances, you may also see a padlock with a cross through it or an exclamation mark over it; this indicates that the connection is theoretically secure but that there is something wrong with the certificate in use by the server. The presence of this altered padlock icon can mean anything from the server administrator simply letting the certificate go out of date to an attacker actively meddling with the security of your connection. In other words: if the icon is anything other than a regular padlock, do not trust that connection is secure.

> Interactive Content
