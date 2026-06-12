# FitSync Pro 🏋️

> Java desktop application for gym member management with physical condition validation, BMI calculation, and health contraindication checking.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/Swing_GUI-007396?style=flat&logo=java&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit5-25A162?style=flat&logo=junit5&logoColor=white)

---

## Overview

FitSync Pro is a Java SE desktop application built for gym management. The core module handles physical condition validation — it calculates a member's BMI, evaluates health contraindications, and determines whether a member is eligible to train based on their health profile.

Built with **IntelliJ IDEA GUI Designer** using the standard `JFrame`/`JPanel` Swing pattern. Unit tested with JUnit.

---

## Features

- ⚖️ **BMI Calculator** — computes Body Mass Index and classifies result (underweight / normal / overweight / obese)
- 🩺 **Health Contraindication Checker** — validates conditions that may restrict training (cardiac issues, injuries, etc.)
- ✅ **Physical Condition Validation Module** — combines BMI + health flags to approve or restrict gym access
- 🖥️ **Swing GUI** — clean multi-panel desktop interface built with IntelliJ GUI Designer
- 🧪 **JUnit Test Suite** — unit tests covering validation logic and edge cases

---

## Tech Stack

| Component | Technology |
|---|---|
| Language | Java SE 17+ |
| GUI | Swing (IntelliJ GUI Designer) |
| Testing | JUnit 5 |
| IDE | IntelliJ IDEA |

---

## Project Structure

```
FitSyncPro/
├── src/
│   ├── model/
│   │   ├── Member.java
│   │   ├── HealthProfile.java
│   │   └── PhysicalCondition.java
│   ├── service/
│   │   ├── BMICalculator.java
│   │   └── ContraindicationChecker.java
│   └── ui/
│       ├── MainWindow.java
│       └── MainWindow.form
└── test/
    ├── BMICalculatorTest.java
    └── ContraindicationCheckerTest.java
```

---

## How to Run

```bash
git clone https://github.com/JoseIgnacio-Puma08/fitsync-pro.git
# Open in IntelliJ IDEA and run MainWindow.java
```

> Requires Java 17+ and IntelliJ IDEA to compile `.form` GUI files.

---

## BMI Classification Logic

| BMI Range | Classification |
|---|---|
| < 18.5 | Underweight |
| 18.5 – 24.9 | Normal |
| 25.0 – 29.9 | Overweight |
| ≥ 30.0 | Obese |

---

## Author

**José Ignacio Pumagualli Silva** — Software Engineering @ UDLA, Quito, Ecuador
📧 pumaguallipro@gmail.com | [Portfolio](https://joselgnacio-puma08.github.io)
