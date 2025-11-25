<div align="center">

# 🔍 Text Diff Checker

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/languages-AR%20%7C%20EN-orange.svg" alt="Languages">
  <img src="https://img.shields.io/badge/responsive-yes-brightgreen.svg" alt="Responsive">
</p>

<p align="center">
  <strong>A professional tool for comparing texts and discovering differences easily and effectively</strong>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-installation">Installation</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-screenshots">Screenshots</a> •
  <a href="#-contributing">Contributing</a>
</p>

---

</div>

## 📋 Overview

**Text Diff Checker** is an advanced web tool for comparing texts and identifying differences with high accuracy. The tool supports comparing two or four texts simultaneously, with an easy-to-use interface that supports both Arabic and English languages with automatic text direction detection.

### 🎯 Project Goals

- Provide an easy and fast tool for text comparison
- Full support for Arabic language with automatic direction detection
- Display differences in a clear visual way
- Provide accurate statistics about changes

---

## ✨ Features

### 🔄 Comparison Modes
| Mode | Description |
|------|-------------|
| **Compare 2 Texts** | Compare original text with modified text |
| **Compare 4 Texts** | Multiple comparison between four different texts |

### 🎨 Difference Highlighting
| Color | Meaning |
|-------|---------|
| 🟢 **Green** | Added text (exists only in new text) |
| 🔴 **Red** | Removed text (exists only in original text) |
| 🟡 **Yellow** | Changed text |

### 📊 Statistics
- ✅ Total word count
- ✅ Added words count
- ✅ Removed words count
- ✅ Similarity percentage

### 🖥️ View Modes
- **Combined View**: Display all changes in one box
- **Split View**: Display old and new text side by side

### 🌐 Language Support
- ✅ Automatic text direction detection (RTL/LTR)
- ✅ Full Arabic language support
- ✅ English and Latin languages support
- ✅ Example texts in Arabic and English

### 📱 Design
- ✅ Responsive design for all devices
- ✅ Modern and attractive UI
- ✅ Easy to use

---

## 🚀 Installation

### Method 1: Direct Use

```bash
# Clone the repository
git clone https://gitlab.com/username/text-diff-checker.git

# Navigate to project folder
cd text-diff-checker

# Open in browser
open index.html
# Or on Linux
xdg-open index.html
# Or on Windows
start index.html
```

### Method 2: Using Local Server

```bash
# Using Python 3
python -m http.server 8000

# Or using Node.js
npx serve .

# Or using PHP
php -S localhost:8000
```

Then open browser at: `http://localhost:8000`

### Method 3: Docker

```bash
# Build image
docker build -t text-diff-checker .

# Run container
docker run -p 8080:80 text-diff-checker
```

---

## 📖 Usage

### Comparing Two Texts

1. Select **"Compare 2 Texts"** mode
2. Enter the first text (original) in the first field
3. Enter the second text (modified) in the second field
4. Click **"🔎 Compare Texts"** button
5. Choose your preferred view mode (combined or split)

### Comparing 4 Texts

1. Select **"Compare 4 Texts"** mode
2. Enter texts in the four fields
3. Click **"🔎 Compare Texts"** button
4. All possible comparisons will be displayed

### Using Examples

- Click **"📝 Arabic Example"** to load sample Arabic texts
- Click **"📝 English Example"** to load sample English texts

---

## 🛠️ Technologies Used

| Technology | Usage |
|------------|-------|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) | Page structure |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) | Styling and design |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) | Logic and interactivity |
| ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white) | CSS framework |

---

## 🔧 Algorithm Used

The project uses **Longest Common Subsequence (LCS)** algorithm for text comparison:

```javascript
function lcs(arr1, arr2) {
    const dp = Array(m + 1).fill(null)
        .map(() => Array(n + 1).fill(0));
    
    for (let i = 1; i <= m; i++) {
        for (let j = 1; j <= n; j++) {
            if (arr1[i-1] === arr2[j-1]) {
                dp[i][j] = dp[i-1][j-1] + 1;
            } else {
                dp[i][j] = Math.max(dp[i-1][j], dp[i][j-1]);
            }
        }
    }
    
    return backtrack(dp, arr1, arr2);
}
```

---

## 🗺️ Roadmap

- [x] Compare two texts
- [x] Compare 4 texts
- [x] Split view
- [x] Automatic text direction detection
- [x] Comparison statistics
- [ ] Export results to PDF
- [ ] Export results to Word
- [ ] Direct file comparison
- [ ] Save comparisons history
- [ ] API for programmatic use
- [ ] Support more languages
- [ ] Dark Mode

---

## 🤝 Contributing

We welcome contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before getting started.

### Contribution Steps

1. **Fork** the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit changes (`git commit -m 'Add amazing feature'`)
5. Push to branch (`git push origin feature/amazing-feature`)
6. Open a **Merge Request**

---

## 📄 License

This project is licensed under **MIT License** - see [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

<div align="center">

**Developer Name**

[![GitLab](https://img.shields.io/badge/GitLab-330F63?style=for-the-badge&logo=gitlab&logoColor=white)](https://gitlab.com/username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/username)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/username)

</div>

---

<div align="center">

**⭐ If you like this project, don't forget to give it a star! ⭐**

</div>
