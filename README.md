# p-nautilus.github.io

Bilingual website of p-Nautilus (English and Spanish). Static HTML and CSS, no build step, no JavaScript beyond the language redirect on the home page.

```
index.html          redirects to /en/ or /es/ by browser language
en/index.html       English page
es/index.html       Spanish page
assets/css/style.css
assets/img/favicon.svg
404.html, robots.txt, sitemap.xml, .nojekyll
```

## Edit

The two language pages have the same structure. Change both when you change one.

Preview locally:

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

## Notes

- Fonts (Alegreya, Hanken Grotesk) load from Google Fonts. To avoid third-party requests, download them into `assets/fonts/` and replace the `<link>` in both pages with `@font-face` rules.
- Links to the GitHub organization and the `harness` repository assume the organization is named `p-nautilus`.
- The hero figure plots the roots of Lehmer's polynomial. It is static SVG.

---

# p-nautilus.github.io (español)

Sitio web bilingüe de p-Nautilus. HTML y CSS estáticos, sin paso de compilación. Las dos páginas (`en/` y `es/`) tienen la misma estructura: si cambias una, cambia la otra. Para ver el sitio en tu computador: `python3 -m http.server 8000` y abre http://localhost:8000/.
