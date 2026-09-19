# Putting this online

Two files: `index.html` and `lamp.jpg`. No build step, no dependencies to
install — it's a static page.

## GitHub Pages (free, permanent, you own it)

1. Make a repo on GitHub named exactly **`Ace1687.github.io`**
2. Upload `index.html` and `lamp.jpg` to it (drag them into the web uploader)
3. Settings -> Pages -> Source: `main` branch, `/root`
4. Two minutes later it's live at **https://ace1687.github.io**

From a terminal instead:

```
cd "C:\Users\smart\OneDrive\Documents\Desktop\aziz-site"
git init
git add -A
git commit -m "Personal site"
git branch -M main
git remote add origin https://github.com/Ace1687/Ace1687.github.io.git
git push -u origin main
```

## A custom domain later

Buy something short (abdulaziz.dev, aziz.build). In the registrar point a
CNAME at `ace1687.github.io`, then add the domain under Settings -> Pages.
GitHub issues the HTTPS certificate for free.

## NFC

Any NTAG213 sticker or card works — a pack costs a few dollars.

- **Android:** NFC Tools (free) -> Write -> Add a record -> URL -> paste the
  link -> Write. Hold the tag to the back of the phone.
- **iPhone:** NFC Tools works the same; iPhone 7+ can write tags.
- Lock the tag afterwards only if you're sure of the URL — locking is
  permanent, and an unlocked tag can be rewritten when the address changes.

Point the tag at the **GitHub Pages URL**, not the claude.ai one — it's
shorter, it's yours, and it survives anything happening to this artifact.

## QR

Once it's on a domain, any QR generator will do. Printed on a card it works
where NFC doesn't (most laptops, older phones, anyone who doesn't know to tap).
