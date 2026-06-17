# Achaar Adda — E-Commerce Website 🫙

> A complete e-commerce website for a real homemade pickle brand from Marihan, Mirzapur, UP.

![Achaar Adda](https://img.shields.io/badge/Status-Live-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🌐 Live Demo
[View Live Website →](https://achaar-adda.netlify.app)

## 📸 Features

- ✅ **Add to Cart** — full cart drawer with quantity controls, offers, dynamic total
- ✅ **WhatsApp Checkout** — cart sends auto-filled order to WhatsApp
- ✅ **FAQ Accordion** — 7 questions with smooth open/close
- ✅ **Product Filtering** — filter by spice level, type, mustard oil
- ✅ **Sort Products** — by price (low/high) and spice level
- ✅ **Wishlist** — heart toggle on each product card
- ✅ **Two Payment Options** — Full online OR 50% now + 50% on delivery
- ✅ **FSSAI Compliance** — food safety registration badge throughout
- ✅ **Responsive Design** — mobile, tablet, desktop
- ✅ **Scroll Animations** — fade-up on scroll via IntersectionObserver
- ✅ **Marquee Offer Bar** — scrolling promotions at top
- ✅ **Toast Notifications** — feedback on cart actions
- ✅ **Village Story Section** — brand origin with Mirzapur identity
- ✅ **Custom SVG Logo** — designed in 3 variants

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 (semantic) |
| Styling | CSS3 (custom properties, flexbox, grid, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Graphics | SVG (custom logo & jar illustrations) |
| Integration | WhatsApp Business API (wa.me deep links) |
| Fonts | Google Fonts (Playfair Display, Inter, Noto Sans Devanagari) |
| Deployment | Netlify / GitHub Pages |

## 📁 Project Structure

```
achaar-adda/
│
├── index.html          # Main website (single-page)
├── README.md           # This file
└── assets/             # (optional) local images if needed
```

## 🚀 How to Run Locally

```bash
# Clone the repo
git clone https://github.com/Preeti529/achaar-adda.git

# Navigate into the folder
cd achaar-adda

# Open in browser
open index.html
# OR just double-click index.html
```

No build tools, no npm, no dependencies — pure HTML/CSS/JS. Just open and it works.

## 🌍 How to Deploy (Netlify — Free)

1. Go to [netlify.com](https://netlify.com) and sign up free
2. Drag and drop the `achaar-adda` folder onto the Netlify dashboard
3. Your site is live in 30 seconds with a free URL

OR connect your GitHub repo and auto-deploy on every push.

## 💡 Key Technical Highlights

### Cart System
Built entirely in vanilla JS with no frameworks:
- Dynamic add/remove/quantity control
- Real-time total calculation
- Offer logic (free shipping at 2 jars, 5% off at ₹500+)
- WhatsApp message auto-generation with full order summary

### Product Architecture
Products defined as a JavaScript data array — easy to add/remove products:
```js
const PRODUCTS = [
  { id:1, name:"Aam ka Achaar", sizes:[{l:"200g",p:180}], spice:3, tags:["tangy"] },
  // add more here...
]
```

### WhatsApp Integration
Orders route directly to WhatsApp with pre-filled messages:
```js
const msg = `🫙 New Order\n${cart.map(i=>`• ${i.name} x${i.qty}`).join('\n')}`;
window.open(`https://wa.me/919336822660?text=${encodeURIComponent(msg)}`);
```

## 👩‍💻 Built By

**Preeti Shukla** — CS Undergraduate, SAREC Mirzapur  
[LinkedIn](https://linkedin.com/in/preeti-shukla) · [GitHub](https://github.com/Preeti529)

---

*This is a real client project — Achaar Adda is a genuine homemade pickle brand from Marihan, Mirzapur, UP.*
