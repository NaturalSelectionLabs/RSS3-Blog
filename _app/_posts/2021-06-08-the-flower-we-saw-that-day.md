---
layout: post
title: The Flower We Saw That Day
author: diygod
heading-bg: "https://i.imgur.com/b5nSM08.png"
heading-bg-local: false
heading-bg-color: "#00c700"
heading-bg-size: "5001px 2813px"
heading-bg-position: "center bottom"
heading-bg-repeat: "repeat"
heading-bg-text: "#fff"
---

Maybe ten years ago, an idea inspired me so much, called "The Spirit of the Internet". I no longer remember where it originated, but everyone generally agrees that the Internet spirit should be open, equal, collaborative, and shared. It is as beautiful as a flower, which touched me as a young man, looking forward to the bright future of the Internet with these characteristics.

But today, it is slowly being forgotten.

Content platforms now hold the power of controlling how users disseminate, distribute and obtain contents. Platforms have built high walls, keeping user-generated contents inside as their own treasure. Users actively or forced to give up their rights and hand them over to the platforms. This leads to trashy platforms run wild, which is really unbelievable. When information loses its power to interconnect, "Internet" is no more than just a name.

Platforms also control what can be created. Everyone should express their ideas freely, without being subject to any type of censorship or restriction from any centralized party. This is a fundamental human right and a basic right for any cyber persona. However, the reality is that platforms have complete control over what can and cannot be created and distributed. They can also remove contents that should belong to their creators at will.

The Internet shouldn't be like this.

The original RSS was the perfect interpretation of the spirit of the Internet and the pioneer of the old era. But it has been having trouble adapting to the new generation. I deeply realized this in the process of developing and maintaining the open-source project RSSHub ([https://github.com/DIYgod/RSSHub](https://github.com/DIYgod/RSSHub)). It cannot solve the problems mentioned above since it has fatal issues in its original design. It keeps the original data still on content platforms. It lacks a way for users to connect with one another through contents and become almost impossible to introduce any business logic for developers and content creators to benefit from. Without fundamental changes, it is impossible to adapt to the new era and destined only for the minority.

Therefore, the Internet needs a new open and inclusive protocol for building social and content networks. We call it RSS3. The proposal has been published on GitHub: [https://github.com/NaturalSelectionLabs/RSS3](https://github.com/NaturalSelectionLabs/RSS3)

- Change from XML to simplify and more efficient JSON
- Cryptographic keypairs are used to authenticate and verify the integrity
- Connections between users are recorded through links and backlinks
- Content interactions are recorded through upstream and contexts
- Contain different types of contents with mime_type
- Paging through items_next and list_next to support storing more content

For creators, everyone can upload RSS3 files that conform to the standard format to the distributed network, recording their personal information, relationships, and contents in the files, and hold the private key to hold the full ownership. Modifying permissions, publishing content, following other creators, and interacting with other contents only need users to alter their RSS3 files with ZERO interference from any centralized party.

For applications, each one can obtain the contents from creators equally. That is, from the RSS3 files of creators. Applications can no longer monopolize and control the contents. Users can switch to any application at any time without worrying about losing existing contents.

For distributed nodes, they will be hosting RSS3 files, maintaining the connections among RSS3 files and the reverse indexes of content interactions, storing permanent data such as transactions and contributions, and using a transparent algorithm to mark creators and content to achieve a user-controllable recommendation system, etc., of course, you can also get rewards for your own work.

As for platforms, let them fade into history.

Hope that RSS3 can help creators regain their own rights from centralized content platforms, making the Internet what it should be, and re-bring the flower we once saw but has forgotten its name.