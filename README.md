# SystemDesignConcepts

### Public IP Addresses: Your Internet Passport

Picture a public IP address as your unique Internet passport. It's a globally distinctive identification assigned by your Internet Service Provider (ISP). This tag makes your home or business network identifiable in the vast ocean of the Internet. When you connect to the Internet, your public IP is what the world sees, much like a license plate on a vehicle in traffic.

When you're surfing the web and visit a website, the server of the website treats your public IP as your unique identifier, just like an airport identifies you by your passport number. This is how the server knows where to deliver the webpage you requested. It's not your device it sees directly, but rather your public IP address, your Internet identity.

Let's delve into the fascinating roles public IP addresses play:

**Web servers:** Imagine you've painted a stunning picture and you wish to display it to the world via your website. To enable Internet users to access it, your server would need a public IP address, much like a gallery needs a street address.

**VPNs (Virtual Private Networks):** VPN servers are like private tour guides in the realm of the Internet. They use public IP addresses to communicate with devices, taking them on a secure journey across the web, often to destinations otherwise inaccessible.

**Email Servers:** Think of public IP addresses as the postal service of the Internet. Just like post offices use physical addresses to send and receive letters, email servers use public IP addresses to send and receive emails over the Internet.

The unique identity that a public IP address provides ensures a smooth and secure operation of the Internet. It's a critical component in the infrastructure that keeps the digital world spinning.

### Private IP Addresses and Their Uses

While traversing the complex structure of networks, have you ever wondered about the unique address assigned to your devices within your confined network? Be it your house, workplace, or a large enterprise setting, these exclusive addresses are termed as Private IP Addresses.

Private IP addresses, akin to an exclusive membership card, cater to devices within a closed network. They're comparable to internal phone extensions within a large office. You can dial the extension from within the office, but not from an outside line. These IPs are the internal extensions for your routers, PCs, printers, smartphones, and a horde of other devices functioning within your private network.

Imagine the private IP as the unique name your home router affectionately assigns to your personal devices. It is like your pet name used only within your family, while your formal name is used for communication with the outside world. They typically fall into the following ranges:

- The modest suburban neighborhood: 192.168.0.0 - 192.168.255.255
- The isolated countryside farmhouse: 172.16.0.0 - 172.31.255.255
- The bustling city apartment: 10.0.0.0 - 10.255.255.255

These reserved ranges are like gated communities for private networks, separated from the vast Internet by the guardianship of Internet standards groups. If a device from your network decides to visit the Internet, much like stepping out of its gated community, it sends a request to the router. Acting like a concierge, the router then presents this request to the Internet.

Private IP addresses are often seen in action:

- Facilitating communication within a homely setup or a large corporation. They're like the intercoms within a household.
- Offering exclusive access to a private database in a LAN, akin to a secret library within a castle.
- Functioning in a secluded setting, like a school or office, not unlike a walkie-talkie system during a camping trip.

The divide between public and private IP addresses serves a dual purpose. It ensures that the private network is secure, much like a sanctuary guarded from the outside world. It also helps to maintain the limited quota of public IP addresses available, similar to conservation efforts for endangered species. This balance is essential to ensure the Internet can continue to grow and connect more devices.

### Network Address Translation (NAT): The Clever Facilitator

Imagine a vast party happening on the Internet, where your private network wants to participate, but there's only one formal invitation, i.e., one public IP address. Here's where NAT, or Network Address Translation, steps in as the clever event organizer.

NAT allows all the devices on your private network to join the grand Internet party using a single public IP address. It's as if all your devices don a single mask - the public IP address - when they step out onto the global Internet stage.

Think of NAT as the crafty translator and manager at this event. It translates the private IP addresses of your network's devices into the public IP, allowing them to communicate with the Internet. When the communication needs to come back, NAT translates in reverse, ensuring that the right responses reach the correct devices.

This crafty management is crucial for preserving the limited number of VIP passes, or public IP addresses, especially under the IPv4 protocol, which has a finite number of these unique identifiers.

Let's walk through this process with an example: When a device from your network - let's call it Alice - decides to access a website, your router, playing the role of the vigilant doorman, uses NAT to send Alice's request onto the Internet, wearing the mask of the public IP.

The website's server doesn't see Alice; it only sees the public IP mask. It sends its response back to the masked figure - the public IP. Then, our vigilant doorman, the router, ensures this response is forwarded back to Alice in your network. This intricate dance of requests and responses occurs seamlessly and in real-time, making the Internet experience smooth and efficient.
