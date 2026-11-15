### Aslan Osmanov

Backend engineer. Python, mostly. I care about the parts of a system that fail quietly:
message delivery, caches, retries, the second request that does not look like the first.

**Open source**

Merged upstream:

- CPython · [Fix `asyncio.as_completed()` outside a running event loop](https://github.com/python/cpython/pull/157857)
- CPython · [Remove dead `_repr_info()` methods from `asyncio.windows_events`](https://github.com/python/cpython/pull/160241)
- Django · [Include the invalid view type in the `path()` / `re_path()` error](https://github.com/django/django/pull/21820)
- Django · [Reorganize the security policy page](https://github.com/django/django/pull/22052)
- Django · [Fix outdated docs for the `JsonResponse` `safe` parameter](https://github.com/django/django/pull/21725)

**What I build**

- [**txoutbox**](https://github.com/OsmnvAslan/txoutbox) · transactional outbox relay for asyncio.
  Bring your own table and your own broker; the core has no dependencies and ships contract tests
  for adapters. `pip install txoutbox`
- [**promptcachelint**](https://github.com/OsmnvAslan/promptcachelint) · explains why an LLM prompt cache missed.
  Diffs consecutive requests and names the block, the offset and the bytes that broke the prefix,
  for Anthropic and OpenAI. Zero dependencies. `pip install promptcachelint`

**How I work**

- Contracts first, then code. Small typed interfaces, adapters behind Protocols, a contract test
  suite that any adapter has to pass.
- Precision over promises. If a tool reports a number, the README says whether it is measured or
  estimated.
- Reviews are input. Every finding gets reproduced, then fixed or explicitly declined with a reason.
- Human plus agent. Much of this code is written with an AI coding agent, and the commits say so.
  The agent works under fixed rules: a failing test before a bug fix; lint, types and tests before
  every commit; an independent review pass on non-trivial diffs; nothing is pushed without my
  explicit approval.

**Elsewhere**

Notes: [osmnvaslan.github.io](https://osmnvaslan.github.io/)  
PyPI: [txoutbox](https://pypi.org/project/txoutbox/) · [promptcachelint](https://pypi.org/project/promptcachelint/)  
Also: [batch-creative](https://github.com/OsmnvAslan/batch-creative), a small Next.js app for batch image generation  
Mail: osmnvaslan@gmail.com
