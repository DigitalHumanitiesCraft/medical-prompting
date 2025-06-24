# Medical Prompting Quickstart Guide

When working with LLMs on medical topics, direct questions often lead to oversimplified or inaccurate responses. This guide shows you how to get reliable, well-reasoned medical information through strategic prompting.

## Core Principle: Build Context, Then Validate

LLMs work best when you guide them through logical steps rather than asking for immediate conclusions. Think of it as teaching the AI to "show its work."

## Strategy 1: Multi-Step Contextual Prompting

**❌ Don't do this:**
> "I have a herniated disc in my cervical spine. What exercises should I do?"

**✅ Do this instead:**

1. **Build the foundation:** "I have a herniated disc at C5-C6. Which specific muscle groups are most affected by this condition?"

2. **Layer on context:** "For those muscle groups you mentioned, what types of exercises are generally recommended for strengthening and flexibility?"

3. **Get specific:** "Based on that information, create a beginner-friendly exercise routine for someone with a C5-C6 herniated disc."

4. **Force validation (LLM-poking):** "Review this exercise plan carefully. Is this really appropriate and safe? List any potential concerns or modifications needed, and explain your reasoning."

### Why This Works
- Each step builds logical context
- The LLM can't skip important considerations
- Final validation catches oversights or unsafe recommendations

## Strategy 2: Combat Pseudo-Precision with Aggressive Fact-Checking

LLMs hate saying "I don't know" and will often provide confident-sounding but inaccurate numbers or facts.

**❌ Dangerous question:**
> "How long do the antioxidants in green tea remain stable after brewing?"

**✅ Better approach:**

1. **Ask with uncertainty built-in:** "What does current research say about antioxidant stability in brewed green tea over time? Be specific about what you know vs. what you're uncertain about."

2. **Force honesty:** "Be absolutely honest about any facts and numbers you don't know exactly. Use web research for claims you're unsure of, and if you can't find 100% proven facts, say so explicitly."

3. **Validate sources:** "What specific studies or sources support these timeframes? If you're making estimates, clearly label them as such."

## Quick Reference: Validation Phrases That Work

Use these "LLM-poking" prompts to force better responses:

- "Is this really accurate? Double-check your reasoning."
- "What are you uncertain about in this response?"
- "List potential risks or contraindications I should know about."
- "Be completely honest about what current research does vs. doesn't support."
- "Search for recent studies to verify these claims."

## The Golden Rule

**Never accept the first response for medical questions.** Always iterate at least 2-3 times with validation prompts. The LLM's second and third responses are typically much more accurate and nuanced.

## Red Flags to Watch For

- Overly confident responses to complex questions
- Specific numbers without cited sources  
- Generic advice that doesn't account for individual variation
- Responses that don't mention consulting healthcare providers

## Remember

This guide helps you get better information from LLMs, but **always consult qualified healthcare professionals** for medical decisions. LLMs are research tools, not replacements for professional medical advice.
