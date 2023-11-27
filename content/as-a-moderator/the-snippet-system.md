---
title: The Snippet System
weight: 40
---

If you want to cut down on saying the same thing over and over again, you can use the Snippets system. Think of callable tags, except only Staff members can create them.

<!--more-->

{{< toc >}}

## Creating a snippet

- `snip create` [name] [contents]<br>
Creates a new snippet with name `name` and the following contents.<br>
If name is not one word, please use quotes for it. The contents do not require quotes.<br>
You can set `contents` to be the name of a different snippet, and the new snippet will become an alias.

- `snip delete` [name]<br>
This will delete a snippet or snippet alias.

## Viewing snippets

- `snip`<br>
This will show all configured snippets for the server.

![Example of Snippets](/img/examples/snippets-example.png)

## Using snippets

- `snip` [name]<br>
This will display a snippet in chat.

![Example of Snip](/img/examples/snippet-plurality-example.png)