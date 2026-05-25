# Secure-Packages-with-CodeArtifact
A streamlined DevOps project showing how to securely manage Java dependencies using AWS CodeArtifact, EC2, IAM roles, and Maven. You authenticated with CodeArtifact, compiled your app, cached dependencies, published a custom package, and verified everything end‑to‑end in CloudShell.
![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)
![EC2](https://img.shields.io/badge/EC2-Compute-blue?logo=amazonaws)
![IAM](https://img.shields.io/badge/IAM-Security-red?logo=amazonaws)
![CodeArtifact](https://img.shields.io/badge/CodeArtifact-Package_Management-purple?logo=amazonaws)
![CloudShell](https://img.shields.io/badge/CloudShell-CLI_Tools-2D9CDB?logo=amazonaws)

![Maven](https://img.shields.io/badge/Maven-Build_Tool-yellow?logo=apachemaven)
![Java](https://img.shields.io/badge/Java-Development-orange?logo=openjdk)
![Git](https://img.shields.io/badge/Git-Version_Control-F05032?logo=git)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?logo=github)

![Linux](https://img.shields.io/badge/Linux-Server_Administration-green?logo=linux)
![Bash](https://img.shields.io/badge/Bash-Scripting-4EAA25?logo=gnubash)

![CI/CD](https://img.shields.io/badge/CI%2FCD-DevOps_Pipeline-blueviolet?logo=githubactions)
![Security](https://img.shields.io/badge/Security-Least_Privilege-critical?logo=datadog)

📑 Table of Contents
Project Overview

Key Tools and Concepts

Project Reflection

CodeArtifact Repository

CodeArtifact Security

IAM Policy Summary

Maven Integration

Verifying the Connection

Publishing Custom Packages

📘 Project Overview
This project demonstrates how to securely manage Java packages using AWS CodeArtifact, EC2, IAM, Maven, and GitHub. It shows how compute, identity, and source control work together in a cloud‑based development workflow.

“Altogether, these experiences strengthened my grasp of cloud infrastructure fundamentals— specifically how compute, identity, and source control work together…”
🛠️ Key Tools and Concepts
You strengthened hands‑on skills in:

EC2 Administration — installing software, managing packages, configuring Java/Maven

IAM Authentication — access keys, AWS CLI, roles, permissions

Git & GitHub — cloning, pushing, pulling, repo integration

CodeArtifact — secure package storage, upstream repos, caching

Maven Builds — compiling Java apps with private repositories

“I strengthened my skills in EC2 server administration… IAM authentication… version control with Git…”

<img width="1536" height="1024" alt="Copilot_20260524_195315_edited" src="https://github.com/user-attachments/assets/0ba6b22e-c165-4820-9fd3-896ca704254c" />

🧠 Project Reflection
You completed the entire workflow in a single focused session:

Launch EC2

Configure IAM

Clone GitHub repo

Integrate Maven with CodeArtifact

Compile the web app

Publish a custom package

Validate the package in CloudShell

“The work was concentrated, hands‑on, and completed within the same session…”

This is Project 3 in your DevOps CI/CD pipeline series.

📦 CodeArtifact Repository
You configured:

A domain (nextwork)

A repository with Maven Central as upstream

A secure, centralized package management workflow

🔐 CodeArtifact Security
Issue
Maven could not authenticate because the EC2 instance had no IAM role attached.

“Initially, we ran into errors because the EC2 instance had no IAM role attached…”

Resolution
You created an IAM policy and attached it to an EC2 role, granting:

Token retrieval

Repository endpoint discovery


“Our repository’s upstream is Maven Central… gaining the benefits of caching, security, and consistent builds…”

“We resolved the permissions error by creating an IAM policy… attaching it to an IAM role…”

📝 IAM Policy Summary
The policy grants the minimum permissions required for:

Getting an authorization token

The policy grants the minimum permissions required for:

Getting an authorization token

Discovering repository endpoints

Reading packages

“This IAM policy grants the minimum permissions required… retrieve an authorization token… read packages…”

⚙️ Maven Integration
You configured settings.xml to:

Authenticate with CodeArtifact

Use the correct repository

Apply a Maven profile for builds

“The settings.xml file configures Maven to use our CodeArtifact repository…”

🔍 Verifying the Connection
After compiling your web app, CodeArtifact displayed four full pages of cached packages, confirming successful integration.

“You opened your CodeArtifact repository and saw four full pages of packages…”

🚀 Publishing Custom Packages
You published your own internal package, then validated it by:

Downloading it in CloudShell

Unzipping it

Inspecting the contents

“Inside, I could clearly see the packaged files—including the original text file I created…”

This confirms CodeArtifact stored and retrieved your package correctly.
