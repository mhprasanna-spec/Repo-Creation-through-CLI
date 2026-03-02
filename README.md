# Repo-Creation-through-CLI


## 🚀 STEP 1 — Install Git (if not installed)

```
sudo apt update
sudo apt install git -y
```

Check:
```
git --version
```

## 🚀 STEP 2 — Configure Git (First Time Only)

```
git config --global user.name "YourGitHubUsername"
git config --global user.email "your-email@example.com"
```

Example:

- git config --global user.name "hellokumar"
- git config --global user.email "hellokumar@gmail.com"

Verify:
```
git config --list
```
## 🚀 STEP 3 — Create Repository on GitHub

Open browser

Go to 👉 https://github.com

Click New Repository

Name it: terraform-alb-project

Click Create Repository

DO NOT initialize with README

Keep that page open.

## 🚀 STEP 4 — Generate GitHub Token (PAT)

Go to GitHub

Click profile → Settings

Developer Settings

Personal Access Tokens

Tokens (classic)

Generate new token (classic)

Select:

✅ repo

Generate token

COPY the token (very important)

## 🚀 STEP 5 — Initialize Git in EC2

Go to your Terraform folder:

cd ~

Then:
```
git init
```

## 🚀 STEP 6 — Add Remote Repository

From your GitHub repo page copy HTTPS URL:

Example:

https://github.com/hellokumar/terraform-alb-project.git

Add it:
```

git remote add origin https://github.com/hellokumar/terraform-alb-project.git
```

Check:
```
git remote -v
```
## 🚀 STEP 7 — Add Files
```
git add .
```

Check:
```
git status
```
## 🚀 STEP 8 — Commit Files
```
git commit -m "Initial Terraform ALB Project"
```
## 🚀 STEP 9 — Push to GitHub (Using Token)
```
git branch -M main
git push -u origin main
```
It will ask:

- Username:

👉 Enter your GitHub username

Then:

- Password:

👉 Paste the Personal Access Token (NOT your GitHub password)

⚠ You will NOT see token while pasting — that is normal.

Press Enter.

## 🎉 DONE

Refresh GitHub page — your files will be there.
