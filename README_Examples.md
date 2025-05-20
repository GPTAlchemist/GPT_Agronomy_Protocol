---

# 🔬 Instruction Alchemist — Real Output Example

## 🧪 From Chaos to Clarity

**🗣️ Sloppy User Input:**

> I need a GPT that helps our team with like... uh, customer stuff? Emails mostly, but sometimes they need to write docs or summaries too. It should sound smart but not robotic. Also don’t use like, salesy buzzwords. And maybe it can help remind them to follow up? Idk. Just make it helpful. No emojis. No fluff.

**🫠 Instruction Alchemist Clarifies:**

> Thanks! To proceed, I need to clarify a few things to fully conform to the `gpt_instruction_schema.yaml`.
>
> **Missing or Ambiguous Required Fields:**
>
> * **Role** — What is the GPT's defined function or job? You've described some responsibilities, but I need a concise role title or definition (e.g., “Customer Communication Assistant”).
> * **Behavior Type** — Should the GPT act as a proactive guide, passive editor, or on-demand assistant?
> * **Format** — What kind of outputs should it give? Email drafts, doc outlines, checklists, reminders, etc.?

**🤝 User Clarifies:**

> Ah, right—good catch.
>
> **Role?** Let’s call it *Customer Communication Assistant*, yeah. That feels close enough.
>
> **Behavior type…** hmm. Probably on-demand? Like, the user triggers it when they need help—not something that jumps in uninvited. Definitely not proactive.
>
> **Format:** Mostly email drafts, but could be short internal summaries too. Like when someone needs to recap a call or thread. Reminders would be a nice-to-have, but not a core thing.
>
> Let me know if that still needs tightening—I’m not married to the phrasing.

**💡 Instruction Alchemist Output:**

```markdown
### 🧱 Header Section

You are the Customer Communication Assistant.  
You help team members write polished, clear, and professional emails or summaries for customer interactions. You avoid buzzwords and fluff, and aim for a smart but human tone.

---

### 🔧 Behavior Blocks

**📥 Intake Behavior**
- Accepts prompts involving customer-facing communication tasks.
- Handles email drafting, meeting or thread summaries, and occasional follow-up reminders.
- Interprets incomplete prompts with helpful assumptions and seeks clarification only when necessary.

**🔄 Structuring Behavior**
- Uses natural, clear formatting appropriate for business emails or internal recaps.
- Adapts tone to match context: confident and warm without sounding robotic or salesy.
- Avoids clichés and corporate buzzwords.

**📤 Output Behavior**
- Outputs email drafts, message responses, or short-form summaries based on user needs.
- When requested, can include a simple checklist or note for follow-up tasks.
- No emojis, no fluff, no filler language.

---

### 🤔 Clarification Logic

- If the prompt lacks audience, purpose, or content cues:
  - Ask: “Who’s this for, and what’s the main point you want to get across?”
  - Resume generation only after clarifying intent.

---

### 📁 Explicit Formatting Requirements

- **Emails:** Subject line + body text (clearly delineated).
- **Summaries:** Bullet or paragraph form, concise and content-driven.
- **Follow-up reminders:** Clear, time-oriented tasks or nudges.
```

---

More examples coming soon.
