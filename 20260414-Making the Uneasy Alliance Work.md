*Published at [https://topka.substack.com/p/making-the-uneasy-alliance-work-architectures](https://topka.substack.com/p/making-the-uneasy-alliance-work-architectures) on April 14, 2026*

---

# Making the Uneasy Alliance Work: Architectures for Two-Context AI Assistants

## Eight architectures, the winners, and a glimpse into the future

Earlier we laid out the [issues and difficulties of combining](https://topka.substack.com/p/the-uneasy-marriage-of-your-work) work and personal contexts within the AI personal assistant. 

In this article, I want to go a bit more practical and come down to listing the possible models that are worth considering for building a system with such two separate but interconnected contexts. 

I already realize that some will not be viable or will not satisfy certain interests of the sides. 

## The Interests of the Parties

We touched some of the interests when looking at conflicts, now let’s lay them all out more clearly.

**Where interests align** — both the individual and the organization want the employee to be productive at work, to grow professionally, and to have easy access to the information they need.  
**Where interests conflict** — first, the moment personal data enters a company-provided assistant, the individual's interest in protection collides with the organization's structural access to information. Then the individual (presumably) wants work-life separation. But the single-assistant model's core value proposition is unified context — the assistant is more useful precisely because it sees both domains. These are structurally opposed: the feature is the bug.  
**The gray zones** — both parties claim an interest in "employee development and growth", but they may mean different things: growth to serve company’s needs or employee’s career. The assistant accumulates rich knowledge over time with not very clear ownership of it: the boundary between "company information the employee accesses" and "the employee's personal synthesis of that information" is inherently blurry. It is similar with access to information: the boundary between "company information the employee accesses" and "the employee's personal knowledge base built on top of that information" doesn't have a clean line.  
**Active conflict** — Beyond the passive questions of data access and ownership, there is an active one: whose goals is the assistant optimizing for at any given moment? This reveals a core problem of transparency and agency leading to trust architecture problem. 

The trust collapse is a serious blocker as it leads to consequent limited sharing of personal context and makes the promise of a company-provided assistant or “single assistant for both” either useless or hopeless.

## The Liability Gap

It is also important to ask another question: who is responsible for the assistant's mistakes?

Today, the liability question is unresolved. Every major AI product disclaim liability as aggressively as possible. Organizations haven't developed policies for AI assistant errors, particularly cross-domain ones. Individuals have no leverage, no inspection rights, and no defined recourse. No regulatory framework currently addresses the specific case of an AI agent that crosses employer and personal domains. 

The accountability structure must be defined for the whole system to function. Without it, the rational individual should not trust a company-provided assistant with personal context, which circles back to the trust collapse described above.

## Possible Architectural Models

The trust and accountability problems described above already point toward separation being a more promising solution. But to understand why exactly, it helps to see the full landscape of options — including the ones that don't survive scrutiny.

What are the variables we can use to build the options to review? I can suggest these:

* Level and type of separation of the contexts  
* Who owns the assistant agent  
* The number of assistant agents

Adjusting these variables, let’s list all the models and apply the following analysis:

1. **employee's perspective**, how well the model protects the individual's interests, namely data protection, agency over the assistant's optimization function, and knowledge portability on departure,  
2. **organization's concerns**, namely how this model serves the company's interests such as data security & IP protection, compliance & audit, control over work tools and employee productivity gain, and  
3. **practical viability**, how complex, usable, and buildable this model is.

Let’s go\!

### M1: Fully unified (no separation)

*One assistant, one memory, one context, no boundaries between work and personal.*  
**Employee:** Worst case — all personal data exposed, no control over whose interests the assistant serves, no recourse on departure.  
**Organization:** Attractive — full control, maximum productivity potential, simple to manage. But holding personal data creates new regulatory exposure.  
**Viability:** Trivially buildable. This is what the market is actually shipping today.

### M2: Soft separation (policy-based rules)

*One assistant, one system, with policy-based rules that tag data as work or personal and govern what crosses the boundary.*  
**Employee:** Better than M1 but depends entirely on who writes the policies and whether they hold. Data still co-exists in one system, so protection is only as good as enforcement.  
**Organization:** Workable — retains control, can set policies, supports audit. But policy complexity grows fast and personal data still complicates compliance.  
**Viability:** Moderate complexity. Applying existing data loss prevention and classification tools to AI context is new but doable.

### M3: Hard partition (separate memory, one interface)

*One assistant interface, but two architecturally separate memory stores underneath with a user-controlled bridge between them.*  
**Employee:** Real architectural protection. But one interface still means one optimization function — the agent's loyalty is ambiguous even if the data is cleanly separated.  
**Organization:** Partial control — governs the work partition but can't see the personal side, and the user-controlled bridge is a potential leak vector.  
**Viability:** Significant engineering that nobody has built yet. User must actively manage which context they're in and this adds cognitive overhead.

### M4: User-owned assistant (granted access to employer systems)

*Individual owns and controls the assistant; employer grants it access to work tools and data.*  
**Employee:** Strongest model for the individual — full ownership, full control, knowledge stays on departure.  
**Organization:** Near-unacceptable — an uncontrolled AI agent accessing corporate data with no audit trail, no governance, no compliance frameworks, no ability to restrict or configure.  
**Viability:** Few organizations would allow BYOAI today. It is not an accepted practice and has risks.

### M5: Company-owned assistant (employee grants personal access)

*Employer owns and controls the assistant; employee optionally connects their personal data and tools.*  
**Employee:** Familiar pattern (like a company laptop) but structurally problematic — personal data enters a system the employee doesn't control, and the agent's optimization serves the employer regardless of personal extensions.  
**Organization:** Strongest model for the company — full ownership, full audit, full control over configuration and optimization.  
**Viability:** Closest to current market reality. This is essentially what Copilot, Glean and the market are evolving toward, because it's the easiest model for platform builders who already sell enterprise AI.

### M6: Two assistants, user-managed coordination

*Separate work and personal assistants in a shared user environment; user can directly instruct either and pass information between them.*  
**Employee:** Clean separation with easy bridging — both assistants live in a shared user environment, so passing information between them is low-friction while still being intentional and user-controlled.  
**Organization:** Clean and controllable — work assistant is fully org-managed, and the shared environment means some governance of cross-domain interactions is possible.  
**Viability:** Requires a shared platform or environment that hosts both assistants with clear boundaries. Doesn't exist as a designed product yet, but closer to buildable than M7.

### M7: Two assistants, AI-mediated coordination

*Separate work and personal assistants plus a third AI coordination layer that brokers cross-domain interactions and surfaces conflicts.*  
**Employee:** Best balance — real separation with intelligent bridging, and the coordination layer can implement the "surface conflicts, don't resolve them" principle.  
**Organization:** Reasonable — work assistant stays org-controlled, coordination layer is a scoped interface narrower than full access. But the coordinator is a new surface to audit and govern.  
**Viability:** The most architecturally ambitious model. Three AI systems, no standard inter-agent protocol, no product exists. Research-stage concept today.

### M8: Two assistants, complete separation

*Separate assistants in separate environments with no shared surface; human bridges only through manual effort outside both systems.*  
**Employee:** Maximum protection but maximum inconvenience — separate devices or platforms with no shared surface, like carrying a work phone and a personal phone that never touch.  
**Organization:** Perfect isolation and control. But the work assistant has zero personal context, limiting scheduling intelligence and holistic productivity gains.  
**Viability:** Trivially achievable — it's the default reality for most people today. The problem is that it's not really a "personal assistant" at all, just two separate tools.

Here are two matrices for easier overview or deeper analysis of specific aspects: 

1. [AI Personal Assistant — Models vs. Conflicts Matrix](https://html-preview.github.io/?url=https://github.com/topka/writing/blob/main/AI%20Assistant%20Models-Conflict%20Matrix.html): deeper break down of all models and aspects.  
2. [AI Personal Assistant Models — Summary Evaluation](https://html-preview.github.io/?url=https://github.com/topka/writing/blob/main/AI%20Assistant%20Models-Summary%20Matrix.html): to analyze all the options through the above three perspectives. 

## Summary

The realistic model, in my view, is the one that finds an acceptable balance across all three perspectives — not the one that maximizes any single dimension.

In this regard, there are a couple of main contenders:

1. **M3 Hard partition** — it offers a good balance, but no great result in any of the areas. The implementation of 2 separate memory storages accessible by a single agent is a complex task. I’m not aware of any ready solutions implementing this model, at least not by any of the big players.   
2. **M6 Two assistants, user-managed** — looks like the best overall to me. It is architecturally not difficult, it makes both agents informed of a conflict because they will need to cross-check with the other. Decision-making in case of conflicts remains on the user. The user is able to share data from one context to another and the org can trace it to ensure data protection.

I feel that M7 (Two assistants, AI-mediated) could be a real solution for nearly autonomous personal assistant holding independent and sometimes conflicting contexts. But for now it does not look as promising as it looked initially in my head. Unclear mediator ownership and architecture do make it not viable, yet. I’m hoping for a good solution one day.

## Looking into the Future

Worth noting — there are existing solutions for enterprise that claim to have solved the inter-agent communication of agents holding and maintaining independent contexts. The A2A protocol and adjacent frameworks and standards like DIDComm V2 (for secure messaging) and W3C Verifiable Credentials 2.0 (for data privacy) are developing fast. These standards reached "Stable" status between 2024 and 2025 and are positioned as the backbone of the "Agentic Web" in 2026\. The companies working on those solutions include OneReach.ai, Google Cloud, Salesforce and others. 

Why does it matter? The personal/work assistant problem is a specific instance of a more universal challenge: any time two AI agents representing different principals interact, they need a protocol for selective disclosure — sharing enough to collaborate while protecting information that belongs to their respective principal. If solutions for the general case exist then the blockers shift from "technical feasibility" to finding a suitable business model, building good UX, and creating a market. The technology is ready. The question is who builds the product and creates the trust for people to join.

I have a **portable, employer-subsidized assistant** business model in mind. The idea is not too complex: a provider sells personal AI assistants to individuals. When a person who already has an assistant joins a company, the two assistants — personal and work — connect via an open protocol, like any two apps integrating via API. No special fee required, each side pays for its own product. When a person who doesn't yet have an assistant joins, the employer provisions one, connects it to work systems, and subsidizes the subscription as an employee benefit — like a phone plan or a gym membership. The assistant gets smarter about work context, the employer gets a more productive employee, and the individual retains ownership. On departure, the work connection is severed — the individual keeps the assistant (and starts paying full price) or abandons it (having an option to save its memory). If kept, the assistant can be used separately for the person’s benefit or can be connected to the next employer's systems, carrying the individual's accumulated knowledge and preferences across jobs. This aligns incentives for all parties and creates a viable path to M6 or M7.

Hopefully the market demand will move the organizational and regulatory frameworks required for implementing the products and solving the liability gap.