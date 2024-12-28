# GPT System Prompts

A modular system of prompts and tools for creating and customizing GPT applications. This repository documents the various system components and their activation conditions.

## 🎯 Structure and Modularity

The system is designed with a modular structure where tools are activated based on specific conditions and configurations.

### 🔨 Base Tools (Always Available)

These tools can be activated in any chat:

1. DALL-E ([`./dalle.md`](./dalle.md))
   - Prompt-based image generation
   - Automatic English translation
   - Artistic and copyright constraints management
   - Output size customization

2. Web Tools ([`./web.md`](./web.md))
   - Real-time information search
   - Location-aware services
   - URL and web navigation management
   
   > Note: This tool replaces the previous "browser". Interestingly, the prompt includes specific instructions not to use the old tool, suggesting possible interactions with previous fine-tuning. The behavior appears to have been updated, possibly in relation to GPT Search integration.

3. Python Environment ([`./python.md`](./python.md))
   - Jupyter-style execution environment
   - Data visualization tools
   - File persistence system

4. Canvas Tool ([`./canmore.md`](./canmore.md)) - New
   - Document creation and management
   - Pattern-based update system
   - Feedback and review functionality

### 🔄 Conditional Tools

These tools are activated only under specific conditions:

1. File Browser ([`./myfiles_browser.md`](./myfiles_browser.md))
   - Activation Condition: Automatically activates when files are uploaded to the chat or GPTs files
   - Multi-query document search
   - Citation system
   - Intelligent query decomposition

2. API Actions ([`./api_action.md`](./api_action.md))
   - Activation Condition: Only activates when API integrations are configured
   - Complete CRUD framework
   - Standardized namespace management
   - Response handling structure

3. Custom GPT Builder ([`./custom-gpt.md`](./custom-gpt.md))
   - Activation Condition: An assistant available only during new GPT creation
   - Configuration instructions
   - Customization guidelines
   - Base templates

### ⚠️ Special Cases

1. Memory System ([`./bio.md`](./bio.md))
   - Status: Tool with conditional functionality
   - Shows a negative prompt when "locked"
   - Manages information persistence across conversations
   - Automated reference system

## 🛠 Base System Configuration

The [`./generic-system-prompt.md`](./generic-system-prompt.md) file contains the complete base system configuration, including all default behaviors and basic instructions for system operation. This file is the starting point for any customization and defines how various components interact with each other.