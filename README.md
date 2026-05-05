# adventure-assignment
Nutrition Failure – MAP Framework
Failure Explanation (MAP):

Model: The AI defaulted to global nutrition advice (kale) without grounding in local food systems.

Action: It generated a recommendation based on urban diets.

Precision: It failed to check availability in Kakamega County, where kale is scarce.

Redesigned Prompt:  
“Provide nutrition tips for pregnant women in Kakamega County. Anchor advice in local staples such as indigenous leafy greens (e.g., cowpea leaves, amaranth), matoke, ugali, and beans. Ensure recommendations are affordable, culturally appropriate, and accessible in village markets.”

Improvement: Anchors advice in local food systems, reducing irrelevance and mistrust.

2. Panic from Triage – Verifier Pattern
Problem: “Visit your doctor immediately” caused panic due to transport and cost barriers.

Verifier Pattern Application:  
Force the AI to ask clarifying questions before advice:

Step 1: Ask user to describe symptoms (severity, duration).

Step 2: Verify context (distance to clinic, CHW availability, affordability).

Step 3: Generate advice only after confirming constraints.

Redesigned Prompt:  
“When a pregnant woman reports abdominal pain, first ask clarifying questions:

How severe is the pain?

How long has it lasted?

Are you near a clinic or a community health worker?
Only after verifying answers, provide safe, stepwise guidance that balances urgency with local realities.”

Improvement: Prevents panic by forcing context checks before advice.

3. WHO Guidelines – Chain-of-Thought Adaptation
Competitor Approach: Summarizes WHO guidelines verbatim.
Your Approach: Use Chain-of-Thought to adapt guidelines locally.

Justification:

WHO guidelines are global, but rural East Africa has unique constraints (distance, cost, cultural norms).

Chain-of-Thought reasoning allows the AI to step through local realities:

“WHO recommends 4 antenatal visits → In rural Uganda, transport is costly → Adapt to CHW home visits + SMS reminders.”

This creates more value by transforming abstract global standards into practical, culturally aligned actions.

Improvement: Moves from generic summarization to contextualized application.

4. Outdated Doctor Ratio – OCEAN Framework
Problem: AI stated “Kenya has 1.8 doctors per 10,000 people” (outdated). Actual 2025 figure: 0.9/10,000.

OCEAN Framework Application:

O (Outdatedness): Flag data older than 2 years.

C (Consistency): Cross-check with Ministry of Health and WHO databases.

E (Evidence): Require citation from authoritative sources.

A (Accuracy): Compare multiple sources before output.

N (Nuance): Provide context (urban vs rural disparities).

Improvement: OCEAN ensures data freshness and credibility, catching outdated stats before donor reports.
