# relaxed-citationjs

This ReLaXed plugin provides utilities to create bibliographies in ReLaXed
using [``citation-js``](https://citation.js.org/).

This plugin wraps code originally written by @Drew-S in the core ReLaXed project.


## Usage

Install with ``npm install -g relaxed-citationjs`` and add ``citationjs`` to the plugins of
your project's ``config.yml``:

```yaml
plugins:
  - citationjs:
      jpeg-quality: 90
```

Then use the ``+cite`` and ``+bibliography`` mixins in your document's Pug source:

```pug
p Refer to the great work in #[+cite('Q21972834', '23-25')] and #[+cite('Q21972835')].

+bibliography

```