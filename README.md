# 💻 Vishal Chaudhary - Cybersecurity Portfolio Website

A sleek and responsive personal portfolio website built with HTML, CSS, and JavaScript to showcase the cybersecurity experience, certifications, projects, and blog of **Vishal Chaudhary**, a dedicated Cybersecurity Specialist and ISO Consultant.

---

## 🌐 Live Preview

👉 [**View Website**](#)   *(Add your GitHub Pages or hosting link here)*

---

## 📌 Features

* 🚀 Modern, responsive, and mobile-friendly UI
* 🌙 Light/Dark mode toggle
* ✍️ Typing effect for intro header
* ⏳ Preloader spinner on page load
* 📄 Dynamic blog post loader (Markdown support via `marked.js`)
* 🔐 Cybersecurity project domains listed
* 🏢 Work experience & education
* 🧾 Certifications in grid layout
* 🗣️ Professional recommendation section

---

## 🗂️ Folder Structure

```
├── index.html         # Main website
├── blogs/             # Folder to store markdown blog posts
│   ├── first-post.md
│   └── another-post.md
├── assets/            # (Optional) Images, icons, etc.
└── README.md          # This file
```

---

## 📦 Tech Stack

* **HTML5**
* **CSS3**
* **Vanilla JavaScript**
* **[marked.js](https://github.com/markedjs/marked)** for Markdown blog rendering
* **Google Fonts (Inter)**

---

## 📚 Blog System

The blog section dynamically loads Markdown files stored in the `/blogs` directory using JavaScript and renders them using the `marked` library.

📌 **To add a new blog:**

1. Create a new `.md` file in the `blogs/` folder.
2. Add it to the `blogPosts` array in the JavaScript:

```js
const blogPosts = [
  { title: "My First Blog Post", filename: "first-post.md" },
  { title: "Another Day, Another Post", filename: "another-post.md" },
  { title: "New Blog", filename: "new-blog.md" }, // Add here
];
```

---

## ⚙️ Setup & Usage

1. **Clone this repository:**

   ```bash
   git clone https://github.com/yourusername/yourrepo.git
   cd yourrepo
   ```

2. **(Optional) Serve locally for development:**

   You can use VS Code Live Server or Python's built-in server:

   ```bash
   python -m http.server
   ```

3. **Open in browser:**

   Open `http://localhost:8000` or simply double-click the `index.html`.

---

## ✨ Customization Tips

* Change the header typing text by editing:

  ```js
  const headerText = "Vishal Chaudhary";
  ```

* To update your roles/subtitle: edit the `<p>` tag below `<h1>` in the header.

* Modify blog content in Markdown using standard syntax.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ About Me

I’m **Vishal Chaudhary**, a cybersecurity specialist with a proven track record in ISO implementations, risk assessments, and compliance frameworks (ISO 27001, PCI DSS, SEBI CSF, etc.).

🔗 [LinkedIn](#) • [GitHub](#) • [Twitter](#)

---

## 🙏 Acknowledgements

* [marked.js](https://github.com/markedjs/marked) for Markdown rendering
* Google Fonts for beautiful typography

