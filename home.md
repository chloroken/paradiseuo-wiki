---
title: Home
description: Welcome to Paradise, a T2A Ultima Online shard for solo players and small groups
published: true
date: 2026-11-24T03:59:27.935Z
tags: 
editor: markdown
dateCreated: 2026-11-03T21:50:31.643Z
---

# Home
Welcome to the *Paradise* wiki. The articles here cite the shard's code directly.

See [Getting Started](/getting_started) to join the server.
See [Features](/features) for how the shard differs from T2A.

The wiki has <span id="page-count">many</span> pages.

<script>
window.boot.register('page-ready', () => {
  fetch('/graphql', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ query: '{ pages { list(limit: 5000) { path isPublished } } }' })
  })
    .then(r => r.json())
    .then(d => {
      const n = d.data.pages.list.filter(p => p.isPublished).length;
      document.getElementById('page-count').textContent = n;
    })
    .catch(() => {});
});
</script>