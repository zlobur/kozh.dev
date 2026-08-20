# kozh.dev

Personal site — portfolio, blog and notes. Built with [Astro](https://astro.build)
on the [astro-navfolio](https://github.com/dodolalorc/astro-navfolio) theme (MIT).

## Development

Requires [Bun](https://bun.sh).

```sh
bun install
bun run dev      # dev server on http://localhost:4321
bun run build    # production build into dist/ + Pagefind search index
bun run preview  # serve the production build
```

## Content

| Path                    | What it is                                    |
| ----------------------- | --------------------------------------------- |
| `src/content/about.mdx` | About page                                    |
| `src/content/blog/`     | Blog posts                                    |
| `src/content/projects/` | Project cards (`index.mdx` is the page intro) |
| `src/content/vibe/`     | Short notes                                   |
| `src/config/site.toml`  | Site title, links, navigation, home page      |

Entries with `draft: true` are not published.

New entries:

```sh
bun run post:new
bun run project:new
bun run vibe:new
```
