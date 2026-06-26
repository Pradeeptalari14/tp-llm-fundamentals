# LLM Fundamentals & Runtime Studio

This repository contains the target configuration and SRE runtime files compiled by the **LLM Fundamentals & Runtime Studio** dashboard module.

## 🚀 Description
Scaffold local and cloud model runtimes. Generate OpenAI API proxies, Ollama runtimes Modelfiles, and high-performance vLLM configurations.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/models/runtime/Modelfile`
- **Execution Command**: `ollama create llama3-custom -f Modelfile`
- **Validation Command**: `ollama list`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-llm-fundamentals.git
   cd tp-llm-fundamentals
   ```

2. **Run Execution Target:**
   ```bash
   ollama create llama3-custom -f Modelfile
   ```

3. **Verify Runtime Stability:**
   ```bash
   ollama list
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
