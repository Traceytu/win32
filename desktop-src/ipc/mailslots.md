---
Description: A mailslot is a mechanism for one-way interprocess communications (IPC). Applications can store messages in a mailslot. The owner of the mailslot can retrieve messages that are stored there.
ms.assetid: 9a68905d-c235-4c72-bc71-1cccdf5cdadc
title: Mailslots
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Mailslots

A *mailslot* is a mechanism for one-way interprocess communications (IPC). Applications can store messages in a mailslot. The owner of the mailslot can retrieve messages that are stored there. These messages are typically sent over a network to either a specified computer or to all computers in a specified domain. A *domain* is a group of workstations and servers that share a group name.

-   [About Mailslots](about-mailslots.md)
-   [Using Mailslots](using-mailslots.md)
-   [Mailslot Reference](mailslot-reference.md)

You can choose to use [named pipes](named-pipes.md) or [Windows Sockets](https://msdn.microsoft.com/library/windows/desktop/ms740673) instead of mailslots for interprocess communications. Named pipes are a simple way for two processes to exchange messages. Mailslots, on the other hand, are a simple way for a process to broadcast messages to multiple processes. One important consideration is that mailslots broadcast messages using datagrams. A *datagram* is a small packet of information that the network sends along the wire. Like a radio or television broadcast, a datagram offers no confirmation of receipt; there is no way to guarantee that a datagram has been received. Just as mountains, large buildings, or interfering signals might cause a radio or television signal to get lost, there are things that can prevent a datagram from reaching a particular destination. Named pipes are like telephone calls: you talk only to one party, but you know that the message is being received.

 

 


