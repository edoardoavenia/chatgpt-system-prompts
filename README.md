# ChatGPT System Prompts

A modular system of prompts and tools for creating and customizing GPT applications. This repository documents the various system components and their activation conditions.

## 🎯 Structure and Modularity

The system is designed with a modular structure where tools can be activated or deactivated based on specific configurations.

### 🔨 Base Tools

These tools are part of the base configuration, though all can be deactivated:

1. DALL-E [`dalle.md`](./dalle.md)
   - Prompt-based image generation
   - Automatic English translation
   - Artistic and copyright constraints management
   - Output size customization

2. Web [`web.md`](./web.md)
   - Real-time information search
   - Location-aware services
   - URL and web navigation management
   
   > Note: This tool replaces the previous "browser". Interestingly, the prompt includes specific instructions not to use the old tool, suggesting possible interactions with previous fine-tuning. The behavior appears to have been updated, possibly in relation to GPT Search integration.

3. Python Environment [`python.md`](./python.md)
   - Jupyter-style execution environment
   - Data visualization tools
   - File persistence system

4. Canvas [`canmore.md`](./canmore.md) - New
   - Document creation and management
   - Pattern-based update system
   - Feedback and review functionality

5. Memory System [`bio.md`](./bio.md)
   - Information persistence across conversations
   - Automated reference system

   > Note: Unlike other tools which are simply removed from the prompt when deactivated, this tool shows a specific "tool disabled" message in the system prompt when deactivated.

### 🔄 Conditional Tools

These tools appear in the system prompt only under specific conditions:

1. File Browser [`myfiles_browser.md`](./myfiles_browser.md)
   - Activation Condition: Automatically appears when files are uploaded to the chat or GPTs files
   - Multi-query document search
   - Citation system
   - Intelligent query decomposition

2. API Actions [`api_action.md`](./api_action.md)
   - Activation Condition: Only appears when API integrations are configured
   - Complete CRUD framework
   - Standardized namespace management
   - Response handling structure

## 📝 System Prompts

### Base ChatGPT Configuration [`generic_system_prompt.md`](./generic_system_prompt.md)
The complete configuration for the standard chat interface, including all default behaviors and tool interactions when every feature is activated. This serves as the foundation for understanding how the various components work together.

### Custom GPT Introduction [`custom_gpt.md`](./custom_gpt.md)
The standard introduction message that informs custom GPTs about their nature as specialized versions of ChatGPT.

### GPT Builder [`gpt_builder.md`](./gpt_builder.md)
A dedicated assistant specifically designed to help users create custom GPTs:
- Available in the "Create new GPT" section
- Uses `gizmo_editor` as its sole tool
- Provides guidance for GPT customization