---
layout: post
title: Deployment Plan
date: 2022-03-28 12:53:00
categories: [drain-gang, project update, deployment, linux, AWS]
---

**Deployment off of AWS in progress:**
- Site being hosted at this [URL](http://18.190.152.109/)
- System setup to rebuild and deploy every Friday Morning
  - Done using `cronjobs` and basic deployment `script`


**WIP // Future Plans:**
- Move from using `cronjobs` to using `systemd timers`, a more robust solution for scheduling jobs on linux systems
- Make use of `S3 buckets` to store `CSV` and `XLSX` files for the application
- Plan on a **github workflow**, two options:
  - Move into a **PR workflow**, all changes are made in PRs and are needed to be **approved** by a team member before being merged into main repository
  - Creating a **deployment branch**, only working code is merged into it and two or more team members must **agree** with merging the master branch into the deployment one. 
