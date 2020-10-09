---
layout: layouts/post.njk
title: Why you should try IPFS
date: 2020-10-09T20:39:31.287Z
description: This is why you should try IPFS.
tags:
  - ipfs
---
Today, I will try to convince you to at least try IPFS.

### Integrity built in.

Let me explain the difference between content-based addressing and location-based addressing. This will help you understand how the integrity works:

- Location-based addressing is where a client would know exactly where a file is. 
- Content-based addressing is where a client would ask what the contents of a file is, verifying the contents were not modified using a hash. So, unlike Location-based addressing (HTTP), it has more security.

### Peer-to-Peer file storage

You can say goodbye to those servers hosting your data (such as AWS S3 and Google Drive) and say hello to Peers! What is a peer? Peers can be a client, and a server. They can replace servers if there are enough of them. Why peers instead of s server? If a peer goes down, other peers can give you the data you need. But if a server goes down, that data is gone until the server is back up.

### A programmatic API.

Like many things, it has an API. From running a node (peer) on your web browser ([js-ipfs](https://js.ipfs.io/)) to interacting with nodes hosted on a user's computer (See their docs for their [HTTP API](https://docs.ipfs.io/reference/http/api)).

Those were some things I wanted to talk about because not many people are willing to try IPFS. If you want to learn more about IPFS, you can check out the (many) links below:

- [Awesome IPFS - a awesome list of projects that are made/are using IPFS.](https://awesome.ipfs.io/)
- [ipfs.io - The main website for IPFS](https://ipfs.io/)
- [Install IPFS](https://ipfs.io/#install)
- [IPFS docs - The official docs for IPFS. They have many tutorials on how to deploy websites to IPFS and how to install IPFS](https://docs.ipfs.io/)
- [Get started with IPFS in the browser](https://github.com/ipfs/js-ipfs/tree/master/examples/browser-script-tag)
- [Get started with IPFS in Node.js](https://github.com/ipfs/js-ipfs/tree/master/examples/ipfs-101)