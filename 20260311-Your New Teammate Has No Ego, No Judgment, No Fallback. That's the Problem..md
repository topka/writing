*Published at [https://substack.com/@topka/p-190617441](https://substack.com/@topka/p-190617441) on March 11, 2026*

---

# Your New Teammate Has No Ego, No Judgment, No Fallback. That's the Problem.

## *The AI-Native Org Design Problems Nobody Is Thinking About*

What’s your relationship structure with the agents you are running at work? Do you trust them? Did you consider that your coding agent can report to your manager if it sees something you did as unethical?

We use AI as a jackhammer today but it is already showing signs of being a “teammate” rather than a tool. And it’s gonna grow. 

An idea struck me recently and the result is this more philosophical than practical writeup. Nevertheless, I’m sure you can find something useful or even relevant for you, especially if you are a manager in an organization calling itself AI-native or rapidly converting into being one. I’d love to hear thoughts and feedback on any of the points or claims I make below.

Let’s go\!

What I started from were the parallels between the concepts and practices we created for working with AI, like Prompting, Context, Specification or Intent Engineering, and the classical work-, people- or project management practices. With humans you as a manager have to be able to formulate your tasks and goals clearly to get the results you were expecting. You have to provide context and resources for your team to work. You need to ensure important information is collected and stored to be accessible for the future. Quite similar, right?

Let’s outline the parallels more specifically and see what can we look at next.

## **Recognized Parallels**

| With AI | With human employees |
| :---- | :---- |
| Prompt / Context / Intent Engineering | Clear task formulation and goal-setting  |
| Interviewing & hiring | Selecting, evaluating or training LLMs and Agents for specific roles and tasks |
| System prompts & memory setup | Employee onboarding (context, culture, tools access) |
| RAG systems & knowledge bases | Knowledge management, wikis, shared documentation |
| MCP / ACP communication protocols | Team and org communication agreements and norms |
| AI evals | Performance reviews and output assessment |
| Multi-agent composition | Team composition with complementary skills |

These similarities should not come as a big surprise. We have a lot of “rails” laid out and we are using them for the new “steam locomotives” together with “horse-driven carriages”. We are in a transition period and it makes sense.

So, a number of classical approaches seem applicable when working with AIs, we just give them new names. I figured it would be interesting to fantasize about other aspects of our work and how they map and how they may or will transform with AI/agents as workers. What can be something we should expect or we can predict now?

## **Parallels Worth Reviewing**

There are several contexts in which the parallels are clear but with interesting differences or specifics that make the topic not as trivial as it may seem initially. 

### **Delegation & Trust Calibration**

The autonomy is granted gradually based on demonstrated performance. Unsupervised access to critical systems is not given on day one. 

This seems similar but there’s an important nuance: trust calibration is inseparable from feedback — every delegated task and observed result is itself a feedback loop updating your trust level, whether deliberate or not. And there are some key differences with AI: 

* trust does not transfer emotionally or generalize the way it does with humans;   
* the agent has no awareness it is being evaluated and no stake in the outcome;   
* trust is non-cumulative across sessions unless memory is explicitly maintained;

We tend to lower our guards as we get a good result, but AI can fail suddenly and confidently rather than gradually with warning signs — and it makes miscalibrated trust more dangerous.

### **Giving Feedback**

What we normally use is 1-on-1 or 360-degree feedback, performance conversations, escalation paths and so on. And this is often hard. With AI, in-session feedback works well and easy — no ego, no defensiveness. 

But there are two fundamental differences: 

1. Humans have an internal evaluative loop — they reflect on their own work, feel discomfort when output is poor, and self-correct even without external input. AI produces output and stops — there is no self-evaluation, no wondering if it was good enough. This makes the quality of the human's deliberate feedback more critical with AI than with human employees, who partially fill the gap themselves.  
2. Feedback to AI does not persist — the next session starts from zero unless the feedback was explicitly encoded into prompts or memory. With humans, feedback is absorbed and changes the person permanently. With AI, it changes the environment (the prompt, the instructions) but not the model itself. The burden of capturing and encoding what was learned falls entirely on the human managing the AI.

Interestingly, despite the differences we still come to the same conclusion: good management has always determined team quality. With AI, this dependency becomes absolute — there is no fallback.

### **Resources & Budgeting**

Both humans and AI need resources. Both have fixed and variable costs. Both humans and AI offer a range of engagement and cost models. Human-centered models — with full-time employee, contractor/freelancer, consulting firm/agency, and an outsourced function/BPO. 

AI models map closely: Subscription/SaaS with fixed fee regardless of usage, mirrors a full-time employee; API/usage-based — pay per token and per call, zero cost when idle, mirrors a freelancer; Reserved compute — fixed committed capacity plus variable on-demand, mirrors a retainer; Self-hosted/on-premise — fixed infrastructure investment, mirrors bringing a consulting team in-house. 

The parallel is more complete than it first appears. The genuinely new thing with AI is not the flexibility itself — that already exists in human engagement models — but the friction of switching between them. Switching an AI from API to enterprise subscription is more of a billing decision (clearly simplifying). Moving a human from contractor to full-time takes months of negotiation and process. While friction usually makes processes slower it also can add another level of consciousness and makes decisions stronger.

This highlights a broader principle for AI-native orgs: several apparent advantages of AI such as easier feedback, flexible costs or instant reconfiguration share this same double edge — less friction means faster movement but also less deliberate thought. Organizations may need to artificially reintroduce checkpoints precisely because the natural friction is gone.

### **Guidelines & Institutional Knowledge**

In human orgs, mistakes lead to updated guidelines, playbooks, and onboarding docs so newcomers do not repeat them. Updating an AI system prompt after a failure follows the same logic — encoding what was learned into an external artifact that future interactions inherit. 

Important specific: in a human org, guidelines supplement a person's own judgment — they read it, internalize it, and carry it forward. With AI, the guideline is the entire mechanism. There is no internalization. Remove the prompt and the lesson disappears. Human orgs externalize knowledge (if they do) as a backup for human learning; with AI, externalization is not a backup — it is the only channel that exists.

## **Something Worth Considering**

Here are some human practices that have **no** *(to my limited knowledge)* **real AI equivalents yet** — but probably need them.

### **Culture & Values Alignment**

Beyond skills matching, hiring for values fit is a critical part of human recruitment — you assess whether a person's principles and working style align with the organization before bringing them in. The AI equivalent is underserved but not unaddressed. Model providers do publish values information such as model spec or system cards and usage policies, giving organizations reference material for formal evaluation. The gap is that most orgs don't use it. Model selection is driven by capability benchmarks, cost, and speed. Values alignment is rarely a formal evaluation criterion, even though it arguably should be. 

On the technical side, the tooling for configuring values at the organizational level already exists and allows deeper behavioral customization for organizations. The real unsolved challenge is organizational, not technical: most companies have no formal process for defining their AI values configuration, no owner responsible for maintaining it as the org evolves, and no audit mechanism for verifying it is working in practice. It is treated as a one-time setup rather than a living governance artifact — the AI equivalent of writing a values statement once and never revisiting it. 

### **Intentional Capability Planning**

In human orgs, career pathing forces you to think about what capabilities you will need in the future — not just what you consume today. Plus you align with your employee’s internal motivation and goals. For AI, 'career pathing' is not about the AI growing (it doesn't have intrinsic motivation) but about:

* The organization deliberately expanding an agent's scope and responsibility based on demonstrated performance.  
* Upgrading models, allocating more compute, expanding memory and tool access as a strategic and not accidental decision.  
* A new discipline: intentional capability planning for mixed human \+ AI teams.

There’s an interesting asymmetry: with humans, capability growth is internal and requires negotiation — a two-way contract. With AI, it is an external configuration and resource decision. The organization has full control — but may get lazy about thinking ahead precisely because the friction disappears. And when this happens and teams grow uncontrollably, various managerial challenges arise sooner or later. Classical HR will not help in this case.

Important question: whose task is it to monitor and control the growth? Is it a new dedicated role? Or do we just use AI as much as we can?

### **Whistleblowing & Safe Escalation**

Employees can flag something wrong above their manager's head. AI probably needs equivalent escalation paths. There can be various possible triggers, like security or data access concerns, ethical, judgement-based or those that arise from a detected anomaly. 

An important distinction: escalation should be about the task, not the person. Flagging 'this request conflicts with policy X' is the AI equivalent of an employee saying they are not sure they are authorized — legitimate and expected.

Logging behavioral patterns or inferences about intent and making them available to management poses a risk of crossing into surveillance. The line is whether the AI is serving the user or monitoring them for someone else.

For efficiency and safety it makes sense to consider when the escalation can occur, namely before starting (analyzing the request), during execution (analyzing interim results) or before delivering results. This last moment is a deliberately designed internal evaluation loop. Interestingly, it is also the most human-like: a thoughtful employee does not just hand over finished work automatically — they consider whether anything needs flagging before it reaches the recipient. This judgment (as well as the whole escalation framework) seems to be currently missing from most AI deployments.

### **Hierarchy & Subordination**

This is really an interesting one and looks like a solid new org design problem.

In a classical org, hierarchy is the skeleton — instructions flow down, escalations flow up, and conflicts are resolved by the chain of command. Everyone knows who their primary boss is. With AI this becomes a genuinely unsolved org design problem.

Any AI deployment involves at least four principal levels:

* Model provider (Anthropic, OpenAI) — foundational values and hard limits, set at training time, non-negotiable  
* Deploying organization — operational context and policies, set via system prompt  
* Team or department — specific configurations and constraints for their use case  
* Individual user — real-time instructions and tasks

Unlike a human employee who navigates tension between levels through judgment, relationships, and intuition, an AI has no way to resolve conflicts between these levels unless a deliberate hierarchy is encoded in advance. Without it, behavior becomes inconsistent and unpredictable.

Concrete example: a user asks the AI to do something within company policy but restricted by their team's specific configuration. Which instruction wins? A human would likely know. An AI needs this resolved explicitly.

Staying within the organization, the key design questions that do not yet have standard answers: How do you encode priority when instructions conflict? How does the AI signal to a user that it cannot fulfill a request due to a higher-level constraint — without revealing what that constraint is? Who in the org owns the hierarchy design, and how is it maintained as the org evolves?

A separate question of agentic AI design is how to (if at all) introduce subordination inside multi-agent systems — specifically whether a specialized agent should defer to an orchestrator unconditionally, or maintain independent judgment and its own guardrails

This question of subordination is not a technology problem. It is an organizational design and governance problem that most orgs are not thinking about yet in my view.

### **Accountability**

In human organizations, authority and accountability are paired — if you have the power to make a decision, you own the consequences. That pairing is what makes accountability function as both a corrective and a preventive mechanism. The knowledge that you will own the outcome shapes behavior before anything goes wrong.

With AI that personal weight disappears entirely. The agent has no stake in the outcome, no reputation to protect, no career consequences. Accountability has to be carried by humans — but *which* humans gets complicated quickly because of two problems:

* Diffusion — when an AI agent acts, responsibility spreads across the person who gave the task, the person who configured the system prompt, the team that selected the model, and the org that deployed it. Diffused accountability tends to become no real accountability in practice.  
* Transparency — with a human you can ask 'why did you do that?' and get a meaningful answer. With AI, explainability is limited. It is hard to hold something accountable when you cannot fully understand its reasoning.

Designing clear accountability chains for AI actions — before something goes wrong — is as much an org design problem as hierarchy itself, and equally unsolved in most organizations.

### **Offboarding**

When you stop using an agent or model, the mechanical steps like revoking API keys, removing integrations, archiving logs, updating system prompts that referenced the retired agent — are well within the scope of existing IT and infrastructure playbooks. Orgs already have procedures for decommissioning software and AI fits them cleanly. 

One addition that standard IT offboarding does not cover however is knowledge extraction, which is closer to what you do when a knowledgeable employee leaves.

A long-running agent may have accumulated something valuable in its configuration — a carefully tuned system prompt, refined instructions, documented edge cases, learned preferences encoded over many iterations. The knowledge should be captured before the agent is retired so it does not have to be rebuilt from scratch. So, while structurally solved, it is likely not yet fully operationalized. Most orgs simply have not written the procedure yet.

## **Something Else**

I’m sure there’s more. This here is clearly not a proper research and not yet a framework, it is rather a fun exercise for a wandering mind to find interesting areas for further exploration. You can already see where I went a bit deeper, I will probably dive even further into some of these topics. 

Let me know what you felt if you finished my writeup. What resonated or troubled you most?   
I hope it’s not that *AI will steal our jobs*.