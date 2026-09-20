### Aslan Osmanov

Backend engineer. Python, mostly. I care about the parts of a system that fail quietly:
message delivery, caches, retries, the second request that does not look like the first.

**What I build**

- [**promptcachelint**](https://github.com/OsmnvAslan/promptcachelint) · explains why an LLM prompt cache missed.
  Diffs consecutive requests and names the block, the offset and the bytes that broke the prefix,
  for Anthropic and OpenAI. Zero dependencies. `pip install promptcachelint`
- [**txoutbox**](https://github.com/OsmnvAslan/txoutbox) · transactional outbox relay for asyncio.
  Bring your own table and your own broker; the core has no dependencies and ships contract tests
  for adapters. `pip install txoutbox`
- [**batch-creative**](https://github.com/OsmnvAslan/batch-creative) · product photos plus one
  reference image in, a consistent series of social posts out. Image-to-image generation with
  failover, streamed over SSE, persisted in SQLite. Next.js.

**How I work**

- Contracts first, then code. Small typed interfaces, adapters behind Protocols, a contract test
  suite that any adapter has to pass.
- Precision over promises. If a tool reports a number, the README says whether it is measured or
  estimated.
- Reviews are input. Every finding gets reproduced, then fixed or explicitly declined with a reason.

**Elsewhere**

PyPI: [promptcachelint](https://pypi.org/project/promptcachelint/) · [txoutbox](https://pypi.org/project/txoutbox/)  
Mail: osmnvaslan@gmail.com
