# Content

## Working links

### Bare URLs

- Bare URL (HTTP, redirects to HTTPS): http://en.wikipedia.org/wiki/Main_Page
- Bare URL (HTTPS): https://en.wikipedia.org/wiki/Potato

### Markdown links

- [Markdown link (HTTP, redirects to HTTPS)](http://en.wikipedia.org/wiki/Association_football)
- [Markdown link (HTTPS)](https://en.wikipedia.org/wiki/Existence)

### Inline code

- Inline code (HTTP, redirects to HTTPS): `http://en.wikipedia.org/wiki/Hamster`
- Inline code (HTTPS): `https://en.wikipedia.org/wiki/Code`

### Code block

- Code block (HTTP, redirects to HTTPS)
  ```shell
  curl http://en.wikipedia.org/wiki/Cactus
  ```
- Code block (HTTPS)
  ```shell
  curl https://en.wikipedia.org/wiki/Abacus
  ```

---

## Non-working links

### Bare URLs

- Bare URL (non-existent page): https://en.wikipedia.org/wiki/Non-existent-page (expect `HTTP 404`)

### Markdown links

- [Markdown link (non-existent page)](https://en.wikipedia.org/wiki/Nothing-is-here) (expect `HTTP 404`)

### Inline code

- Inline code (non-existent page): `https://en.wikipedia.org/wiki/Page-not-found` (expect `HTTP 404`)

### Code block

- Code block (non-existent page) (expect `HTTP 404`)
  ```shell
  curl https://en.wikipedia.org/wiki/Nothing-to-see
  ```
