# 🏗️ Buildkite Lorem Ipsum Pipeline - Aditi Abhang

Welcome to the **Lorem Ipsum Generator** pipeline! This Buildkite setup demonstrates how to use Python inside Docker containers to generate sample text using the [`py-lorem`](https://github.com/nubela/py-lorem) package, and annotate results directly in the Buildkite UI 🎉

---

## 🚀 What It Does

This pipeline will:

1. 🐍 Spin up a `python:3.13` Docker container  
2. 📝 Generate a random sentence and paragraph using `loremipsum.sentence` and `loremipsum.paragraph`  
3. 📄 Save the output into files (`sentence.txt` and `paragraph.txt`)  
4. 📢 Annotate the Buildkite UI with the generated content  

---

## 🔧 Pipeline Overview

```yaml
steps:
  - Generate a sentence (max 20 characters)
  - Annotate the sentence in the UI
  - Generate a paragraph (max 100 characters)
  - Annotate the paragraph in the UI
```
Each step uses a python -c one-liner to execute the code and save the output.

---

## 🧪 Sample Output in Buildkite UI

**Paragraph:** Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore

**Sentence:** Lorem ipsum dolor si.

---

## 🐳 Tech Stack
- Buildkite Pipelines 🛠️
- Docker Plugin [`docker-buildkite-plugin`](https://github.com/buildkite-plugins/docker-buildkite-plugin)
- Python 3.13 🐍
- [`py-lorem`](https://github.com/aditiabhang/py-lorem)

---

## 👩‍💻 Author
Made with Passion💫 by [`Aditi Abhang`](https://www.linkedin.com/in/aditi-abhang/)💻

