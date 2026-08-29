# Development Setup Guide – AIRIS-AI (All Free)

**AIRIS-AI by Umaiz Sufiyan – 100% free, no payment gateway, no sponsorship.** All execution tools unlocked locally.

This guide details the process for standing up the AIRIS-AI development environment.

## Prerequisites

Ensure your system meets the following requirements:
- **OS:** Windows 10/11, macOS (Apple Silicon recommended), or Ubuntu Linux.
- **Runtime:** Node.js v23+
- **Version Control:** Git
- **IDE:** VS Code or Cursor recommended.

## Option 1: AIRIS-AI – Full Access (Free, Recommended)

For all developers – full React frontend + full system execution tools, **free and unlimited** (no sponsorship, no private repo):

```bash
# 1. Clone AIRIS-AI (free, all features)
git clone https://github.com/sufiyan-sabeel/AIRIS-ai.git

# 2. Navigate into the directory
cd AIRIS-ai

# 3. Install dependencies
npm install

# 4. Start the Vite development server
npm run dev
```

> **Original IRIS required sponsorship:** Option 1 was UI Shell only (tools stubbed) and Option 2 required **IRIS Insider ($15/mo)** private `iris-insiders` repo. **AIRIS-AI removes that – everything is free in the public AIRIS-ai repo.** No payment gateway.

## Option 2: Legacy IRIS Insider (Original, Now Free)

Original IRIS Insider is now merged into AIRIS-AI – no separate private repo needed. All voice-first functionality is in the public AIRIS-AI repo above.

```bash
# No private repo needed – use AIRIS-AI public repo (free)
git clone https://github.com/sufiyan-sabeel/AIRIS-ai.git
cd AIRIS-ai
npm install
npm run dev
```

### Linking Modules
If you are developing custom tools, place your integration logic within the protected Main Process directory. Ensure that any new IPC channels are properly registered in the `preload` script before invoking them from the React frontend.
