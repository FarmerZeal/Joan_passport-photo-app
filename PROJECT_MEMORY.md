# PROJECT_MEMORY.md

# Project Joan — Permanent Project Memory

Last Updated: 2026-07-24

---

# Mission

Project Joan aims to become a professional offline-first passport photo application that produces print-ready outputs with maximum simplicity, reliability, and speed.

The application should work completely offline after installation and never require users to upload personal photos to any server.

Privacy is a core principle.

---

# Vision

Build one excellent product.

Avoid feature bloat.

Every new feature must improve the user experience.

Quality is preferred over quantity.

---

# Core Philosophy

Finish one product before rebuilding it.

Small improvements are better than unnecessary rewrites.

Do not restart projects because of new ideas.

Ship.
Test.
Improve.
Repeat.

---

# Development Principles

1. Offline First

The application must continue working without an internet connection after installation.

2. Privacy First

Images are processed entirely on the user's device.

No uploads.

No cloud processing.

3. Simplicity

Avoid unnecessary libraries.

Prefer Vanilla JavaScript whenever practical.

4. Stability

Never replace working code unless there is a measurable benefit.

5. Documentation First

Important decisions must always be documented.

---

# Technology Stack

HTML5

CSS3

Vanilla JavaScript

Canvas API

jsPDF

Service Worker

Web App Manifest

GitHub Pages

---

# Current Architecture

Single Page Application

No backend

No database

No login

Everything runs locally.

---

# Deployment Strategy

Primary deployment:

GitHub Pages

Development:

localhost

Never use file:// for production testing.

Reason:

Local file restrictions cause inconsistent browser behavior.

---

# UI Philosophy

Retro Windows 95

Monochrome

High Contrast

Courier Font

Square Buttons

Minimal animation

Fast loading

Large touch targets

---

# Features (Completed)

✔ Passport Photo Generator

✔ PDF Export

✔ JPG Export

✔ JPEG Export

✔ Automatic A4 Layout

✔ Custom Copy Count

✔ Auto Fill Maximum

✔ Preview Canvas

✔ Cut Guide Lines

✔ Offline Support

✔ Progressive Web App

✔ Home Screen Installation

✔ GitHub Pages Deployment

✔ Custom App Icon

---

# Major Problems Solved

Problem

jsPDF NOT LOADED

Cause

Local browser restrictions while using file://

Decision

Move project to GitHub Pages.

Result

Fixed.

------------------------------------------------

Problem

Offline PDF not working

Cause

Application wasn't served correctly.

Decision

Deploy as PWA with Service Worker.

Result

Offline PDF generation works.

------------------------------------------------

Problem

Home Screen App failed

Cause

localhost shortcut was used.

Decision

Install PWA from GitHub Pages instead.

Result

Working.

------------------------------------------------

Problem

Application Icon missing

Cause

Manifest icon path incorrect.

Decision

Create icons folder.

Update manifest paths.

Result

Working.

---

# Permanent Decisions

Never use file:// for production.

Always deploy using GitHub Pages.

Always keep jsPDF locally inside libs/.

Never depend on external CDN for production.

Documentation is part of the project.

---

# Documentation Rules

The following files must always remain synchronized.

README.md

PROJECT_MEMORY.md

CHANGELOG.md

TODO.md

Whenever one major feature is completed,

all four documents should be updated.

---

# Single Source of Truth

PROJECT_MEMORY.md is the official project memory.

If documentation conflicts with conversation history,

PROJECT_MEMORY.md has priority unless intentionally changed.

---

# Development Workflow

Plan

↓

Implement

↓

Test

↓

Fix

↓

Update Documentation

↓

Commit

↓

Deploy

↓

Release

---

# Milestone Rule

Every important milestone MUST update PROJECT_MEMORY.md.

This is a permanent project rule.

No milestone is considered complete until PROJECT_MEMORY.md has been updated.

---

# Current Version

v1.0 Beta

Status

Stable

Offline

Working

PWA

Working

GitHub Pages

Working

Ready for real-world testing.

---

# Future Goals

Improve printing workflow.

Improve UI polish.

Remember previous settings.

Support more passport formats.

Improve preview.

Reduce code complexity.

Maintain backward compatibility whenever possible.

---

# Developer Motto

Finish one product before rebuilding it.

Code is temporary.

Documentation is permanent.

PROJECT_MEMORY.md is the project's memory.