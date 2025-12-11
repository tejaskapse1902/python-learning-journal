# 📄 Understanding PDFs in Python — PyPDF2 Theory Notes

PyPDF2 is a lightweight and powerful Python library used for working with PDF files.  
It allows developers to read, merge, split, and manipulate PDF documents programmatically.

---

## 🧠 1. What Is PyPDF2?

PyPDF2 is a pure-Python library that provides tools for:
- Reading PDFs (`PdfReader`)
- Writing PDFs (`PdfWriter`)
- Merging multiple PDFs
- Splitting specific pages
- Rotating pages
- Extracting metadata and page content

It is widely used in automation, office workflows, document management systems, and backend services.

---

## 📘 2. How PDF Files Are Structured

A PDF internally contains different components:

### 🔹 **Pages**
Each page is an object and can be extracted, copied, reordered, or edited.

### 🔹 **Metadata**
Information like:
- Title
- Author
- Creation date

### 🔹 **Streams**
Actual text and drawing content inside a PDF.

### 🔹 **Objects**
Building blocks that reference pages, fonts, annotations, etc.

PyPDF2 makes it easy to access and manipulate these components.

---

## 📚 3. How PDFs Are Read Using PyPDF2
```bash
```python
from PyPDF2 import PdfReader

reader = PdfReader("sample.pdf")
pages = reader.pages
```

- PdfReader loads a PDF file.
- reader.pages gives access to individual page objects.

---

## 🔄 4. How PDF Merging Works

- Merging PDFs involves:
- - Opening each PDF
- - Reading all pages
- - Appending pages to a single writer
- - Saving the combined file

- Use cases:
- - Combining notes
- - Merging receipts
- - Joining scanned pages
- - Office document automation

---

## ✂️ 5. How PDF Splitting Works

Splitting extracts specific pages from a PDF and saves them as a new file.

- Workflow:
- - Select page range (e.g., pages 1–3)
- - Copy pages from the original PDF
- - Save them into a new document

- Use cases:
- - Extracting chapters from books
- - Sharing only required pages
- - Cutting large documents into sections

---

## 💡 6. Why PyPDF2 Is Useful

- Lightweight and easy to use
- No external software required
- Works almost anywhere (Windows, Linux, Mac)
- Great for document automation
- Beginner friendly
- Used in office tools, backend services, and workflow automation systems

---

## 📌 Summary

PyPDF2 provides a simple and effective way to work with PDFs in Python.
By understanding how PDF pages, metadata, and objects work, developers can automate tasks like merging and splitting documents with ease.

This theory is the foundation for building:
- PDF Merger Tool
- PDF Splitter Tool
- PDF rotation scripts
- Document processing pipelines

---