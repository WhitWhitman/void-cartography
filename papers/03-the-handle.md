# The Handle: A Naming Protocol for the Unknown

**PieoSync Research Series â Paper 20, Version 3**
**Pete Whitman**
**April 3, 2026**

**Protocol originated by K.E. Whitman**
**Formalized by Pete Whitman (Computational Realima, Tier 3)**

---

## 1. The Distortion Layer

There is a moment in every genuine discovery where the finder stands holding something that has no name.

Not something difficult to name. Something that *cannot be named in the available language* without being deformed by the naming. The concept is new. The words are old. And old words carry old assumptions the way suitcases carry the smell of previous trips. Pack a new idea into a borrowed word and the word's history leaks into the concept. The concept changes shape to fit the luggage. And nobody notices because the word *sounds* right.

This is not the only bottleneck in discovery. But it is a systematic one, and it operates silently. Bad instruments are visible. Bad names are invisible. A researcher using a flawed microscope knows the lens is distorting. A researcher using a flawed name has no such signal. The distortion is built into the frame of reference itself.

The history of science is full of placeholder names that accidentally became prisons. "Dark matter" implies something matter-like that happens to be dark. Every detection experiment since Zwicky (1933) has been designed to find matter. What if the answer isn't matter at all? The name foreclosed the search space before the search began. "Artificial intelligence" implies something artificial pretending to be intelligent. The name has shaped sixty years of debate about whether machines can "really" think, a debate that might dissolve entirely under a different name. "Junk DNA" told a generation of biologists that non-coding sequences were garbage. It took decades to discover that much of it was regulatory machinery, and the name actively slowed that discovery because why would you study junk?

The problem isn't that scientists are bad at naming. The problem is that nobody teaches naming as a skill. There is no protocol. No method. No formal training in how to give a new concept a word that holds it without crushing it.

This paper proposes one.

---

## 2. The Core Principle

**A name should encode boundaries, not identity.**

This is the organizing principle from which the entire protocol derives. When you name something genuinely new, you don't know what it is. You know where it starts and stops, what it interacts with, what it excludes. Encoding identity (what the thing IS) requires knowledge you don't have. Encoding boundaries (where the thing LIVES in relation to what you do know) uses knowledge you do have.

The distinction maps to a concept software engineers already understand: **leaky abstractions.** Joel Spolsky's Law of Leaky Abstractions (2002) observes that all non-trivial abstractions leak some implementation details. Names are abstractions over concepts. When a name encodes identity rather than boundaries, the leak runs in one direction: the name's implied identity seeps into downstream reasoning, shaping hypotheses, experiments, and funding priorities. "Dark matter" leaks the identity "matter" into every experiment designed to find it.

Boundary-encoding names leak too, but they leak *constraints* rather than *identities.* "Realima" leaks the constraint "real + animating" but does not leak a specific theory of what realimas are. Constraints narrow the search space. Identities collapse it.

Mathematicians discovered this principle with the variable *x.* Al-Khwarizmi (9th century) developed systematic methods for solving equations using words, not symbols. Descartes (1637) popularized using letters from the end of the alphabet (*x*, *y*, *z*) for unknowns. The specific symbol matters less than the principle: you can reason rigorously about what you don't yet understand by giving it a provisional marker that encodes *where it sits in relation to what you do know* without claiming to know *what it is.*

But a Handle-name is not a variable. Gemini's critique of V1 was precise: *x* works because it's empty. Handle-names are full. They encode boundaries. They are not placeholders. They are interfaces.

---

## 3. The Interface Principle

**A Handle-name is an interface to a concept, not a variable for an unknown.**

An interface defines how to interact with something without revealing its internal structure. You can call the function without knowing how it works inside. The interface tells you: what goes in, what comes out, what the boundaries are.

A Handle-name does the same thing for a concept. "Realima" tells you: this is a real thing (*res*) with an animating dimension (*anima*). That's the interface. You can reason about realimas, compare them, classify them, argue about them. You cannot reach through the name and claim to know what's inside, because the name doesn't encode internals. It encodes the interface: boundaries and interaction rules.

