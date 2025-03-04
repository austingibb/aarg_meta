# aarg Prototypes Meta File

## Overview

This document defines the **classification system for prototypes** within aarg. Prototypes are early-stage experimental inventions that have not yet graduated to full versioned inventions. Instead of version numbers, prototypes are categorized using a **quality enum system** to define their expected level of refinement.

## Prototype Classification System (Quality Enums)

Each prototype is tagged in its filename with an enum that describes its intended **quality level**:

### **Quality Levels**

- **`-WC`** (World Class) → Designed to impress the smartest minds on Earth. Requires exceptional polish, performance, and documentation.
- **`-CC`** (Corporate Class) → Ready for enterprise-level deployment, scalable and well-structured.
- **`-MC`** (Medium Class) → Functional for mid-sized operations, reliable but not cutting-edge.
- **`-SC`** (Small Class) → Works well for small teams or startups, practical but with some rough edges.
- **`-GC`** (Garage Class) → A rough proof-of-concept, meant for internal experimentation only.

## File Naming Convention

Each prototype must use the following format:

```
[invention_name]-[quality_enum].boox
```

### **Example Filenames:**

```
QuantumCompute-WC.boox
AIChatbot-CC.boox
InventorySystem-MC.boox
LocalBakeryPOS-SC.boox
3DPrintedTool-GC.boox
```

## Transitioning from Prototype to Invention

Once a prototype is **refined enough for structured development**, it **graduates** to a full invention. At this stage:

1. The prototype **loses its quality enum**.
2. It moves into a **versioned URI-based structure**, maintaining a consistent naming convention.
3. A structured specification (`meta.md`) is created to define its development path.

**Example transition:**

```
Before: AIChatbot-GC.boox (Garage Class Prototype)
After: aarg.inventions.v1,0,0.AIChatbot.v1,0,0.meta.md
```

## Versioning System for Inventions

- **Versioning follows a strict format**: `v<major>,<minor>,<patch>`.
- **All inventions must have three version digits** (e.g., `v1,0,0`).
- **There is no distinction between folders and domains**; all objects follow the exact URI format.
- **Each versioned object must include a `meta.md`** file that describes its structure and purpose.

## Purpose of This System

- **Maintains flexibility in the prototype phase** without rigid versioning.
- **Clearly defines expected quality levels** so effort matches the intended audience.
- **Provides an easy way to filter and sort prototypes** based on their level of refinement.
- **Ensures a structured graduation process** when an idea is ready for full development.
- **Creates a uniform, predictable versioning structure** across all aarg components.


