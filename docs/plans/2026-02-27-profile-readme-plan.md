# GitHub Profile README Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Create a clean, professional GitHub profile README for `mattbobambrose/mattbobambrose`.

**Architecture:** Single `README.md` file with four sections: header/intro, featured projects, tech stack badges, and GitHub stats cards. Uses shields.io for tech badges and github-readme-stats for stats cards. All static markdown — no GitHub Actions.

**Tech Stack:** Markdown, shields.io badges, github-readme-stats

---

### Task 1: Create README with header and intro

**Files:**
- Create: `README.md`

**Step 1: Write the README with header section**

```markdown
# Hi, I'm Matthew Ambrose

**CS student at Northeastern University** (expected May 2027) specializing in Kotlin development, voice AI, and AI agent pipelines. Two co-op terms building AI-powered healthcare applications at EO Care — from voice-based patient onboarding to end-to-end AI agent pipelines driving Bayesian clinical decision-making.
```

**Step 2: Verify rendering**

Run: `cat README.md`
Expected: File exists with header content.

**Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add profile README with header and intro"
```

---

### Task 2: Add featured projects section

**Files:**
- Modify: `README.md`

**Step 1: Add featured projects**

Append after the intro:

```markdown
## Featured Projects

| Project | Description |
|---------|-------------|
| [**vapi4k**](https://github.com/vapi4k/vapi4k) | Open-source Ktor plugin and Kotlin DSL for defining, deploying, and maintaining Vapi voice AI applications |
| [**Koog**](https://github.com/JetBrains/koog) | Contributor to JetBrains' Kotlin framework for building AI agents — used in production for clinical fact extraction |
| [**MCP Utils**](https://github.com/mattbobambrose/mcp-utils) | Kotlin library for building MCP servers with automatic tool registration via `@LLMTool` annotations |
| [**Claude Code Plugins**](https://github.com/mattbobambrose/mattbobambrose-claude-skills) | Community marketplace of Claude Code plugins for code quality, documentation, testing, and Kotlin tooling |
```

Note: `personal-finance-simulator` is private — excluded. Koog and vapi4k link to their respective orgs (JetBrains, vapi4k).

**Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add featured projects section"
```

---

### Task 3: Add tech stack badges

**Files:**
- Modify: `README.md`

**Step 1: Add tech stack section with shields.io badges**

Append after featured projects:

```markdown
## Tech Stack

**Languages**

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)

**Frameworks**

![Ktor](https://img.shields.io/badge/Ktor-087CFA?style=flat&logo=ktor&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat&logo=jetpackcompose&logoColor=white)
![Kotest](https://img.shields.io/badge/Kotest-7F52FF?style=flat&logoColor=white)

**Infrastructure & Tools**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0080FF?style=flat&logo=digitalocean&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
```

**Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add tech stack badges"
```

---

### Task 4: Add GitHub stats cards

**Files:**
- Modify: `README.md`

**Step 1: Add stats section**

Append after tech stack:

```markdown
## GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=mattbobambrose&show_icons=true&theme=default&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=mattbobambrose&layout=compact&theme=default&hide_border=true)
```

**Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add GitHub stats cards"
```

---

### Task 5: Final review and push

**Step 1: Review the full README**

Run: `cat README.md`
Expected: All four sections present and well-formatted.

**Step 2: Push to GitHub**

```bash
git push origin master
```

**Step 3: Verify on GitHub**

Visit https://github.com/mattbobambrose to confirm the profile README renders correctly.
