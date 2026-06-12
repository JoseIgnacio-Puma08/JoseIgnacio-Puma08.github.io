# Digital Asset Management System 💎

> Java application for managing digital assets with an OOP inheritance architecture, ArrayList-based persistence, and a JUnit test suite.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit5-25A162?style=flat&logo=junit5&logoColor=white)
![OOP](https://img.shields.io/badge/SOLID-Principles-blue?style=flat)

---

## Overview

A Java SE project that models a digital asset management system — think images, videos, documents, and audio files — using a clean OOP class hierarchy. The focus is on applying SOLID principles, proper use of inheritance and polymorphism, and writing reliable unit tests.

---

## Features

- 🗂️ **Asset type hierarchy** — abstract `DigitalAsset` base class with specialized subclasses (ImageAsset, VideoAsset, DocumentAsset, AudioAsset)
- ➕ **Full CRUD** — add, list, search, update, and delete assets via ArrayList
- 🔍 **Binary search** — efficient search by asset ID or name
- 🧪 **JUnit test suite** — covers core business logic, edge cases, and null handling
- 📐 **SOLID principles** — single responsibility, open/closed, and interface segregation applied throughout

---

## Tech Stack

| Component | Technology |
|---|---|
| Language | Java SE 17+ |
| Testing | JUnit 5 |
| Data | ArrayList |
| IDE | IntelliJ IDEA |

---

## Class Structure

```
DigitalAsset (abstract)
├── ImageAsset    (resolution, format)
├── VideoAsset    (duration, codec)
├── AudioAsset    (bitrate, format)
└── DocumentAsset (pageCount, type)

AssetManager
├── assets: ArrayList<DigitalAsset>
├── add(asset)
├── remove(id)
├── findById(id)
└── listByType(type)
```

---

## Running Tests

```bash
git clone https://github.com/JoseIgnacio-Puma08/digital-asset-management.git
# Open in IntelliJ IDEA
# Right-click test folder → Run All Tests
```

---

## Author

**José Ignacio Pumagualli Silva** — Software Engineering @ UDLA, Quito, Ecuador
📧 pumaguallipro@gmail.com | [Portfolio](https://joselgnacio-puma08.github.io)
