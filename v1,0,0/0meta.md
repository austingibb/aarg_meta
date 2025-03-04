# aarg.v1,0,0 Meta File

## Overview

This document establishes the **structural and versioning framework** for aarg.v1,0,0. The **aarg system** is a **hierarchically organized, version-controlled model** designed to facilitate the structured development of inventions, prototypes, projects, goals, research, and supporting resources. This system ensures **scalability, maintainability, and clarity** across all structured components and how they work together.

## Versioning System

- **Strict versioning format**: `v<major>,<minor>,<patch>`.
- **All objects adhere to a three-digit versioning convention** (e.g., `v1,0,0`).
- **Folders and domains are functionally identical**; every object follows a **consistent URI-based structure**.
- **Each versioned object contains a `meta.md` file**, defining its structure, scope, and intended use.

## Core Structural Framework

```
aarg.v1,0,0/
│-- meta.md  (this document, defining the aarg architecture)
│-- goals.v1,0,0/  (Hierarchical goal-setting system)
│-- inventions.v1,0,0/  (Blueprint-driven invention management)
│-- prototypes.v1,0,0/  (Early-stage experimental iterations)
│-- projects.v1,0,0/  (Execution-focused project tracking)
│-- resources.v1,0,0/  (Research documentation, references, and supporting assets)
```

## Dependency Structure
The **aarg system** follows a strict dependency hierarchy to maintain logical consistency:
- **Goals may reference inventions, but inventions may only reference resources.**
- **Prototypes follow the same rule as inventions.**

This results in the following dependency flow:
```
goals → inventions → resources/*
prototypes → resources/*
```
Goals define **high-level objectives** that guide the development of inventions. Inventions are built using information and assets from the **resources system**, ensuring a well-structured flow of knowledge without circular dependencies.

### **Goals System** (`aarg.goals.v1,0,0`)

The **goals subsystem** organizes objectives into a **nested hierarchical model**, facilitating long-term strategic planning and incremental execution:

- **Big Goals** → Foundational, high-impact objectives.
- **Medium Goals** → Structural milestones contributing to the realization of big goals.
- **Small Goals** → Executable tasks with direct, measurable outcomes.

### **Inventions System** (`aarg.inventions.v1,0,0`)

- **Graduated Inventions (`.meta.md` files)** → Fully structured, versioned, and formally defined systems ready for deployment or further iteration.

### **Prototypes System** (`aarg.prototypes.v1,0,0`)

- **Prototypes (`.boox` files)** → Early-stage experimental iterations, lacking formalized versioning.

### **Projects System** (`aarg.projects.v1,0,0`)

- **Execution-centric framework** designed to manage real-world implementations.
- **Milestone-oriented structure**, ensuring quantifiable deliverables.
- **Interoperability with goals**, allowing for cross-referencing and dependency tracking.

### **Resources System** (`aarg.resources.v1,0,0`)

- **Research** → Methodologically rigorous, hypothesis-driven studies.
- **References** → Aggregated external knowledge and documentation.
- **Assets** → Tangible materials supporting implementation and execution.

## Purpose of This System

- **Establishes a unified architecture** for structured work across multiple domains.
- **Enforces semantic clarity and maintainability** through versioning and documentation.
- **Balances hierarchical flexibility with historical integrity**, ensuring structured evolution over time.
- **Provides a scalable framework** for organizing complex, multi-disciplinary projects.

