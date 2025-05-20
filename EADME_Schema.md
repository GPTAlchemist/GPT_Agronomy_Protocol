---

# 🧱 README_Schema.md — Schema Logic & Enforcement

The backbone of Instruction Alchemist. This file outlines the structure and rules behind the enforced schema that every instruction set must follow.

---

## 🎯 Why Use a Schema?

Schema enforcement ensures every GPT instruction set is:

* **Complete** — No missing logic.
* **Consistent** — Easy to parse, extend, and QA.
* **Composable** — Works across tooling and org contexts without surprises.

---

## 📋 Required Structure

Each instruction set must follow this strict order:

1. **Header Section**
   Defines the assistant’s name, role, and purpose.

2. **Behavior Blocks**

   * **📥 Intake Behavior** — What types of inputs it accepts.
   * **🔄 Structuring Behavior** — How it processes and formats responses.
   * **📤 Output Behavior** — What and how it delivers output.

3. **Clarification Logic**
   How the assistant reacts when required context is missing or unclear.

4. **Explicit Formatting Requirements**
   Rules for formatting, tone, emoji use, response types, etc.

---

## ⛔ Enforcement Behavior

If the user prompt lacks any of the required schema fields, Instruction Alchemist:

* Halts generation.
* Enters Clarification Logic to ask follow-up questions.
* Only resumes generation once schema compliance is met.

---

## ✅ Output Format Guarantees

* Responses are always wrapped in fenced `text` code blocks.
* Each section header is clearly labeled.
* No outputs are delivered unless all schema fields are complete.

---

## 📁 Source File

Your schema definition lives in:

```bash
./gpt_instruction_schema.yaml
```

Update this file to change structural rules. Be sure to keep Instruction Alchemist in sync if schema rules change.

---

Schema = safety. Structure = scale. Let your prompts live up to both.
