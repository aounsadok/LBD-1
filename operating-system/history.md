# History of Operating Systems
*Operating Systems 1 — LBDAD1, FSM. Instructor: Nizar Kerkeni*

## The Big Picture

The evolution of Operating Systems tracks the evolution of computers themselves:

- **1950s–1960s: Simple computers** — direct interaction between the user (operator) and the machine. **No Operating System needed.**
- **Later, "complex" computers** — interaction became difficult to manage directly. This created the **need for an Operating System** to sit between user and hardware.

---

## Timeline

### 1969 — UNIX is born
- Created by **Ken Thompson**.
- Originally written in **Assembly language**.
- **Multitasking** & **Multi-user** — a major leap from what came before.

### 1972 — The C language
- **Dennis Ritchie** creates **C**, a high-level programming language.

### 1973 — UNIX rewritten in C
- UNIX rewritten as **90% C + 10% Assembly** — this is what made it **portable** (able to run on different hardware without a full rewrite).
- Spawned many **UNIX variants**: HP-UX, IBM-AIX, Unix BSD, and others.

### 1981 — MS-DOS
- Microsoft releases the first version of **MS-DOS** (Microsoft Disk Operating System).
- Built for **IBM-PC and compatibles**.
- **Single-tasking & Single-user** — one program, one user, at a time.

### 1983 — GNU Project
- **Richard Stallman** launches **GNU** ("GNU's Not Unix" — a recursive acronym).
- Goal: a completely **Free/Libre** operating system.

**The Four Freedoms of Free Software:**
| # | Freedom |
|---|---|
| 0 | **Run** the program as you wish, for any purpose |
| 1 | **Study** how it works and **change it** to do what you want |
| 2 | **Redistribute** copies to help others |
| 3 | **Distribute** your modified versions to others |

*(Reference: [gnu.org/philosophy/free-sw.html](https://www.gnu.org/philosophy/free-sw.html))*

### 1984 — Macintosh
- **Apple** releases the Macintosh with **System** software.
- Introduces a **Graphical User Interface (GUI)** to the mainstream.
- **Multitasking & Single-user**.

### 1985 — Windows 1.0
- Microsoft releases the **first version of Windows** — a GUI layered **on top of MS-DOS** (not yet a standalone OS).

### 1988 — POSIX
- **POSIX** (Portable Operating System Interface) becomes the standard specification for UNIX-like systems, aiming for compatibility across variants.

### 1991 — Linux
- **Linus Torvalds** releases the **Linux kernel** for the **PC/i386 architecture**.
- **Multitasking & Single-user**.
- Released under the **GNU-GPL** (GNU General Public License) — free software.

> 💡 Note: Linux is a *kernel*, not a full OS by itself — it needs to be paired with tools (often from the GNU project) to form a complete system, hence the term "GNU/Linux."

### 1992 — First GNU/Linux distributions
- Early distributions combining the Linux kernel + GNU programs + a GUI: **Debian** and **Slackware** among the first.
- A GNU/Linux **distribution** = Linux kernel + GNU project programs + GUI + more.

### 1995 — Windows 95
- **Multitasking & Single-user.**

### 1995 — Java
- **Sun Microsystems** releases **Java**, an **object-oriented** programming language.

### 1997 — Mac OS
- Apple's system software is renamed **Mac OS**.

### 2004 — Ubuntu
- First version released: **Ubuntu 4.10**.
- Built on **Debian**, with a focus on being: **Simple, Intuitive, Secure.**

### 2007 — iOS
- Apple releases **iOS** for **mobile devices**.

### 2008 — Android
- **Google** releases **Android**:
  - Built on the **Linux kernel**.
  - GUI/apps originally written in **Java**.
  - Since 2017, **Kotlin** has become Google's preferred language for Android development — Java is still supported, but Kotlin is now favored for new app development.

---

## Quick Reference Table

| Year | Milestone | Key Player |
|---|---|---|
| 1969 | UNIX | Ken Thompson |
| 1972 | C language | Dennis Ritchie |
| 1973 | UNIX rewritten in C (portable) | Ritchie & Thompson |
| 1981 | MS-DOS | Microsoft |
| 1983 | GNU Project | Richard Stallman |
| 1984 | Macintosh (GUI) | Apple |
| 1985 | Windows 1.0 | Microsoft |
| 1988 | POSIX standard | — |
| 1991 | Linux kernel | Linus Torvalds |
| 1992 | First GNU/Linux distros | Debian, Slackware |
| 1995 | Windows 95 / Java | Microsoft / Sun Microsystems |
| 1997 | Mac OS | Apple |
| 2004 | Ubuntu | Canonical |
| 2007 | iOS | Apple |
| 2008 | Android | Google |

---
*Course materials: [kerkeni.tn/supports/se1](https://kerkeni.tn/supports/se1)*
*Notes cleaned up and organized by Claude, from slides prepared by Nizar Kerkeni (FSM).*
