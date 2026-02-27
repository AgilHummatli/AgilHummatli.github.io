---
layout: default
title: My Path to Learning C (and Understanding Computers)
---

# My Path to Learning C (and Understanding Computers)

[← Back to Home](../)

---

Most people start learning C with syntax. They memorize printf, pointers, malloc. But they do not understand what is actually happening inside the machine.

I took a different approach. First understand the computer, then learn the language.

---

## Phase 1: Understand How Computers Actually Work

### 1. Read "Code: The Hidden Language of Computer Hardware and Software"
**Author:** Charles Petzold

This book builds from flashlights and Morse code all the way to CPUs and operating systems. After reading it, nothing in computing feels like magic. You understand that with a keyboard, you change physical reality.

[My full notes on this book](./code-petzold)

---

### 2. Watch "Exploring How Computers Work"
**Channel:** Sebastian Lague

Short visual explanation of how computers work at the hardware level. Good supplement to Petzold.

**Link:** [https://www.youtube.com/watch?v=QZwneRb-zqA](https://www.youtube.com/watch?v=QZwneRb-zqA)

---

### 3. Watch all 41 videos of "Crash Course Computer Science"
**Host:** Carrie Anne Philbin

Covers same ground as Petzold but in video format with animations. 40 episodes, ~10 minutes each. From early computing to AI and future of computing.

**Link:** [https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo](https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)

---

### 4. Take "Build a Modern Computer from First Principles: From Nand to Tetris"
**University:** Hebrew University of Jerusalem

You build a computer from scratch. Start with NAND gate, end with working computer that runs Tetris. This is where theory becomes real.

**Link:** [https://www.nand2tetris.org/](https://www.nand2tetris.org/)

**Coursera:** [https://www.coursera.org/learn/build-a-computer](https://www.coursera.org/learn/build-a-computer)

---

## Phase 2: Learn Programming Fundamentals

### 5. Take "CS50: Introduction to Computer Science"
**University:** Harvard

The best introduction to programming and computer science. Starts with C, moves to Python, then web development. Problem sets force you to think, not just copy.

**Link:** [https://cs50.harvard.edu/x/](https://cs50.harvard.edu/x/)

**YouTube:** [https://www.youtube.com/c/cs50](https://www.youtube.com/c/cs50)

---

## Phase 3: Master C Language

### 6. Read "C Programming: A Modern Approach"
**Author:** K.N. King

Use this as your main C textbook. Comprehensive, well-structured, modern approach. Better than K&R for learning.

---

### 7. Follow "Tutorial On Pointers And Arrays In C"
**Author:** Ted Jensen

Pointers are where most C learners struggle. This tutorial explains them clearly with examples.

**Link:** [https://pdos.csail.mit.edu/6.828/2017/readings/pointers.pdf](https://pdos.csail.mit.edu/6.828/2017/readings/pointers.pdf)

---

## Why This Order Matters

| Step | What You Learn |
|------|----------------|
| Petzold | How computers work at physical level |
| Sebastian Lague | Visual reinforcement |
| Crash Course | Breadth of CS topics |
| Nand to Tetris | Build actual computer from gates |
| CS50 | Programming thinking + C basics |
| K.N. King | Deep C knowledge |
| Pointers tutorial | Master the hardest part |

By the time you write `int *p = &x;` you understand:
- What memory actually is (flip-flops holding state)
- How addresses work (binary numbers selecting locations)
- What happens when you dereference (fetching value from that address)

No magic. Just layers of abstraction you have seen built from scratch.

---

## Additional Resources

| Resource | Purpose | Link |
|----------|---------|------|
| Beej's Guide to C | Alternative reference | [https://beej.us/guide/bgc/](https://beej.us/guide/bgc/) |
| Exercism C Track | Mentored practice | [https://exercism.org/tracks/c](https://exercism.org/tracks/c) |
| Project Euler | Math + C practice | [https://projecteuler.net/](https://projecteuler.net/) |

---

*This is the path I followed. It takes longer than jumping straight into syntax, but the understanding you build lasts forever.*

[← Back to Home](../)
