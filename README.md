# Madanur Consumer Information Web App

A lightweight, mobile-friendly web application to search consumer electricity details and transformer service numbers for **Madanur** area.

---

## 🚀 Features
- **Consumer Search** by Short Service Number  
- **Transformer Lookup** by Transformer Number (e.g., TR10)  
- **Local Search History** (last 5 searches)  
- **Responsive Design** – works on phones, tablets, and desktops  
- **GitHub Pages Ready** – host for free without a server  

---

## 📦 Usage
1. Clone or download this repo.
2. Open `index.html` in any browser – no build step required.  
3. (Optional) Host on GitHub Pages:
   - Fork this repo  
   - Go to **Settings → Pages**  
   - Select source: **Deploy from a branch → main → / (root)**  
   - Save and visit `https://yourusername.github.io/repo-name`

---

## 🔧 Customization
Replace the **mock data objects** (`mockConsumerDB`, `mockTransformerDB`) in `index.html` with real API calls or Google Apps Script URLs:

```javascript
// Example: connect to your live Google Apps Script
fetch('https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec?ssNo=' + ssNo)
  .then(r =&gt; r.json())
  .then(showResult);