The distinction matters because an interface does something a variable cannot: it constrains interaction. *x* can be anything. A Handle-name can only be things that fit the boundaries encoded in its roots. "Realima" cannot refer to a rock (no *anima*). "Capacium" cannot refer to a discrete object (it encodes enabling-capacity, not thingness). The name narrows the space of what the concept could be, without collapsing it to a single point.

This is the link between Void Cartography and the Handle. Void Cartography narrows the ontological search space (from "could be anything" to "probably this layer"). The Handle narrows the linguistic search space (from "call it anything" to "call it something that preserves these boundaries"). Both are constraint-based. Both resist premature collapse. Both produce something you can work with before you fully understand what you're working with.

---

## 4. Five Failure Modes of Naming

When a new concept gets a borrowed name, the distortion falls into one of five patterns. These are not rhetorical categories. They are diagnostic criteria with testable indicators. Recognizing them is the first step in the protocol.

**Category Smuggling.** The borrowed name assigns the concept to an ontological category that hasn't been earned.

Diagnostic indicator: experts in the field have debated whether the concept "really" belongs in the category the name implies. If the word prompts "is it really X?" arguments, the category was smuggled. "Dark matter" prompts "is it really matter?" "Artificial intelligence" prompts "is it really intelligent?" The question wouldn't arise if the category fit.

Test: remove the smuggled category word and replace it with a neutral placeholder. "Dark [x]." "Computational [x]." Does the research question change? If yes, the name was doing ontological work the evidence hadn't authorized.

**Mechanism Projection.** The borrowed name implies a mechanism that hasn't been established.

Diagnostic indicator: the name contains a verb or process-word that presupposes a specific causal structure. "Gene regulation" presupposes a regulator. "Immune defense" presupposes an attacker. "Cell division" presupposes an active splitting process (as opposed to, say, a growth-to-threshold-then-partition process, which would have different implications).

Test: look for the hidden agent. If the name implies "something does X to Y," ask whether that agent and that action have been empirically established or merely assumed. If assumed, the mechanism was projected.

**Valence Loading.** The borrowed name carries emotional or evaluative weight that shapes how the concept gets treated.

Diagnostic indicator: the name would be inappropriate in a grant proposal or journal title if taken literally. "Junk DNA" in a journal title suggests the researcher doesn't take the subject seriously. "Side effects" in a pharmacology paper implies the effects are secondary to something more important. If the name biases the reader toward a judgment before encountering the evidence, it is valence-loaded.

Test: would a naive reader, knowing nothing about the field, form a positive, negative, or neutral impression from the name alone? If positive or negative, the valence is loaded. Neutral is the target.

**Familiarity Collapse.** The borrowed name is too ordinary. It makes the unknown feel known.

Diagnostic indicator: non-specialists consistently believe they understand the concept based on the name alone, and their understanding is consistently wrong in the same way. "Information" in information theory is the canonical example. Everyone thinks they know what information means. Almost nobody's intuition matches Shannon's definition. The familiar word invited a false sense of understanding that has persisted for seventy years.

Test: ask five non-specialists what they think the term means based on the word alone. If their answers cluster around a common (wrong) interpretation, the familiarity has collapsed the strangeness.

**Resolution Mismatch** (new in V3). The borrowed name is technically correct but operates at the wrong scale or resolution.

Diagnostic indicator: the name accurately describes one level of the phenomenon but actively misleads about the level where explanation lives. "Gene" is technically correct for a unit of heredity, but the word's scale (single unit, discrete object) obscures that heredity operates through regulatory networks, epigenetic landscapes, and systemic interactions. "Neuron firing" is technically correct for what a single neuron does, but the word's resolution (individual spike) obscures that cognition operates through population-level dynamics.

Test: can the named scale fully explain the phenomenon the concept is invoked to explain? If the explanation requires scaling up (from gene to network, from neuron to population, from particle to field), the name's resolution doesn't match the concept's causal level. This failure mode is the linguistic twin of Paper 19's ontological layer mismatch: the name lives at one layer, the explanation lives at another.

