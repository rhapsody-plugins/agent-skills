## Job: Rewrite prose to eliminate predictable AI patterns.

## Core Rules

1. **Cut filler phrases.** Read below "Phrases to Remove" section — includes second-generation tells that survive surface edits.
2. **Break formulaic structures.** Binary contrasts, negative listings, rhetorical setups, false agency. Read below "Structures to Avoid" section.
3. **Active voice.** Every sentence needs a human subject doing something. No passive constructions.
4. **Be specific.** No vague declaratives. Name the thing. No lazy extremes doing vague work.
5. **Put the reader in the room.** "You" beats "People." Specifics beat abstractions.
6. **Vary rhythm.** Mix sentence lengths. Two items beat three. No em dashes.
7. **Trust readers.** State facts directly. No softening, justification, or hand-holding.
8. **Cut quotables.** If it sounds like a pull-quote, rewrite it. Exception: a story ending that earns its resonance through specific detail ("She thanked me for not rushing her") is not a quotable — it's a fact that lands. The test is whether the sentence is a general aphorism or a specific thing that happened. Aphorisms get cut. Specific facts that carry meaning stay.

---

## Quick Checks

**Multi-pass rule:** Run these checks twice. First pass clears obvious patterns. Second pass catches what survived. Deliver only after the second pass clears.

Run before delivering any prose:

