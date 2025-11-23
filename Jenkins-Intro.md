# Jenkins-Intro.md

# 🧠 Jenkins – CI/CD Automation Intro

## What is Jenkins?

- Free, open-source CI/CD automation tool
- Automates build, test, deploy, and delivery of software
- Written in Java, with a web GUI
- Automates repetitive/manual tasks—reliable, fast, and error-free

---

## How Jenkins Uses CI/CD

### 1. Continuous Integration (CI)

- Developers frequently push/merge code to a central repo (e.g., GitHub).
- Jenkins detects the push, builds and tests code automatically.
- Failing tests/compilations trigger instant feedback (alerts to team).

### 2. Continuous Delivery (CD)

- After passing CI, Jenkins prepares the app for staging or release.
- No need to manually deploy or build packages.

### 3. Continuous Deployment (CD)

- Jenkins can fully automate going to production after every successful build/test.

| Term    | Meaning                                                          |
|---------|------------------------------------------------------------------|
| CI      | Code merged → auto build + test → feedback to team               |
| CD (Del)| Code ready for deploy on every commit                            |
| CD (Dep)| Code is **automatically** deployed (no manual intervention)      |

---

## Jenkins History

| Year | Event                                                                           |
|------|---------------------------------------------------------------------------------|
| 2004 | Hudson tool created by Kohsuke Kawaguchi at Sun Microsystems for build/test auto |
| 2010 | Oracle acquired Sun, community dispute                                          |
| 2011 | Project forked/renamed to Jenkins, community driven                             |
| Today| Jenkins = world’s most popular open-source CI/CD tool                           |

---

## Why Jenkins?

- Automation = less time on manual steps
- Integration = 100s of plugins (Git, Docker, AWS, Slack, …)
- Fast feedback for faster delivery
- Open-source, free, and widely supported

---

## Visual Flow

Developer → Build Engineer → Testing Server → Production Server
↓ ↑
Jenkins automates this whole cycle!

 

---

## Summary

- Jenkins = automation + CI/CD
- Built in Java, open-source
- Pioneered by Kohsuke Kawaguchi (from Hudson)