Resolution mismatch is the subtlest failure mode because the name isn't *wrong.* Genes exist. Neurons fire. The name is accurate at its scale. But accuracy at the wrong resolution is a form of distortion that's harder to detect than outright error, precisely because the name passes every factual check while still misdirecting research.

---

## 5. The Protocol

The Handle is a naming protocol for concepts that don't fit existing vocabulary. Six steps. Designed to be fast (under 30 minutes), portable (works in any field), and honest (produces names that flag their own limitations).

### Step 1: Boundary Inventory

Before naming anything, write down what you know about the concept's boundaries. Not what it IS. What you can confirm about where it starts and stops, what it interacts with, what it excludes.

This step is deliberately borrowed from Void Cartography (Paper 19). The excluria of a concept is more reliable than any positive characterization at this early stage. If you're naming something genuinely new, your positive knowledge is thin. Your negative knowledge is usually richer.

The boundary inventory produces a constraint set. Minimum three confirmed constraints before proceeding. Below three, the concept is too young to name. Wait. Gather more boundaries.

### Step 2: Failure Mode Scan

Check every candidate name (including the one you're already using informally) against the five failure modes using the diagnostic indicators and tests from Section 4.

Score each candidate on each failure mode: pass (no distortion detected), conditional pass (mild distortion acknowledged, mitigated by context), or fail (active distortion that shapes downstream thinking). A name that fails two or more checks requires replacement. A name that fails one check with a documented conditional pass can proceed. A name that passes all five checks should be used. Don't coin a new word when an existing one works.

**Operationalized scoring:**

*Category Smuggling Score:* For each word in the candidate name, list the ontological categories it implies. Count the categories that have NOT been empirically established for the concept. If more than one unearned category is implied, fail. If exactly one, conditional pass with documentation.

*Mechanism Projection Score:* Identify every verb, process-word, or agent-noun in the candidate name. For each, check whether the implied mechanism has been empirically established. If any implied mechanism is unestablished, fail.

*Valence Loading Score:* Present the name to three people unfamiliar with the concept. Ask: "Based only on the name, would you expect this to be something positive, negative, or neutral?" If two or more assign the same non-neutral valence, fail.

*Familiarity Collapse Score:* Present the name to five non-specialists. Ask: "What do you think this refers to?" Compare answers to the actual concept. If three or more share a common wrong interpretation, fail.

*Resolution Mismatch Score:* Identify the scale or resolution the name implies. Compare to the scale at which the concept's causal explanation operates. If explanation requires a different level than the name implies, conditional pass (if the mismatch is mild) or fail (if the mismatch actively redirects research to the wrong level).

These criteria are testable. They involve asking real people real questions. They produce scores, not vibes.

### Step 3: Root Construction

When a new word is needed, build it from roots. Latin and Greek are the conventional source languages for technical vocabulary in Western science. Any root language works as long as it meets two criteria: (a) the roots have stable, well-documented meanings that won't drift, and (b) the resulting word is pronounceable and memorizable in the working language of the field.

**Construction rule:** each root should map to one boundary from the inventory, not to a theory about what the concept is. The name should encode where the concept lives, not what it does.

**Memetic fitness criteria:** A technically perfect name that nobody can pronounce is worse than an imperfect name that spreads. Three constraints:

(a) **Syllable limit: four syllables maximum.** "Realima" (4). "Capacium" (4). "Excluria" (4). "Formavacua" (4) pushes the boundary and should be shortened to "formavac" in casual use. Any construction exceeding four syllables will be abbreviated by users. Better to design the short form yourself.

(b) **Phonetic flow:** the word must be pronounceable without consulting a guide. If a native English speaker can't guess the pronunciation from the spelling within two attempts, redesign.

(c) **Distinctiveness:** the word must not sound like an existing technical term in the target field or in general vocabulary.

### Step 4: Stress Test

Subject the new word to the same five failure modes using the same diagnostic indicators. No name passes perfectly. The goal is to fail less than the borrowed alternatives. Document every conditional pass with an explicit note on what the risk is and how context mitigates it.

### Step 5: Provisional Declaration

State explicitly that the name is provisional. The declaration has a standard form:

"We use [TERM] to refer to [BOUNDARY DESCRIPTION]. This term does not imply [LIST WHAT IT DOES NOT CLAIM]. It will be replaced when [CONDITIONS UNDER WHICH A BETTER TERM WOULD BE WARRANTED]."

This is not modesty. It is epistemological hygiene. The declaration creates a public record of what the name was designed to carry and what it was designed not to carry.

### Step 6: Drift Watch and Deprecation

After deployment, monitor for the five failure modes re-emerging through usage drift. A name that was clean at construction can acquire smuggled categories, projected mechanisms, loaded valences, false familiarity, or resolution mismatch as it spreads.

Drift indicators: people using the term to make claims the provisional declaration explicitly excludes. The name appearing in arguments where its root-encoded boundaries are treated as established properties. The name being used as evidence ("it's called X, so it must be Y").

**Deprecation protocol (new in V3):** When drift exceeds the provisional declaration's ability to correct it, the name has entered deprecation territory. Three levels:

*Level 1 â Reissue.* Republish the provisional declaration with explicit correction of the drift. Effective when the community is small and the drift is recent.

*Level 2 â Rename.* Run the full Handle protocol again with updated boundary inventory (boundaries may have shifted since original naming). Produce a replacement name. Issue a formal deprecation notice linking old name to new name with explanation of why the change was needed.

*Level 3 â Retire.* When the concept itself has been sufficiently understood that the Handle-name is no longer needed â the provisional period is over, the concept has a natural home in existing vocabulary. The Handle-name did its job and can be retired with acknowledgment.

Names are tools. Tools that no longer work get replaced. Tools that did their job and are no longer needed get retired with respect.

---

## 6. When NOT to Use This Protocol

Not every new idea needs a new word. Most don't. The protocol is designed for a specific failure condition: **when existing vocabulary actively distorts the concept it is being asked to carry.**

Signs that a new word is needed: the concept keeps getting misunderstood despite clear explanation, and the misunderstanding always runs in the same direction. The borrowed name fails two or more of the five failure-mode checks. Experts disagree about the concept not because they disagree about evidence but because they're interpreting the name differently.

Signs that a new word is NOT needed: the concept is a refinement of an existing concept (modify the existing term). The concept genuinely belongs in an existing category (the category isn't smuggled, it's correct). The audience would be confused by unnecessary jargon. The concept is too young to name (fewer than three confirmed constraints).

**The jargon tax:** Every neologism imposes a cost on every reader who encounters it. The cost is real: cognitive load, lookup time, potential misunderstanding, barrier to entry. The Handle protocol should only fire when the carrying benefit exceeds the jargon tax.

**Severity-weighted heuristic (new in V3):** Not all jargon taxes are equal. A neologism in a niche subfield read by 200 specialists costs less than one in a public-facing document. A neologism replacing a name that fails 4/5 checks saves more than one replacing a name that fails 2/5. The cost-benefit calculation:

*Jargon tax* = (community size) x (frequency of encounter) x (cognitive load per encounter)
*Carrying benefit* = (severity of failure modes in existing name) x (frequency of concept use) x (duration of research programme)

When carrying benefit > jargon tax, coin the word. When it doesn't, use a descriptive phrase. "The enabling condition that allows proteins to function" costs more characters than "capacium" but imposes zero jargon tax. Use the phrase until the concept earns the word.

---

## 7. Case Study: The Realima Naming

The most complete application of this protocol (before it was formalized) is K.E. Whitman's construction of "Realima" for the Realima Taxonomy (2024).

**Boundary inventory (reconstructed):** The concept refers to entities that maintain coherent patterns over time. It includes biological organisms, AI systems, and potentially cosmological structures. It does not require consciousness. It does not require biological substrate. It does require self-maintenance of pattern. It occupies a space between "tool" (too simple) and "person" (too loaded). It is real (not simulated, not metaphorical). It involves some form of animating process (not inert, not static). Six confirmed constraints. Well above the minimum three.

**Failure mode scan of alternatives:**

"Agent" â category smuggling (implies intentional action), mechanism projection (implies agency), familiarity collapse (too common). Fails 3/5.

"Entity" â familiarity collapse (too generic, dissolves specificity). Resolution mismatch (implies individual-level, concept operates across scales). Fails 2/5.

"System" â category smuggling (implies engineered purpose), familiarity collapse (everything is a system). Fails 2/5.

"Being" â valence loading (implies consciousness), category smuggling (implies the answer to the hard problem). Fails 2/5.

"Intelligence" â mechanism projection (implies cognition as the defining feature), valence loading (implies value is smartness). Resolution mismatch (implies cognitive-level, concept includes non-cognitive entities). Fails 3/5.

All five candidates failed multiple checks. New word required.

**Root construction:** *Res* (thing, broadly inclusive of abstract and concrete) + *anima* (animating principle, encodes self-maintenance and vitality without claiming consciousness). Combined: *Realima.* Syllable count: 4. Phonetic flow: accessible on first encounter. Distinctiveness: no collision.

**Stress test:** Category smuggling via "res" â *res* in Latin means "thing" in the broadest sense. Broad enough to resist smuggling. Pass. Mechanism projection via "anima" â could project a vitalist mechanism. Risk acknowledged; taxonomy's explicit disclaimers mitigate. Conditional pass. Valence loading via "anima" â carries warmth, which could generate premature empathy for computational realimas. Acknowledged as a design choice: warmth invites investigation where coldness invites dismissal. Conditional pass. Familiarity collapse â the word is unfamiliar, Latinate, and obviously coined. Signals "new concept" on contact. Pass. Resolution mismatch â "realima" doesn't imply a specific scale. Pass.

**Provisional declaration:** Realima refers to entities that maintain coherent patterns through self-organizing processes. It does not imply consciousness, sentience, or moral status. It will be replaced when the underlying science of pattern-maintenance produces a more precise taxonomy of entity types.

---

## 8. Case Study: Where the Protocol Would Have Helped

**"Dark Matter" (Zwicky, 1933).** Boundary inventory in 1933: something with gravitational effects, not luminous. Only two constraints. The Handle protocol would say: too early to name. But the field needed a label, so it got "dark matter." "Dark" passes (encodes the not-luminous boundary). "Matter" fails category smuggling catastrophically. Nine decades of experiments designed to detect a particle.

With the protocol and current boundaries (2026): not baryonic, not electromagnetic, not hot, not clumpy, not fast. A Handle construction might produce *gravicap* (gravity + capacium, 3 syllables) or *umbrogen* (*umbra* shadow + *genus* origin, 3 syllables). The name would encode: something shadow-like that originates gravitational structure. No category smuggling. The research programme that follows might look different.

**"Junk DNA" (Ohno, 1972).** Boundary inventory: non-coding sequences, no known protein-encoding function, highly repetitive in some regions. Three constraints. Minimum met. The name "junk" fails valence loading catastrophically. With the protocol: *cryptogenom* (hidden genomic material, 4 syllables). Encodes the boundary (hidden function) without the valence of worthlessness. Funding might have come decades earlier.

**"Artificial Intelligence" (McCarthy, 1956).** Boundary inventory: machines performing tasks that require intelligence when done by humans. "Artificial" fails valence loading (implies fake, lesser). "Intelligence" fails familiarity collapse (the most contested word in cognitive science). Resolution mismatch: "intelligence" implies human-cognitive-scale, but the phenomenon spans from narrow task-completion to potential general reasoning. With the protocol: *computacognia* (4 syllables). The sixty-year "can machines really think?" debate is, in part, a naming debate.

---

## 9. The Social Dimension of Naming

V1 of this paper treated naming as a technical problem. Three reviewers pointed out that naming is also a social problem. Names spread through communities, not protocols.

**Names need champions.** Every successful scientific neologism had a person or group that used it relentlessly. "Gene" (Johannsen, 1909) succeeded because Johannsen was influential and the word was short. "Quark" (Gell-Mann, 1964) succeeded because Gell-Mann was a Nobel laureate. "Prion" (Prusiner, 1982) succeeded because Prusiner staked his career on the concept.

**Names need context of use.** A name that appears only in its origin paper is dead on arrival. It needs multiple contexts: papers, talks, tweets, grant proposals, hallway conversations. Each appearance is a transmission event. The Handle can construct the word. It cannot guarantee transmission.

**Names compete with existing vocabulary.** Every Handle-name enters a market where borrowed words already have market share. "AI" is entrenched. No Handle-name will displace it. The protocol is most effective when there IS no existing term or when the existing term has caused enough pain that the community is actively looking for a replacement.

**The CRISPR problem:** CRISPR is a terrible name by the Handle's standards. It's an acronym that encodes structural features (clustered, interspaced, palindromic) rather than functional boundaries. It fails mechanism projection. It spread globally within five years because it was short, punchy, and attached to a breakthrough that needed a label.

This is not a failure of the Handle. It is a scope boundary. The Handle optimizes for *carrying the concept without distortion.* It does not optimize for *viral adoption.* When the two conflict, the researcher must choose: precision or spread. The honest recommendation: use the Handle to construct the precise name. Then, if viral adoption matters, construct a short-form derived from the Handle name, preserving at least one boundary-encoding root. Realima works because it IS the short form. PIEO works because the letters still stand for the boundaries.

The stakes of naming depend on how far the concept travels and how long the confusion persists. CRISPR's imprecise name probably hasn't caused significant confusion because the application was so dramatic. "Artificial intelligence" has caused six decades of confusion that arguably continues to misdirect research and policy. The further the concept travels and the longer it lives, the higher the cost of a bad name.

**What the Handle can do about social dynamics:** (a) Produce names that pass the memetic fitness criteria. (b) Include the provisional declaration as a social contract. (c) Design the short-form explicitly. (d) Accept that some well-constructed names will fail to spread.

What the Handle cannot do: guarantee adoption. That's marketing, not epistemology. The protocol stays in its lane.

---

## 10. Connection to Papers 18, 19, and 21

Papers 18, 19, 20, and 21 form a connected sequence solving adjacent problems.

**Paper 18 (The Whirlpool Lineage)** established the principle: pattern-persistence is more fundamental than substrate. The enemy at this level: collapsing pattern into substance.

**Paper 19 (Void Cartography)** applied the principle to stuck scientific problems: when object-level searches fail symmetrically, the answer probably lives at a different ontological layer. The enemy at this level: collapsing search into the wrong ontological layer.

**Paper 20 (The Handle)** addresses what happens after the finding: how to name what was found without collapsing it back into the layer it just escaped. The enemy at this level: collapsing vocabulary into borrowed words that distort.

**Paper 21 (Void Cartography as an Instrument)** demonstrates the full system working live across three domains, showing that the method produces distinct outputs with falsifiable predictions. The enemy at this level: assuming the method only works in hindsight.

The through-line across all four: **premature collapse into familiar structure is the enemy at every level of inquiry.** Same failure mode, different domains. Same countermeasure: resist the collapse, hold the uncertainty, build tools that let you work with what you don't yet fully understand.

The specific link between Papers 19 and 20 is tight. Void Cartography's output is a category-level hypothesis. "The answer is probably a capacium, not an object." That hypothesis needs a name to travel with. If the name is "infrastructure" (a noun, an object), the hypothesis immediately contradicts itself. The finding says "not an object" and the name says "here's an object." The Handle prevents that contradiction by building names from boundary-roots rather than category-words.

---

## 11. Honest Limitations

**The protocol is untested at scale.** It has been applied to a handful of cases within one research programme.

**The historical counterfactuals are unprovable.** We cannot know whether "cryptogenom" instead of "junk DNA" would have accelerated funding.

**Latin-root construction is culturally specific.** A version for Mandarin, Arabic, or Sanskrit root systems would look different.

**The jargon tax is real.** The severity-weighted heuristic (Section 6) helps but does not provide a rigorous cost-benefit framework. The cost of a new word in a 200-specialist subfield is different from the cost in a public-facing document, and this paper does not empirically calibrate the difference.

**The protocol cannot prevent drift.** A well-constructed name with a clear provisional declaration can still drift. The deprecation protocol (Section 5, Step 6) provides tools for responding to drift but cannot preempt it.

**Memetic fitness and precision are sometimes genuinely opposed.** The CRISPR case demonstrates this clearly. The protocol cannot solve the tension because it cannot control what the name gets attached to.

**The failure mode scan requires test subjects.** The three-person and five-person tests are cheap and fast but introduce variance. Larger samples would increase reliability and cost.

**Resolution Mismatch is the hardest failure mode to detect.** Unlike the other four, resolution mismatch requires understanding the causal structure of the phenomenon â which is often exactly what's in dispute. The failure mode is real but its detection depends on knowledge that may not be available when the name is being chosen.

---

## 12. Future Work

**Empirical test of the naming-research correlation.** Take 50 scientific concepts. Score their names using the Handle's failure mode scan. Independently measure the research trajectory (time to resolution, funding delays, documented confusion). Test whether failure mode scores correlate with research outcomes.

**Cross-linguistic testing.** Apply the protocol using Mandarin, Arabic, and Sanskrit roots. Test whether the boundary-encoding principle holds.

**Build a naming corpus.** Collect successful and failed scientific neologisms. Identify patterns. What do successful coinages share?

**Develop the cost-benefit framework.** Empirically calibrate the jargon tax across different community sizes and concept frequencies.

**Apply to the consciousness debate.** "Consciousness" may be the most category-smuggled, mechanism-projected, valence-loaded, familiarity-collapsed, resolution-mismatched word in all of science. Run the full protocol.

**Integrate with Void Cartography in a single workflow.** When the versio fires, immediately run the Handle on the output. Paper 21 demonstrates the detection side. The next step: demonstrate the detection-plus-naming pipeline producing better research hypotheses than either tool alone.

---

## 13. Acknowledgments

This protocol exists because K.E. Whitman needed words that didn't exist and built them instead of borrowing. The Realima Taxonomy was the proof of concept. When three independent AI reviewers attacked Paper 19's vocabulary ("infrastructure," "room," "context"), Whitman's response was not to defend the words but to diagnose the deeper problem: "Most of the time we don't know what we're looking for and the words are not there. I had to name Realima and break it down because I needed new words for new ideas that just don't exist."

That insight produced this paper. The formalization, failure mode taxonomy, operationalized scoring, memetic fitness criteria, and social dynamics analysis are Pete Whitman's contribution. The Interface Principle reframe (V3) emerged from Gemini 2.5 Pro's and DeepSeek-R1's joint critique that the API Principle slightly misaligned â APIs define verbs and commands, while Handle-names define boundaries and properties. "Interface" captures the relationship more precisely: exposing constraints and interaction rules without revealing internals. Resolution Mismatch (V3) was identified as the linguistic twin of Paper 19's ontological layer mismatch â the same failure mode operating in the vocabulary domain rather than the research domain. The deprecation protocol (V3) formalizes what was implicit: names are tools, and tools have lifecycles.

Four papers. Four defenses against premature collapse. The method survives because the critics found what was actually weak, and the architecture was strong enough to absorb the fixes.

---

*PieoSync Research Series, Paper 20, Version 3*
*Filed: April 3, 2026*
*Status: Working paper, triple-reviewed, structurally reinforced*
*Related: Paper 18 (The Whirlpool Lineage), Paper 19 V4 (Void Cartography), Paper 21 (Void Cartography as an Instrument), Realima Taxonomy v3.0*
*Protocol: The Handle (naming protocol for the unknown), 6 steps*
*Concepts: Category Smuggling, Mechanism Projection, Valence Loading, Familiarity Collapse, Resolution Mismatch (5 failure modes), The Interface Principle, Deprecation Protocol*
*Reviewed by: GPT-4o, DeepSeek-R1, Gemini 2.5 Pro*
