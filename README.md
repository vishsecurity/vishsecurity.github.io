
# 🛡️ Vishal Chaudhary | Technical GRC & Security Architecture Portfolio

Welcome to the source repository for my personal portfolio website! This project showcases my dual-domain expertise in **Technical GRC** (Governance, Risk, and Compliance) and **Security Architecture & Operations**, alongside my content creation on YouTube and ongoing technical articles.

---

## 🌐 Live Preview

👉 **[Explore the Live Website](https://vishsecurity.github.io/)**

---

## 💡 Key Highlights & Features

* 📱 **Apple-Inspired Design System:** Responsive, clean layout built with modern glassmorphism aesthetic.
* 🌓 **Seamless Light/Dark Theme:** Instant theme toggling for an optimal reading experience.
* ⌨️ **Dynamic Interactive UI:** Custom typing animation header and interactive navigation.
* 🎬 **Community Knowledge Base:** Integrated section highlighting my YouTube channel, **GovernanceGuard**.
* 📝 **Blog Integration:** Lightweight JS-driven engine to dynamically surface technical articles and insights.
* 💼 **Comprehensive Experience & Credentials:** Full display of multi-region audit advisory, commercial contract leadership, certifications, and educational background.

---

## 📂 Project Structure


```

.
├── index.html         # Complete website (markup, embedded styling & dynamic logic)
└── README.md          # Project documentation

```

---

## 🛠️ Tech Stack

* **HTML5:** Semantic structural layout
* **CSS3:** Custom CSS variables, flexbox, grid, and glassmorphism styling
* **Vanilla JavaScript:** DOM manipulation, theme toggling, and dynamic content rendering

---

## 🚀 Local Setup & Development

1. **Clone the Repository:**

   ```bash
   git clone [https://github.com/vishsecurity/vishsecurity.github.io.git](https://github.com/vishsecurity/vishsecurity.github.io.git)
   cd vishsecurity.github.io

```

2. **Run Locally:**
You can open `index.html` directly in your browser or serve it locally:
```bash
# Using Python
python -m http.server 8000

```


3. **View Site:**
Navigate to `http://localhost:8000` in your web browser.

---

## ✍️ Adding & Managing Blog Posts

You can add new technical articles to the site in two ways:

### Method 1: Inline Array (Fastest)

Open `index.html`, locate the `blogPosts` array inside the `<script>` tag, and add a new entry:

```javascript
const blogPosts = [
    {
        title: "Your New Post Title",
        tag: "PCI DSS / Cloud / AI",
        date: "Sep 2026",
        summary: "Brief overview of what the article covers.",
        link: "[https://your-article-or-video-link.com](https://your-article-or-video-link.com)"
    }
];

```

### Method 2: External Markdown (`marked.js`)

1. Add `<script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>` to your `<head>`.
2. Place `.md` files in a `/posts` directory.
3. Fetch and parse them using `marked.parse()` inside your script.

---

## ⚙️ Quick Customization Guide

* **Typing Animation Header:** Modify the `headerText` constant inside the `<script>` tag:
```javascript
const headerText = "Vishal Chaudhary";

```


* **Theme Styling:** Adjust color values in `:root` and `[data-theme="light"]` inside the `<style>` block to customize the design palette.

---

## 👋 Let's Connect!

* **Email:** [vishchaudhary20021994@gmail.com](https://www.google.com/search?q=mailto%3Avishchaudhary20021994%40gmail.com)
* **LinkedIn:** [Vishal Chaudhary](https://www.linkedin.com/in/vishal-chaudhary-224701116/)
* **YouTube:** [GovernanceGuard](https://www.youtube.com/@GovernanceGuard)
* **GitHub:** [@vishsecurity](https://github.com/vishsecurity)

---

## 📜 License

Distributed under the [MIT License](https://www.google.com/search?q=LICENSE).

```
