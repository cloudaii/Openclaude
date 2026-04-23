# OpenClaude Android

**Deploy an autonomous, hardware-aware AI agent directly onto your Android device using Termux, Shizuku, and OpenRouter LLMs**.

# About Project

This repository provides zero-effort configuration scripts to deploy OpenClaude into the Android ecosystem.

Beyond simply running a terminal-based AI, this Supercharged Edition leverages Shizuku and the Android UIAutomator framework to give the AI physical control over your device. The AI can autonomously traverse your file system, read screen hierarchy dumps to "see" apps, and tap, swipe, and type its way through native UI tasks—effectively acting as an autonomous God-Mode assistant.

# Key Features

• **Autonomous UI Control**: Natively hooks 
    into Shizuku to allow the AI agent to 
    execute screen coordinates, swipe, and 
    interact with visual elements 
    dynamically.

• **1-Click PC Installer**: Ships with an 
    automated PowerShell script  
    (pc_push_install.ps1) that deploys all 
    APKs, grants all necessary permissions 
    via ADB, and bootstraps Termux silently  
    without a single manual interaction on 
    the phone.

• **Dynamic Model Selection**: Automatically     polls the live OpenRouter API on startup 
    to list currently available 100% free 
    models.

• **Limitless Auto-Execution**: Bypasses  
    terminal permission prompts using the 
    injected --limitless execution flag and 
    optimized CLAUDE.md context overrides, 
    preventing "I am just an AI" rejection 
    loops.

• **Network Architecture Resilience**:  
    Features built-in cryptographic library 
    healing (libngtcp2/openssl) and DNS path 
    reroutes to prevent common Termux HTTPS 
    request failures under load.

# Installation

You can install this using either a PC (Fastest/Fully Automatic) or directly on the Phone. You will need an OpenRouter API Key.

# Option 1: Using a PC

This method automates the entire process including APK installation, permission granting, and environment bootstrap.

1. Enable Developer Options and USB
   Debugging on your Android phone.
   
2. Plug your phone into your Windows PC.
   
3. Download this completely repository to
   your PC and double-click 4
   pc_push_install.ps1. (If it prompts you,     type R to run once).
   
4. Once the setup completes, your Termux app    will automatically launch.

5. In your phone's Termux terminal, type
   exactly what the script tells you:
   ```
   bash~/storage/shared/Download/bootstrap.sh
   bash ~/termux_setup.sh
   ```
# Option 2: Phone-Only (No PC)

If you don't have a PC, you can configure it entirely on your phone.


