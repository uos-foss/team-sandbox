# 🚀 Team Sandbox: Our Learning Blog

Welcome to our team's GitHub sandbox! This website is powered by **Beautiful Jekyll** and hosted live via GitHub Pages. 

The purpose of this project is to give everyone on the team a safe, zero-stress environment to practice using GitHub, writing in Markdown, creating branches, and participating in code reviews.

👉 **Live Site URL:** [`https://[Your-Org-Name].github.io`](https://uos-foss.github.io/team-sandbox/)

---

## 🌳 The Rule of the Land: Always Use Branches!
To keep our website safe, the **`main` branch** is protected. You cannot save changes directly to it. Instead, you must grow a temporary side-branch, do your work there, and ask the team to look at it via a **Pull Request (PR)**.

---

## ✍️ Guide for Content Creators (Non-Coders)

You can do all of this directly on the GitHub website using your browser. No coding required!

### Step 1: Create Your Workspace (Branch)
1. At the top left of this page, click the dropdown menu that says `main`.
2. Type a new name for your branch using this format: `content/your-name/topic` (e.g., `content/sarah/my-first-post`).
3. Click **"Create branch: content/your-name/topic..."**. You are now in a safe sandbox!

### Step 2: Write a Blog Post
1. Click into the **`_posts/`** folder.
2. Click **Add file** (top right) -> **Create new file**.
3. **Name your file exactly like this:** `YYYY-MM-DD-your-title.md` (e.g., `2026-05-18-hello-world.md`). *Note: It must end in `.md`.*
4. At the very top of your file, copy and paste this configuration block (called Front Matter) and update it:
   ```yaml
   ---
   layout: post
   title: "My Awesome First Post!"
   author: "Your Name"
   ---
   ```
   5. Below that block, type your post using regular text and **Markdown**. (See the Markdown Cheat Sheet below).
    

### Step 3: Save and Ask for Review

1. Click the green **Commit changes...** button in the top right. Write a short note about what you did (e.g., _"Added Sarah's intro post"_).
