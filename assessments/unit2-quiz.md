# Unit 2 Quiz: Applied Prompt Engineering

**Time Limit:** 15 minutes
**Total Points:** 50
**Passing Score:** 35/50 (70%)

---

**Instructions:**
- Answer all 10 questions.
- Multiple choice: Select the single best answer.
- Short answer: Write 2-4 sentences unless otherwise specified.
- Practical: Follow the specific instructions provided. Show your reasoning.
- No AI tools may be used during this assessment.

---

## Section A: Multiple Choice (2 points each | 10 points total)

**1. In the CO-STAR framework, what does the "A" stand for?**

- A) Action
- B) Audience
- C) Analysis
- D) Application

**2. When should you choose the Chain-of-Thought (CoT) framework over a simple Zero-Shot prompt?**

- A) When you need a one-word answer
- B) When the task requires multi-step reasoning, math, or logic
- C) When you want the shortest possible response
- D) When you are writing creative fiction

**3. What is "Few-Shot" prompting?**

- A) Providing the AI with a few examples of the desired input-output pattern before asking your question
- B) Limiting the AI to only a few words in its response
- C) Asking the AI the same question multiple times
- D) Using the AI for only a few minutes at a time

**4. What is the primary benefit of Chain-of-Thought prompting?**

- A) It makes the AI respond faster
- B) It forces the AI to show its reasoning step-by-step, improving accuracy on complex tasks
- C) It reduces the token count of the response
- D) It bypasses the AI's safety filters

**5. Which statement about formatting differences between GPT and Claude is MOST accurate?**

- A) GPT and Claude accept identical prompt formatting with no differences
- B) Claude tends to respond well to XML tags for structure, while GPT often works well with Markdown headers and clear sectioning
- C) Claude cannot process structured prompts
- D) GPT requires all prompts to be in JSON format

---

## Section B: Short Answer (5 points each | 15 points total)

**6. CO-STAR Prompt Construction**

You are an HR manager who needs to write a job rejection email that is professional yet empathetic. Using the CO-STAR framework, write out each element (Context, Objective, Style, Tone, Audience, Response format) for this scenario. You do not need to write the full prompt -- just identify each CO-STAR element clearly.

**7. Constraint Engineering**

Explain what "constraint engineering" means in prompt design. Give two specific examples of constraints you might add to a prompt to improve output quality (e.g., length limits, format requirements, exclusions).

**8. Multi-Role Technique**

Describe the "Multi-Role" prompting technique. When is it most useful, and how does assigning multiple perspectives to the AI improve the quality of the output?

---

## Section C: Practical Application (12-13 points each | 25 points total)

**9. Prompt Transformation (12 points)**

The following is a poorly written prompt. Rewrite it as a well-structured prompt using any framework you have learned. Clearly label which framework you are using.

**Bad prompt:**
> "Tell me about our company's Q3 performance."

Your rewritten prompt must include: **(4 points each)**
- Clear context and role assignment
- Specific output requirements (format, length, audience)
- At least two constraints

**10. Framework Selection and Application (13 points)**

**Scenario:** A plant engineer needs to generate a daily production summary that will be emailed to shift supervisors. The summary must include production numbers, downtime incidents, and safety observations. It should be factual and concise.

- **Part A:** Which prompting framework is most appropriate for this scenario? Justify your choice. **(5 points)**
- **Part B:** Write the complete prompt using your chosen framework. **(8 points)**

---

**End of Quiz**
