# Knights Mission Manager ⚔️

> Java desktop application for managing missions assigned to Knights of the Zodiac characters, featuring a full Swing GUI and OOP-based architecture.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/Swing_GUI-007396?style=flat&logo=java&logoColor=white)
![OOP](https://img.shields.io/badge/OOP-Inheritance-blue?style=flat)

---

## Overview

A collaborative Java desktop project that implements a mission management system for Knights of the Zodiac characters. The system demonstrates core OOP principles including inheritance hierarchies, polymorphism, and encapsulation, all wrapped in a multi-panel Swing GUI.

Developed as a group project at UDLA with full version control via GitHub.

---

## Features

- 🧬 **Inheritance hierarchy** — Knight base class with specialized subclasses per character type
- 📋 **Mission management** — assign, list, complete, and remove missions per knight
- 🖥️ **Multi-panel Swing GUI** — tabbed interface for knights roster and mission board
- 📦 **ArrayList-based storage** — in-memory data management with full CRUD
- 🔍 **Search functionality** — find knights and missions by name or status

---

## Tech Stack

| Component | Technology |
|---|---|
| Language | Java SE 17+ |
| GUI | Swing (JTabbedPane, JTable, JPanel) |
| Data | ArrayList collections |
| IDE | IntelliJ IDEA |

---

## Class Hierarchy

```
Knight (abstract)
├── GoldKnight
├── SilverKnight
└── BronzeKnight

Mission
├── title: String
├── difficulty: int
├── status: MissionStatus (PENDING / IN_PROGRESS / COMPLETED)
└── assignedKnight: Knight
```

---

## How to Run

```bash
git clone https://github.com/JoseIgnacio-Puma08/ProyectoProgramacionJose-Pumagualli.git
# Open in IntelliJ IDEA and run the main Ventana.java class
```

---

## Team

Built collaboratively by students of Programación III at UDLA.

---

## Author

**José Ignacio Pumagualli Silva** — Software Engineering @ UDLA, Quito, Ecuador
📧 pumaguallipro@gmail.com | [Portfolio](https://joselgnacio-puma08.github.io)
