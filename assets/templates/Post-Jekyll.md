<%*
const title = await tp.system.prompt("Enter the post title:");
const userDate = await tp.system.prompt("Enter the post date (dd-mm-yyyy):");
const [day, month, year] = userDate.split('-');
if (!day || !month || !year) {
  throw new Error("Invalid date format. Please enter the date in dd-mm-yyyy format.");
}
const formattedDate = `${year}-${month}-${day}`;
const normalizeTitle = title.normalize("NFD").replace(/[\u0300-\u036f]/g, "");
const id = `${formattedDate}-${normalizeTitle.replace(/[^a-zA-Z0-9]+/g, '-').toLowerCase()}`.replace(/-+$/, '');
const filePath = `Blog/_posts/${id}`;
// Move the file to the specified folder
await tp.file.move(filePath);
-%>

---
layout: post
title: "<% title %>"
id: "<% id %>.md"
categories:
image: https://lh3.googleusercontent.com/pw/AP1GczMke9JuL30aTXCysOC4P9Ukh-rZKQB2WUerf7Azkc0dqwYpGq1gfRtkwTf6_tySztCNblJBxZ9Z6qBJ0vgY1oYQ1gc8dCwgN8AyQcEkR_jx8YLMvWUtehCvseuV4jnsQN1d7MIxww1bZbVhpaq04B2V=w997-h1026-s-no-gm?authuser=0
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/<% id %>.md
tags: 
date: <% formattedDate %>
author: eduardo
---
## <% title %>
or question/headline catchy

#prompt 
Olá xuxuGPT, estou revendo um texto do meu blog e pensando nos 5 blocos de informação que acho importante ter: 
- **Inspiration** and Motivation
- What does this do? **clear description**
- Connections with the references
- What are the next steps? **outcomes**
- What did I learn from this?


