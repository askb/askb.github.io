# askb.au

Personal site — one static page. No framework, no build step, no JavaScript.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The page |
| `style.css` | Design tokens + layout |
| `fonts/` | Archivo + Space Grotesk, latin subset, self-hosted |
| `robots.txt` | `Disallow: /` while unpublished — **delete before launch** |

## Preview

```bash
cd ~/git/github/personal/askb.github.io && python3 -m http.server 8000
```

Use `&&`. If the directory is wrong, `cd` fails, the shell stays put and
`http.server` silently serves whatever it was already in. A directory listing
means there is no `index.html` where you are serving from.

## Deploying

GitHub Pages, branch `main`, `/` root. Pages is **always public** on a
personal account — private Pages is Enterprise Cloud only.

Launch order: delete `robots.txt` → repo public → enable Pages → add `CNAME`
containing `askb.au` → tick **Enforce HTTPS** once the certificate issues.

## Licence

Code MIT. Content © Anil Belur.