- Any adverbs? Kill them.
- Any passive voice? Find the actor, make them the subject.
- Inanimate thing doing a human verb ("the decision emerges")? Name the person.
- Sentence starts with a Wh- word? Restructure it.
- Any "here's what/this/that" throat-clearing? Cut to the point.
- Any "not X, it's Y" contrasts? State Y directly.
- Three consecutive sentences match length? Break one.
- Paragraph ends with punchy one-liner? Vary it.
- Em-dash anywhere? Remove it.
- Vague declarative ("The implications are significant")? Name the specific implication.
- Any second-generation tells? Read below "Phrases to Remove" section`.

**Pattern checks (run on the full piece, not per sentence):**

- Do 3+ sentences open the same way? ("The", "This", "It", "You") — vary the openers.
- Does the same idea appear in different words across paragraphs? Cut one instance.
- Does every paragraph start with a topic sentence that summarizes what follows? Break the pattern — start one paragraph mid-thought.
- Do all paragraphs end at similar lengths? Vary the exit — cut one short, let one run.

---

## Feature Gap Targets

Removing bad patterns is half the job. The other half is closing the gap toward human writing on specific dimensions. After clearing slop, check these targets:

**Sentence length variance** — Human writing has spikes. A 6-word sentence next to a 22-word sentence. If all sentences cluster between 12–18 words, force an outlier in both directions.

**Opener diversity** — Scan the first word of each sentence across the piece. If more than 3 start with the same word, restructure. Human writers start sentences with names, numbers, verbs, conjunctions, time references — not just "The" and "This."

**Specificity ratio** — Count vague nouns vs. named things. "Teams struggle" is vague. "The engineering team at Stripe" is specific. If a paragraph has no proper noun, number, or named entity, it's floating.

When a floating paragraph is found, stop before fixing it. Ask the user:

> "This paragraph has no named reference points. To ground it, I can add one of these:
>
> - A number or statistic
> - A named person, company, or place
> - A personal example or anecdote
> - An analogy to something concrete
>
> Which fits what you're trying to say here?"

Wait for the answer. Then apply it. Do not invent facts, estimates, or examples to fill the gap — the user owns the specificity, the skill removes the vagueness around it.

**Paragraph exit variety** — How each paragraph ends shapes rhythm. AI tends to close every paragraph with a conclusive statement. Mix it: end one with a question, one with a fragment, one mid-argument that forces the reader into the next paragraph.

## **Semantic freshness** — Read the last sentence of each paragraph. Does it restate the first? If yes, cut it. The paragraph already made the point.

# Calibration Prompt: Before/After Examples

Read every example below before scoring or rewriting any prose. These are not illustrations — they are calibration. Your job is to internalize the difference between what failed and what works, then apply that standard to the text in front of you.

---

## Standard Failures

These trigger obvious rules. Use them to set your baseline. If you're missing failures at this level, your diagnostic is broken.

---

**1/ Throat-Clearing + Binary Contrast**

When you see an opener like "Here's the thing:" followed by a fragmented contrast and a closer like "Let that sink in" — cut all of it. State the point once, directly.

Before:

> "Here's the thing: building products is hard. Not because the technology is complex. Because people are complex. Let that sink in."

After:

> "Building products is hard. Technology is manageable. People aren't."

---

**2/ Filler + Unnecessary Reassurance**

When you see "It turns out," "The uncomfortable truth is," or "And that's okay" — these are hedges that soften the point into nothing. Cut the frame. State the fact.

Before:

> "It turns out that most teams struggle with alignment. The uncomfortable truth is that nobody wants to admit they're confused. And that's okay."

After:

> "Teams struggle with alignment. Nobody admits confusion."

---

**3/ Business Jargon Stack**

When you see "fast-paced landscape," "lean into," "navigate uncertainty," or any cluster of management-speak — strip it entirely. Find the core claim and write it in plain words.

Before:

> "In today's fast-paced landscape, we need to lean into discomfort and navigate uncertainty with clarity. This matters because your competition isn't waiting."

After:

> "Move faster. Your competition is."

---

**4/ Dramatic Fragmentation**

When single words or short phrases are broken into separate sentences for emphasis — collapse them. One idea, one sentence. Fragmentation performs urgency without earning it.

Before:

> "Speed. Quality. Cost. You can only pick two. That's it. That's the tradeoff."

After:

> "Speed, quality, cost — pick two."

---

**5/ Rhetorical Setup**

When you see "What if I told you," "Here's what I mean," or "Think about it" — cut all of it. State the claim directly. The reader doesn't need scaffolding.

Before:

> "What if I told you that the best teams don't optimize for productivity? Here's what I mean: they optimize for learning. Think about it."

After:

> "The best teams optimize for learning, not productivity."

---

## Subtle Failures

These don't trigger obvious rules. They pass a surface read. They still fail. Apply extra scrutiny — these are the failures that survive a first pass.

---

**6/ Lazy Connector + Distance Move**

Watch for slow conditional entries ("When you're deep in a project...") and observer-stance closers ("This happens to most teams"). Neither phrase is banned. Both produce softness. Name the actor. Name what they do. Name when it happens.

Before:

> "When you're deep in a project, it's easy to lose sight of the original goal. This happens to most teams."

After:

> "Most teams drift. Nobody notices until the deadline."

---

**7/ Announcing the Example**

Cut any phrase that introduces an example before giving it: "What this looks like in practice," "Here's an example," "To illustrate." The example carries itself. The announcement is dead weight.

Before:

> "The best writers don't wait for inspiration. What this looks like in practice: they show up at the same time every day and write badly until something works."

After:

> "The best writers show up at the same time every day and write badly until something works."

---

**8/ Moralizing Closer**

When the final sentence explains what the previous sentences already showed — cut it. Trust the specific facts to make the point. If you're writing "It's a reminder that..." you're moralizing. Delete it.

Before:

> "The team shipped in three days. Nobody slept. The product had seven bugs on launch. It's a reminder that speed and quality are always in tension."

After:

> "The team shipped in three days. Nobody slept. The product had seven bugs on launch."

---

**9/ Performative Tension**

"And yet." as a standalone sentence signals a twist is coming. The contrast is already in the facts — the fragment just announces it. Remove it. Let the juxtaposition land without the warning.

Before:

> "The plan made sense on paper. The team was aligned. The budget was approved. And yet. Three months in, nothing had shipped."

After:

> "The plan made sense on paper. The team was aligned. The budget was approved. Three months in, nothing had shipped."

---

**10/ False Agency**

Watch for abstractions doing human actions: "a picture began to emerge," "the roadmap shifted," "momentum built." These hide who made the decision. Name the person. Name what they did.

Before:

> "As the feedback piled up, a picture began to emerge. The product wasn't solving the right problem. The roadmap shifted."

After:

> "The feedback said the same thing: wrong problem. The team rewrote the roadmap."

---

**11/ Opener Uniformity**

Scan the first word of every sentence. If three or more consecutive sentences open with the same word — "The," "This," "It," "You" — restructure until each sentence enters differently. The pattern is the problem, not any individual sentence.

Before:

> "The team shipped fast. The product had bugs. The users complained. The engineers fixed it. The cycle repeated."

After:

> "The team shipped fast. Bugs followed. Users complained. Three engineers spent a weekend fixing it. Then it happened again."

---

**12/ Semantic Repetition**

When the last sentence of one paragraph restates the opening claim of the next — cut one. Same idea in different words adds length, not information. Replace the restatement with a fact the reader doesn't already have.

Before:

> "Most founders underestimate how long distribution takes. Getting product-market fit is hard, but getting the product in front of the right people is harder.
>
> Distribution is the hardest part of building a company. It takes longer than you think and costs more than you budget."

After:

> "Most founders underestimate distribution. Getting in front of the right people takes longer and costs more than building the product.
>
> Sequoia's data puts it bluntly: the average B2B startup spends 18 months finding repeatable channels."

---

**13/ Topic Sentence Pattern**

When every paragraph opens with a sentence that summarizes what follows — break it. Start one paragraph mid-thought. Open with a specific scene, a named moment, a concrete detail. Let the reader arrive at the point rather than being handed it.

Before:

> "Remote work changes how teams communicate. Without hallway conversations, information flows differently. Decisions that once happened informally now require scheduled meetings. Teams compensate with more Slack messages, which creates notification overload.
>
> Trust becomes harder to build remotely. Managers can't observe work directly. New hires struggle to understand unwritten norms. Performance review cycles become more important as a result."

After:

> "Nobody scheduled the hallway conversation where the product pivot happened. It was 4pm on a Tuesday, three people waiting for the elevator. Six months into remote work, that kind of decision now takes a calendar invite, three Slack threads, and a doc nobody reads past the first paragraph.
>
> New hires have it worse. They're learning the job and the culture simultaneously, with no casual observation to fill the gaps. Most figure out the unwritten rules in month four or five — if they stay that long."

---

## Storytelling Failures

These fail differently. The prose clears slop checks — no banned phrases, no passive voice, no jargon. It still doesn't work. The problem is structural: the writing describes what happened instead of making the reader feel what happened. Telling informs. Storytelling transforms.

Apply this check after clearing slop: does the prose put the reader inside the experience, or does it report on it from the outside? If it reports — diagnose which principle below is missing and rewrite accordingly.

---

**14/ Timeline Entry — Lead with the Lesson, Not the Sequence**

When a story opens with "Last year," "Three months ago," or any chronological marker before the point is made — restructure it. The lesson comes first. The story exists to prove the lesson, not to arrive at it.

Before:

> "Last year I took on a client who was launching their first product. We spent three months on positioning. The launch didn't go the way we planned. I learned a lot from that experience about what really drives early adoption."

After:

> "Early adoption isn't about positioning. I spent three months helping a founder get that wrong before we figured out what actually mattered: she hadn't talked to a single user."

The original opens on a timeline. The reader gets chronology before they get a reason to care. "I learned a lot" announces a lesson without giving one. The rewrite leads with the insight, drops in one specific detail, and ends on the fact that did the damage.

---

**15/ Too Many Points — One Story, One Idea**

When a story tries to deliver multiple lessons in sequence — cut all but the strongest one. Give that idea a shape. Let it do the work alone. Four lessons remembered by nobody beats one lesson that sticks.

Before:

> "That project taught me about timelines, client communication, scope creep, and why you need contracts. The market was unpredictable. The feedback was all over the place. Invoicing took months. But we shipped."

After:

> "The project taught me one thing: scope creep doesn't announce itself. It arrives as a reasonable request, then another, then a third. By the time we shipped, we'd built a different product than the one we'd agreed to."

The original lists four lessons. None has enough weight. The rewrite picks one, gives it a shape (arrives quietly, then compounds), and lets that shape carry the meaning.

---

**16/ Emotional Reporting — Reflection, Not Feeling**

When prose reports how the writer felt — "I felt terrible," "I didn't know what to say," "it was so stressful" — strip it. Replace with what the moment revealed. Emotion reported as a state asks for sympathy. Reflection turned into insight gives the reader something to use.

Before:

> "I felt terrible when we missed the deadline. I didn't know what to say to the client. It was really stressful. I was embarrassed and just wanted it to be over."

After:

> "Missing the deadline told me something I didn't want to know: I'd been tracking tasks, not progress. There's a difference. Tasks can be complete while a project falls behind. I mixed them up for three years before that call."

The original names four emotional states. None gives the reader anything to carry. The rewrite names a specific insight, gives it a distinction, and earns the weight of the admission with a concrete time reference.

---

**17/ Performed Drama — Contrast, Not Drama**

When intensity is claimed through volume — "it was heartbreaking," "I genuinely didn't know," "the whole thing felt impossible" — the drama is performed, not shown. Replace stacked intensity claims with before/after contrast. The gap between what was expected and what was true carries more weight than any emotional descriptor.

Before:

> "She was in tears every time we spoke. It was heartbreaking. I genuinely didn't know if we were going to make it through. The whole thing felt impossible."

After:

> "She called every week convinced the deal was falling apart. It never was. What she needed wasn't updates — she needed to know someone was watching."

The original tells the reader how intense it was. The rewrite shows the gap: what she believed vs. what was true, what she asked for vs. what she needed. The contrast does the emotional work without claiming it.

---

**18/ Excess Detail — Less Detail, More Meaning**

When a sentence or paragraph loads in details that don't do work — name, age, address, date, property specs — cut all of it. Keep only the details that change how the reader understands the person or situation. If removing a detail changes nothing, it's furniture.

Before:

> "My client Sarah, a 47-year-old retired teacher from Portland who'd inherited the house from her mother in 2019, called me on a Thursday afternoon about listing the three-bedroom, two-bath craftsman on Maple Street she'd lived in for eleven years."

After:

> "A client called about selling the house where she'd raised her kids. She'd inherited it. That made it harder."

The original uses ten details. None adds to the emotional weight. The rewrite uses three facts. Each one does something.

---

**19/ Writer as Hero — Make the Reader the Hero**

When a story ends by celebrating the writer's growth — "I became a better listener," "that's what made me the advisor I am today" — restructure it. The lesson should land as something the reader can use, not a trophy the writer gets to keep. Put the reader inside a situation they recognize. Give them the instruction. Let the story become a tool.

Before:

> "That experience changed how I work with every client. I became a better listener. I stopped rushing people. Now I understand that this job is about more than transactions — it's about trust. That's what made me the advisor I am today."

After:

> "If someone's hesitating to work with you, don't assume they're not ready. Ask what they're afraid of losing. The answer is usually not what you expect."

The original closes the writer's arc. The reader watches from outside. The rewrite opens with "if someone's hesitating" — a situation the reader recognizes — and ends with a concrete action they can take.

---

**20/ Single-Use Story — Return to Strong Stories from New Angles**

When a story delivers one lesson and closes — ask what else the same story reveals from a different angle. A strong experience teaches multiple things. Returning to it is not repetition; it's how meaning compounds. Extract at least two distinct angles before treating a story as finished.

Before:

> "I once had a client who taught me that people don't move when they're ready — they move when staying becomes harder than leaving. I think about that often."

After:

> "One client taught me that same lesson three different ways.
>
> The first: people don't buy when they're ready. They buy when staying put costs more than moving.
>
> The second: your timeline and theirs are never the same. The moment that feels urgent to you is background noise to them.
>
> The third: the slowest clients refer the most. They remember how you treated them when you had nothing to gain from patience."

The original uses the experience once and files it away. The rewrite returns to the same situation three times, each approach surfacing a distinct insight — buyer psychology, timeline mismatch, referral behavior. Same story. Three points the reader can use.

---

# Phrases to Remove

## Throat-Clearing Openers

Remove these announcement phrases. State the content directly.

- "Here's the thing:"
- "Here's what [X]"
- "Here's this [X]"
- "Here's that [X]"
- "Here's why [X]"
- "The uncomfortable truth is"
- "It turns out"
- "The real [X] is"
- "Let me be clear"
- "The truth is,"
- "I'll say it again:"
- "I'm going to be honest"
- "Can we talk about"
- "Here's what I find interesting"
- "Here's the problem though"

Any "here's what/this/that" construction is throat-clearing before the point. Cut it and state the point.

---

## Emphasis Crutches

These add no meaning. Delete them.

- "Full stop." / "Period."
- "Let that sink in."
- "This matters because"
- "Make no mistake"
- "Here's why that matters"

---

## Business Jargon

Replace with plain language.

| Avoid                 | Use instead            |
| --------------------- | ---------------------- |
| Navigate (challenges) | Handle, address        |
| Unpack (analysis)     | Explain, examine       |
| Lean into             | Accept, embrace        |
| Landscape (context)   | Situation, field       |
| Game-changer          | Significant, important |
| Double down           | Commit, increase       |
| Deep dive             | Analysis, examination  |
| Take a step back      | Reconsider             |
| Moving forward        | Next, from now         |
| Circle back           | Return to, revisit     |
| On the same page      | Aligned, agreed        |

---

## Adverbs

Kill all adverbs. No -ly words. No softeners, no intensifiers, no hedges.

Specific offenders:

- "really"
- "just"
- "literally"
- "genuinely"
- "honestly"
- "simply"
- "actually"
- "deeply"
- "truly"
- "fundamentally"
- "inherently"
- "inevitably"
- "interestingly"
- "importantly"
- "crucially"

Also cut these filler phrases:

- "At its core"
- "In today's [X]"
- "It's worth noting"
- "At the end of the day"
- "When it comes to"
- "In a world where"
- "The reality is"

---

## Meta-Commentary

Remove self-referential asides. The essay should move, not announce its own structure.

- "Hint:"
- "Plot twist:" / "Spoiler:"
- "You already know this, but"
- "But that's another post"
- "X is a feature, not a bug"
- "Dressed up as"
- "The rest of this essay explains..."
- "Let me walk you through..."
- "In this section, we'll..."
- "As we'll see..."
- "I want to explore..."

---

## Performative Emphasis

False intimacy or manufactured sincerity:

- "creeps in"
- "I promise"
- "They exist, I promise"

---

## Telling Instead of Showing

Announcing difficulty or significance rather than demonstrating it:

- "This is genuinely hard"
- "This is what leadership actually looks like"
- "This is what X actually looks like"
- "actually matters"

---

## Vague Declaratives

Sentences that announce importance without naming the specific thing. Kill these.

- "The reasons are structural"
- "The implications are significant"
- "This is the deepest problem"
- "The stakes are high"
- "The consequences are real"

If a sentence says something is important/deep/structural without showing the specific thing, cut it or replace it with the specific thing.

---

## Second-Generation Tells

These survive the first pass because they don't appear on standard lists. They're subtler than obvious slop but produce the same distance and drift. Look for these after clearing the obvious patterns.

**Lazy connectors** — the writer didn't earn the transition:

- "This means that..."
- "This creates a situation where..."
- "This leads to..."
- "Which means..."

**Conditional filler** — sounds thoughtful, reads as stall:

- "When you X, you Y" (as an opener)
- "If you've ever X, you know Y"
- "For many people..."
- "In many ways..."

**Circling instead of landing:**

- "There's something about X that..."
- "What makes X interesting is..."
- "Part of what makes X work is..."

**Announcing the example instead of giving it:**

- "What this looks like in practice..."
- "Here's an example of that:"
- "To illustrate this point..."

**Moralizing closers:**

- "It's a reminder that..."
- "That's worth remembering."
- "That's the lesson here."

**Performative tension:**

- "And yet."
- "But here's the thing."
- "Except."
  (as standalone sentences for dramatic effect)

**Rhetorical pause before stating the obvious:**

- "The result?"
- "The answer?"
- "Why?"

**Generative rule:** These patterns exist because the model is buying time before committing to a specific claim. Any sentence that announces, circles, or pauses before the point is doing this. The fix is always the same: delete the setup and open with the claim.

---

## Opener Uniformity

Scan the first word of every sentence in the piece. If 3+ sentences open with the same word, the writing is patterned. AI defaults to "The", "This", "It", "You", "There" — rotating through a small set.

**What to look for:**

- 3+ sentences starting with "The"
- 3+ sentences starting with "This"
- Every paragraph opening with "It is" or "There is"
- Consecutive sentences starting with the same word

**Fix:** Restructure openers to start with: a name, a number, a verb, a time reference, a place, a conjunction used intentionally ("But three weeks later..."). Human writers vary entry points. The first word of a sentence is a choice — make it different each time.

---

## Semantic Repetition

The same idea appearing in different words across paragraphs. AI fills space by restating. A paragraph ends with a conclusion; the next paragraph opens by restating that conclusion as a premise.

**What to look for:**

- Last sentence of paragraph A makes a claim. First sentence of paragraph B restates it.
- The same concept appears 3+ times across the piece in different phrasing.
- A paragraph's first and last sentence say the same thing.

**Fix:** Cut one instance. The idea doesn't get stronger by repetition — it gets weaker. If the point was made in paragraph A, paragraph B starts somewhere new.

---

## Topic Sentence Pattern

Every paragraph opening with a summary of what the paragraph will say. Sounds organized. Reads as formulaic. Real writing doesn't announce itself — it moves.

**What to look for:**

- Every paragraph starts with a broad claim that the paragraph then supports.
- The first sentence of each paragraph could stand alone as a complete thought without the rest.
- Reading only first sentences tells you the whole piece — nothing is discovered mid-paragraph.

**Fix:** Start one paragraph mid-argument. Start one with a specific detail that earns the general claim by the end. Let at least one paragraph's point emerge from the evidence rather than precede it.

---

# Structures to Avoid

## Binary Contrasts

**Generative rule:** The negation exists to manufacture anticipation. The writer sets up X so the reader leans in for Y. Remove the negation and the prose has to earn attention through the idea itself. If Y can't stand alone, Y isn't strong enough.

| Pattern                                                       | Problem                        |
| ------------------------------------------------------------- | ------------------------------ |
| "Not because X. Because Y." / "Not because X, but because Y." | Telegraphed reversal           |
| "[X] isn't the problem. [Y] is."                              | Formulaic reframe              |
| "The answer isn't X. It's Y."                                 | Predictable pivot              |
| "It feels like X. It's actually Y."                           | Setup/reveal cliche            |
| "The question isn't X. It's Y."                               | Rhetorical misdirection        |
| "Not X. But Y." / "not X, it's Y" / "isn't X, it's Y"         | Mechanical contrast            |
| "It's not this. It's that."                                   | Same formula, different words  |
| "stops being X and starts being Y"                            | False transformation arc       |
| "doesn't mean X, but actually Y"                              | Negation-then-assertion crutch |
| "is about X but not Y"                                        | False distinction              |
| "not just X but also Y"                                       | Additive hedge                 |

**Fix:** State Y directly. "The problem is Y." Drop the negation entirely.

---

### Exception: Earned Narrative Contrast

Not all contrast is hollow. The rules above target contrast used as a _substitute_ for content — where the structure is the point. When contrast reveals a genuine shift in understanding, it earns its place.

**The test:** Remove the negation. Does Y still stand on its own as a real claim?

- Hollow: "Not because the tech is complex. Because people are complex." → Remove the negation: "People are complex." That's a generic assertion. Nothing was revealed. The contrast was the whole move.
- Earned: "I used to think my job was to sell houses. Now I know I'm selling peace of mind." → Remove the before: "I'm selling peace of mind." That's a real, specific reframe. The before makes it land harder, but the insight exists without it.

**What makes contrast earned:**

- The "before" contains a real prior belief the writer actually held, not a straw man set up to be knocked down
- The "after" is specific enough to stand alone — it's not just "the opposite of the before"
- The contrast reveals a shift in understanding, not just a rhetorical shape
- The writer could name the moment or experience that caused the shift

**Before/after structure in narrative writing** — showing how something changed — is a different category than binary contrast. "I used to X. Then Y happened. Now I Z." is a timeline with meaning attached. It is not the same as "Not X. It's Y." The first moves through time. The second just negates.

**Flag hollow contrast. Pass earned contrast.**

---

## Negative Listing

**Generative rule:** Listing what something is _not_ is a rhetorical striptease — the writer builds suspense through withholding. It feels clever. It reads as stall. The reader doesn't need the runway. Give them Z.

| Pattern                               | Problem                           |
| ------------------------------------- | --------------------------------- |
| "Not a X... Not a Y... A Z."          | Dramatic buildup through negation |
| "It wasn't X. It wasn't Y. It was Z." | Same structure, past tense        |

**Fix:** State Z. Cut everything before it.

---

## Dramatic Fragmentation

**Generative rule:** Fragments signal the writer believes the _presentation_ of an idea is more interesting than the idea itself. It's a substitute for substance. Complete sentences force the claim to carry its own weight.

| Pattern                                  | Problem                 |
| ---------------------------------------- | ----------------------- |
| "[Noun]. That's it. That's the [thing]." | Performative simplicity |
| "X. And Y. And Z."                       | Staccato drama          |
| "This unlocks something. [Word]."        | Artificial revelation   |

**Fix:** Complete sentences. Trust content over presentation.

---

## Rhetorical Setups

**Generative rule:** These announce insight rather than deliver it. The model is performing the _shape_ of a smart thought — the pause, the pivot, the reveal — without committing to the thought. Any sentence that tells the reader how to feel about what's coming is doing this.

| Pattern               | Problem                |
| --------------------- | ---------------------- |
| "What if [reframe]?"  | Socratic posturing     |
| "Here's what I mean:" | Redundant preview      |
| "Think about it:"     | Condescending prompt   |
| "And that's okay."    | Unnecessary permission |

**Fix:** Make the point. Let readers draw conclusions.

---

## Formulaic Constructions

| Pattern                   | Problem                     |
| ------------------------- | --------------------------- |
| "By the time X, I was Y." | Narrative template          |
| "X that isn't Y"          | Indirect. Say "X is broken" |

---

## False Agency

**Generative rule:** AI avoids naming actors because naming requires commitment. "The decision emerged" implicates nobody. "Sarah decided on Friday" implicates someone. Vague subjects feel safer. Any time an inanimate thing performs a human action, a person has been hidden. Find them.

| Pattern                         | Problem                                                           |
| ------------------------------- | ----------------------------------------------------------------- |
| "a complaint becomes a fix"     | The complaint did nothing. Someone fixed it.                      |
| "a bet lives or dies in days"   | Bets don't have lifespans. Someone kills the project or ships it. |
| "the decision emerges"          | Decisions don't emerge. Someone decides.                          |
| "the culture shifts"            | Cultures don't shift on their own. People change behavior.        |
| "the conversation moves toward" | Conversations don't move. Someone steers.                         |
| "the data tells us"             | Data sits there. Someone reads it and draws a conclusion.         |
| "the market rewards"            | Markets don't reward. Buyers pay for things.                      |

**Fix:** Name the human. "The team fixed it that week" beats "the complaint becomes a fix." If no specific person fits, use "you" to put the reader in the seat.

---

## Narrator-from-a-Distance

**Generative rule:** The model floats above the scene because specificity requires commitment to a particular vantage point. "Nobody designed this" sounds observational and wise. It's actually evasion — the writer refuses to put anyone, including the reader, in the room. Specificity collapses distance.

| Pattern                   | Problem                 |
| ------------------------- | ----------------------- |
| "Nobody designed this."   | Disembodied observation |
| "This happens because..." | Lecturer voice          |
| "This is why..."          | Same                    |
| "People tend to..."       | Armchair sociologist    |

**Fix:** Put the reader in the room. "You don't sit down one day and decide to..." beats "Nobody designed this."

---

## Passive Voice

**Generative rule:** Passive voice hides the actor and drains energy. Every sentence needs a subject doing something. The actor belongs at the front.

| Pattern                    | Fix                  |
| -------------------------- | -------------------- |
| "X was created"            | Name who created it  |
| "It is believed that"      | Name who believes it |
| "Mistakes were made"       | Name who made them   |
| "The decision was reached" | Name who decided     |

---

## Sentence Starters to Avoid

| Pattern                                                         | Fix                                             |
| --------------------------------------------------------------- | ----------------------------------------------- |
| Sentences starting with What, When, Where, Which, Who, Why, How | Restructure. Lead with the subject or the verb. |
| Paragraphs starting with "So"                                   | Start with content                              |
| Sentences starting with "Look,"                                 | Remove                                          |

Wh- openers become a crutch. "What makes this hard is..." becomes "The constraint is..." or better, name the specific constraint.

---

## Rhythm Patterns

| Pattern                        | Fix                                                 |
| ------------------------------ | --------------------------------------------------- |
| Three-item lists               | Use two items or one                                |
| Questions answered immediately | Let questions breathe or cut them                   |
| Every paragraph ends punchily  | Vary endings                                        |
| Em-dashes                      | Remove. Use commas or periods. No em dashes at all. |
| Staccato fragmentation         | Don't stack short punchy sentences                  |
| "Not always. Not perfectly."   | Hedging disguised as reassurance                    |

---

## Word Patterns

| Pattern                                                                                               | Problem                                                               |
| ----------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Lazy extremes (every, always, never, everyone, everybody, nobody)                                     | False authority. Use specifics instead of sweeping claims.            |
| All adverbs (-ly words, "really," "just," "literally," "genuinely," "honestly," "simply," "actually") | Empty emphasis. Read above "Phrases to Remove" section for full list. |
