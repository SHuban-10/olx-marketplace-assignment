# 🛒 OLX Marketplace Web Application
> **Assessment Project for Web Developer Internship Role**  
> Built with **Plain HTML5, CSS3, and Modern JavaScript (Vanilla ES6+)** — zero external dependencies, 100% responsive, and ready to run immediately in any browser.

---

## 📌 Project Overview
This project is an **OLX-style marketplace web application** where users can register, browse, and post ads for both **physical products** and **local services**. It implements all features requested in the assignment assessment sheet with an authentic OLX India design aesthetic.

---

## ✅ Assessment Requirements Compliance Checklist

| Requirement | Assignment Spec | Implementation File & Details | Status |
| :--- | :--- | :--- | :---: |
| **1. User Registration** | User can register and log in | [`register.html`](register.html) & [`js/auth.js`](js/auth.js) — Full registration form (Name, Email, Phone, City, Password), login tab, active session in `localStorage`, and logout. | **Done** |
| **2. Add products/services** | Form with 10 exact data fields | [`post-ad.html`](post-ad.html) with all 10 fields explicitly mapped & validated. | **Done** |
| *i. product/service* | Field 1 | Radio card toggle: `📦 Product` vs `🛠️ Service` | **Done** |
| *ii. Name* | Field 2 | Title / Name text input with length validation | **Done** |
| *iii. Detail* | Field 3 | Multi-line textarea description | **Done** |
| *iv. Category* | Field 4 | Dropdown with Mobiles, Vehicles, Electronics, Real Estate, Home Services, etc. | **Done** |
| *v. Subcategory* | Field 5 | **Cascading dynamic dropdown** that updates based on the selected Category | **Done** |
| *vi. Country* | Field 6 | Country selector (defaults to India) | **Done** |
| *vii. State* | Field 7 | State selector (Maharashtra, Delhi NCR, Karnataka, Telangana, etc.) | **Done** |
| *viii. City* | Field 8 | **Cascading City dropdown** based on chosen State (Mumbai, Delhi, Bengaluru, etc.) | **Done** |
| *ix. Area* | Field 9 | Area / locality input with autocomplete datalist suggestions | **Done** |
| *x. Price* | Field 10 | Currency input formatted with ₹ Indian Rupee | **Done** |
| **3. Show on frontend** | Immediately visible after posting | Saved into `localStorage` database, redirects to [`listing.html`](listing.html) with success toast, and immediately appears in all feeds. | **Done** |
| **4.a Category Page** | Dedicated Category page & listing | [`category.html`](category.html) — Category pills, subcategory filtering, item counts, search. | **Done** |
| **4.b City Wise Listing** | City wise listing | [`city.html`](city.html) — Popular cities grid, area-based locality filtering, ad counts. | **Done** |
| **4.c City + Category Wise** | Combined multi-filter | [`explore.html`](explore.html) — Simultaneous dual filtering by City + Category + Type + Sort + Keyword. | **Done** |
| **4.d Listing Page** | Single listing detail page | [`listing.html`](listing.html) — Image preview, 10-field specification breakdown, price card, seller profile, WhatsApp & Call buttons. | **Done** |

---

## 🚀 How to Run the Project

Because this project is built in **Pure Plain HTML/CSS/JS**, there is **no build step, no npm install, and no backend server needed**!

### Option 1: Direct Browser Launch (Simplest)
1. Navigate to the project directory:
   ```
   C:\Users\Shuban\.gemini\antigravity\scratch\olx-marketplace
   ```
2. Double-click on `index.html` to open it directly in Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari.

### Option 2: Using VS Code Live Server
1. Open the `olx-marketplace` folder in VS Code.
2. Right-click `index.html` and click **"Open with Live Server"**.

---

## 🔑 Pre-Configured Demo Credentials for Evaluator

To make reviewing effortless, a sample user account is pre-registered:
- **Email**: `demo@olx.com`
- **Password**: `password123`
*(There is also a convenient **"Quick Fill"** button on the `register.html` page).*

Additionally, the marketplace comes pre-seeded with **8+ realistic demo listings** (Apple iPhone 14 Pro, Royal Enfield Classic 350, AC Jet Cleaning Service, 2BHK Apartment, Dell XPS 15, Web App Development Service) with high-definition photos across Mumbai, Delhi, Bengaluru, and Hyderabad.

---

## 📂 Project Directory Structure

```text
olx-marketplace/
├── index.html          # Main Home page with search, categories, and fresh listings
├── register.html       # Feature 1: User Registration & Login
├── post-ad.html        # Feature 2 & 3: Add Product/Service Form (All 10 Fields)
├── category.html       # Feature 4.a: Category Page & Category-wise listings
├── city.html           # Feature 4.b: City Wise Listing
├── explore.html        # Feature 4.c: City + Category Wise combined filtering
├── listing.html        # Feature 4.d: Detailed single listing page
├── my-listings.html    # Bonus: Seller's personal listing dashboard
├── css/
│   └── styles.css      # Custom responsive stylesheet (OLX Teal & Navy theme)
├── js/
│   ├── data.js         # Initial mock database, categories, locations & LocalStorage DB
│   ├── auth.js         # User registration, authentication & session management
│   └── navbar.js       # Global header, search bar, city dropdown, and footer
└── README.md           # Project documentation and evaluation guide
```

---

## 🎨 Key Features & Polish
- **Authentic OLX Design**: Styled with OLX signature colors (`#002f34`, `#00a49f`, `#ffce32`), card hover animations, badge tags, and mobile responsive layout.
- **Cascading Dropdowns**: Category dynamically updates Subcategories; State dynamically updates Cities and sample Areas.
- **Image Support**: Upload custom photos via file picker (converted to Base64) or input an image URL with live preview.
- **Contact & WhatsApp Integration**: "Call Seller" popup modal and direct "Chat on WhatsApp" links with pre-filled inquiries.
- **Persistent Storage**: All changes (new users, newly published ads, deletions) persist cleanly in browser `localStorage`.
