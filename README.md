# 🌐 PureArt Wix Redirect

This repository hosts a simple redirect page designed to forward traffic from a custom domain to a Wix-hosted website using GitHub Pages.  
It provides a clean and secure solution for enabling HTTPS on a Wix site without a paid SSL certificate.

---

## 🔧 Purpose

Wix only supports HTTPS for domains fully managed through their platform.  
To avoid purchasing SSL certificates or transferring DNS, this project acts as a smart middle-layer:

- **Custom domain**: `www.pure-art.co`  
- **Redirect target**: [https://deen803.wixsite.com/home](https://deen803.wixsite.com/home)  
- **Host**: GitHub Pages (secure, fast, and free)

---

## 🚀 Live Site

👉 Visit the secure version:  
**[https://www.pure-art.co](https://www.pure-art.co)**

---

## 🧠 How It Works

1. Domain DNS is configured via **Namecheap** to point to GitHub Pages:
   - CNAME for `www` → `norman-deen.github.io`
   - A records for root domain → GitHub IPs
2. GitHub Pages serves a minimal `index.html` with:
   - JavaScript redirect (secure and modern)
   - Fallback HTML link (for older browsers)
3. GitHub provides a **free HTTPS certificate**, solving the "insecure site" warning.

---

## 💡 Use Cases

- Freelancers and designers using Wix or other platforms without HTTPS for custom domains
- Quick redirect setup without server costs
- Branding and SEO improvements by keeping your own domain active and secure

---

## 📁 Files in this Repository

| File         | Purpose                                 |
|--------------|------------------------------------------|
| `index.html` | Performs instant redirect to Wix site    |
| `CNAME`      | Declares the custom domain               |
| `.nojekyll`  | Disables Jekyll processing on GitHub     |

---

## 📌 Notes

- The redirect target can be changed anytime by modifying `index.html`.
- Ensure your DNS propagation is complete before enforcing HTTPS.
- This approach avoids Wix SSL limitations without violating their policies.

---

## ✍️ Author

**Nour Altinawi**  
Full-Stack & 3D Front-End Developer  
🔗 [LinkedIn](https://www.linkedin.com/in/nour-tinawi) | 💼 [Portfolio](https://www.pure-art.co)

---
