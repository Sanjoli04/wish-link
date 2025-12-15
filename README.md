# ✨ WishLink

WishLink is a single-page, serverless web application for creating **personalized, shareable links** that can include festive visual effects and optional payment or donation support. The app is powered by **Supabase** for backend services and integrates **Razorpay** for handling payments.

It is designed to be minimal, easy to deploy, and focused on clean user experience.

---

## 🌟 Features

* **Personalized Links**
  Create unique URLs for sharing wish lists, collecting small payments/donations, or sending special messages.

* **Festive UI**
  Includes a dynamic animated canvas (snow/gift particle effects) to make each link feel special and engaging.

* **Single-File Architecture**
  Entire application (HTML, Tailwind CSS, and JavaScript) lives inside a single `index.html` file for simplicity and easy deployment.

* **Secure Backend**
  Uses **Supabase** for secure, real-time data storage and link management.

* **Payment Integration**
  Integrated with **Razorpay Checkout** to support optional payment or donation flows.

* **Responsive Design**
  Built with **Tailwind CSS** for a modern, mobile-first, and responsive user interface.

---

## 💻 Tech Stack

| Technology                 | Purpose                              |
| -------------------------- | ------------------------------------ |
| HTML5 / Vanilla JavaScript | Core application structure and logic |
| Tailwind CSS               | Styling and responsive UI            |
| Supabase                   | Database and backend services        |
| Razorpay Checkout          | Payment gateway integration          |

---

## 🚀 Setup & Installation

This project is a **single-file application**, so setup is straightforward. You only need to configure your Supabase and Razorpay credentials.

### Prerequisites

* **Supabase Account**
  A Supabase project URL and public anon API key.

* **Razorpay Account**
  A Razorpay **Key ID** for payment integration.

---

### Steps

#### 1. Clone the repository

```bash
git clone https://github.com/Sanjoli04/wish-link.git
cd wish-link
```

#### 2. Configure credentials

Open `index.html` and locate the `App.Constants` section inside the `<script>` tag (around line 100–110). Update the placeholders with your actual credentials:

```javascript
// Inside index.html, within the <script> tags
const App = {
    Constants: {
        SUPABASE_URL: 'YOUR_SUPABASE_PROJECT_URL',
        SUPABASE_ANON_KEY: 'YOUR_SUPABASE_ANON_KEY',
        RAZORPAY_KEY_ID: 'YOUR_RAZORPAY_KEY_ID',
        // ... other constants
    },
    // ... rest of the application logic
};
```

#### 3. Deployment

You can deploy the single `index.html` file using any static hosting provider such as:

* GitHub Pages
* Netlify
* Vercel
* Firebase Hosting

---

## 💡 Usage

### Creating a Link

1. Open the hosted application.
2. Fill in the required details (recipient name, message, amount, etc.).
3. Click the **Create Link** button.
4. A unique URL will be generated.
5. Share the link with your recipient.

---

### Viewing a Link

When someone opens a generated WishLink:

* They see the personalized message along with festive animations.
* If an amount was specified, they are presented with a Razorpay payment option.

---

## 🤝 Contributing

Although WishLink is currently implemented as a single-file project, contributions are welcome.

* Fork the repository
* Make your changes in `index.html`
* Commit your changes

```bash
git commit -m "Fix: Resolved canvas animation bug"
```

* Open a Pull Request

Bug reports and feature suggestions are welcome via GitHub issues.

---

## 📜 License

This project is licensed under the **MIT License**.
(You may add a `LICENSE` file if not already present.)

---

## 📧 Contact

**Sanjoli**
GitHub: [Sanjoli Vashisth](https://github.com/Sanjoli04/)

---
## 🔗 Live Demo

You can view the live deployed version of WishLink here:

👉 [WishLink](https://wishmagic.netlify.app/)

- This demo showcases the UI, link creation flow, festive animations, and Razorpay integration (without performing real transactions).
---

⭐ If you find this project useful or inspiring, consider giving it a star!
