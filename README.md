# Node.js local environment setup

This guide explains how to install **Node.js**, **npm**, and **npx** on macOS, Windows, and Linux.

---

## ✅ macOS

1. Check if you have Homebrew installed:
   ```bash
   brew --version
   ```
   If you get `command not found`, install Homebrew:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. Install Node.js (includes npm and npx):
   ```bash
   brew install node
   ```

3. Verify versions:
   ```bash
   node -v
   npm -v
   npx -v
   ```

   You should see something like:
   ```
   v20.x.x
   10.x.x
   10.x.x
   ```

---

## ✅ Windows

1. Download and install Node.js from the official website:  
   👉 https://nodejs.org/

   - Use the **LTS** version (recommended for most projects).

2. After installation, open **Command Prompt** or **PowerShell** and check versions:
   ```bash
   node -v
   npm -v
   npx -v
   ```

   You should see something like:
   ```
   v20.x.x
   10.x.x
   10.x.x
   ```

---

## ✅ Linux (Debian/Ubuntu example)

1. Update your package index:
   ```bash
   sudo apt update
   ```

2. Install Node.js and npm:
   ```bash
   sudo apt install nodejs npm
   ```

   For some distros, you may want to install `npx` separately, but recent versions include it.

3. Verify versions:
   ```bash
   node -v
   npm -v
   npx -v
   ```

   Expected output:
   ```
   v20.x.x
   10.x.x
   10.x.x
   ```

---

## ✅ Tip: Run a local server

To test local scripts, you can use:
```bash
npx serve .
```
or
```bash
npx http-server .
```

This will serve your project at:
```
http://localhost:3000/
```
