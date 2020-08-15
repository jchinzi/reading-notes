## [Intro to EJS in ExpressJS](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

- Use case often include nav bars and footers (pieces that stay static)

In Layout.EJS:
> <%- include('partials/onepartial') %>

In Partials/onepartial:
- Add html as needed

---

## [EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)

Partials allow one to rueuse the same HTML across multiple views

- Create an ejs file that contains the HTML you want to reuse
- Then use <%- include(PARTIAL_FILE) %> where the partial file is relative to the template you use it in.

---

[Home](https://jchinzi.github.io/reading-notes/)