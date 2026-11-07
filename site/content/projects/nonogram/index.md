
---
title: "Nonogram CSP Solver"
date: 2026-06-21T10:00:00+09:00
draft: false
slug: nonogram-csp-solver
description: "CSP modeling and search algorithm optimization for Nonogram puzzles"
summary: "A Python-based Nonogram solver implementing Backtracking, Revise, and AC-3 algorithms."
featured: true
tags:
  - Python
  - Artificial Intelligence
  - CSP
  - Backtracking
  - AC-3
  - PyQt
---

## Project Overview

This project focuses on solving Nonogram puzzles using Constraint Satisfaction Problems (CSP).

The goal was to model Nonogram puzzles as CSPs and compare different search and constraint propagation algorithms.

## My Contributions

- Modeled each row and column as a CSP variable.
- Generated possible patterns for each variable's domain.
- Implemented pure Backtracking Search.
- Applied Revise filtering to eliminate inconsistent domain values.
- Implemented AC-3 using queue-based constraint propagation.
- Built a PyQt-based visual debugger.
- Analyzed and corrected an issue in the AC-3 queue update logic.

## Experimental Results

The algorithms were tested using identical puzzle inputs.

| Puzzle Size | Backtracking | Revise | AC-3 |
|---|---:|---:|---:|
| 7×7 | 1.789 s | 0.0118 s | 0.0117 s |
| 10×10 | 8.958 s | 0.0613 s | 0.0276 s |
| 15×15 | Timeout | Timeout | 0.136 s |

The timeout threshold was 15 seconds.

AC-3 successfully solved the tested 15×15 puzzle within 0.136 seconds, while the other two approaches exceeded the time limit.

The following images show visual materials from the Nonogram CSP Solver project.

images/nonogram1.png



images/nonogram2.png



images/nonogram3.png



## What I Learned

Through this project, I gained experience in CSP modeling, Backtracking Search, constraint propagation, algorithm performance analysis, and debugging.

This experience strengthened my interest in artificial intelligence and algorithmic problem solving, which I hope to explore further in Physical AI and Robotics.

## Technologies Used

Python, CSP, Backtracking, Revise, AC-3, PyQt
