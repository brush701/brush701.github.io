---
layout: post
title: On Crypto
---

#### Merkle Trees
When I started writing this post, I had intended to avoid diving into the
technical details of blockchain or cryptocurrencies. The plan was to link out
to high-quality articles on these topics so that the interested reader could
learn more at their own discretion. Unfortunately, a cursory search didn't turn
up any articles on Merkle trees that I found sufficiently accessible for the
non-techincal reader. So here's my brief overview on the topic.

Let's take the "tree" bit first. For computer scientists, a tree is a way to
represent specific types of relationships between things. The
[Wikipedia Article](https://en.wikipedia.org/wiki/Tree_(data_structure)) on
trees is actually pretty good, but the short version is that every tree has a
"root node," which just means a starting place. That root node might have 1, 2,
or more child nodes, and each of those children can have children, and so on.
The obvious and familiar example of this would be a family tree.

![Tree](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/Binary_tree.svg/300px-Binary_tree.svg.png)

A Merkle tree is just a very special kind of tree where each node is labeled
with a unique and un-forgeable "ID code" that is based on all of its children.
The most important property of this ID is that if you change any of the
children, grandchildren, etc. even a little bit, the ID for the node will be
completely different. If you're curious about how this works, check out this
article on [hash functions](https://en.wikipedia.org/wiki/Hash_function).  
