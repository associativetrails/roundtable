# Problem Solving — Disciplines Panel
**Date:** 3 June 2026
**Problem:** Fixed-fee web development projects consistently run over budget due to scope creep. Client budgets are fixed. Goal is to price better.

---

## Step 1 — Problem Reframe

**What you think the problem is:** Scope creep is eating your margin.

**What the problem might actually be:** The scope is expanding because it was never precisely enough defined to defend. A change order process that exists on paper but can't be enforced in practice is no change order process at all. The real problem is likely that you're winning projects with intentionally or inadvertently vague specifications — which clients then fill with their own expanding expectations — and you have no structural mechanism to either prevent that expansion or get paid for it.

**The assumption already baked in:** That better pricing is the fix. But if the scope is undefined at the point of pricing, pricing better is impossible — you're pricing a moving target. The upstream problem is specification, not estimation.

**The gap:** You may be solving for the wrong thing. "Pricing better" assumes you know what you're pricing. You may not.

---

## Step 2 — Diagnostic Pass

### Bernard — Historian

> "Fixed-price contracting has a very long and very consistent history of going badly for the supplier when scope is ambiguous — and it has an equally long history of the supplier accepting the arrangement anyway because it wins the work. This pattern is not new. You see it in construction, in defence procurement, in enterprise software. The client offers a fixed budget, the vendor prices to win, and then the discovery phase reveals that what was implied and what was specified were two entirely different projects.
>
> What I'd want to know is: what determined the cases where it went well? Almost uniformly, it's specificity of specification at the point of contract. The projects that stayed within budget were the ones where the scope document was detailed enough to make expansion visible and attributable. The ones that ran over had scopes written in client language — outcomes described, not deliverables defined.
>
> The question I'd ask that hasn't been asked yet is: who wrote the scope? Because in most cases I've studied, the scope was written by the person who wanted the budget approved, not the person who understood what the work required."

### Isabel — Economist

> "There's a straightforward incentive problem here. At the point of sale, both parties have an incentive to not look too closely at the scope — the client because a vague scope is easier to get budget approval for, and the developer because a vague scope is easier to price attractively. The problem is that both of those incentives produce the same outcome: a project that cannot be delivered for the agreed price.
>
> The change order process is theoretically the correction mechanism, but it only works if the client believes you will actually stop working if they don't pay. If they've learned — from you or from prior vendors — that work continues regardless, then the change order process has no teeth. It's a request mechanism, not an enforcement mechanism.
>
> The question that hasn't been asked: what happens when you say no? Not 'what happens when you ask for more money' — you've already answered that. What happens when you decline to do the additional work without additional payment? Because that's where the real incentive structure reveals itself."

### Nneka — Sociologist

> "I want to look at the power structure in this relationship, because I think it's doing more work than anyone is acknowledging. When the client says 'there isn't any more budget,' that statement is being treated as a fact about resources. But it may be a statement about power — specifically, about who in this relationship is able to set terms and who is not.
>
> The client came to you with a fixed budget. You accepted that frame. You priced to it. You then discovered that the project exceeds it. When you asked for more money, the client restated their original position. At no point in this sequence did your position as the expert — the person who knows what the work costs — carry enough weight to change the terms. That's not a pricing problem. That's a positioning problem.
>
> The question I'd ask: when did the client's budget become your constraint? Because there's a point in every sales conversation where a vendor accepts a client's budget as fixed rather than treating it as one variable in a negotiation. I'd want to understand what's happening at that moment."

### Owen — Psychologist

> "There are a couple of psychological dynamics here worth naming. The first is the planning fallacy — the well-documented tendency to underestimate the time and cost of future tasks even when we have direct experience of similar tasks going over. Fixed-fee developers are not uniquely bad at this; everyone is. The question is whether there's a structural correction built into the process, or whether you're relying on intuition each time and getting the same result.
>
> The second is something I'd call scope optimism on the client side. When clients describe what they want, they describe a plausible future in which their requirements are clear and stable. They are not lying — they genuinely believe this. But requirements that feel clear in conversation are almost never clear in implementation, and the gap between the client's mental model and what the work actually requires is where the scope creep lives.
>
> The question nobody has asked yet: do your clients know when they're changing scope? Because in my experience, a significant proportion of scope creep is not clients knowingly asking for more — it's clients asking for what they thought they already asked for. If that's happening, the problem isn't the change order process — it's that there was never a shared definition of what was in scope in the first place."

### Raj — Engineer

> "The systems framing here is pretty clear. You have a process — scoping, pricing, contracting, delivery — and it's producing a consistent failure mode. Consistent failure modes in systems are almost never random; they have a cause. The question is where in the pipeline the failure originates.
>
> My read: the failure is at the specification interface. Fixed-fee projects require a specification that is precise enough to draw a line around. 'Website for a restaurant' is not a specification. 'Five-page static site, contact form, menu PDF upload, mobile responsive, no CMS' is a specification. The difference matters enormously for pricing — and for being able to say, clearly and without awkwardness, 'that's outside the scope we defined.'
>
> What I'd also point to: change orders fail not because the process is wrong but because the original scope document wasn't tight enough to make the change legible. If the scope says 'e-commerce functionality,' and the client asks for a loyalty programme, it's genuinely ambiguous whether that's in scope. Tight specifications make changes undeniable. Vague ones make them arguable.
>
> The question I'd ask: can you point to the line in your current scope documents that would let you say, unambiguously, 'this is new work'? If not, that's the system failure."

### Sofia — Philosopher

> "I want to examine the concept of 'better pricing,' because I think it's doing more work than it can bear. Pricing better implies we know what we're pricing and the question is the number. But the panel has surfaced a prior problem: what is being priced is not well-defined. A price is a claim about the cost of a specified thing. If the thing is unspecified, the price is not undefined — it's wrong by construction.
>
> There's also a values question being smuggled in here. The goal stated is 'win projects and not work for free.' But there are two levers: don't win projects you'll lose money on, and stop losing money on projects you've won. Those are different strategies with different implications. The first requires you to walk away from work. The second requires you to change your delivery process. It matters which one you're actually after — and the panel seems to be addressing the second while the first may also be in play.
>
> The question I'd ask: is the goal to price the current type of project better, or to change what type of project you take? Because those require entirely different interventions."

---

## Step 3 — Root Cause Mapping

**Where the panel agrees:**

- The scope document is not tight enough to defend. Scope creep is happening in the gap between what was implied and what was specified.
- The change order process has no enforcement mechanism — it's a polite request that clients can decline.
- Vague specifications benefit both parties at point of sale and harm the developer at point of delivery.

**Where the panel diverges:**

- Isabel and Nneka are pointing to a power and leverage problem: the developer has accepted the client's framing (fixed budget, no more available) as a constraint rather than a negotiating position. The fix there is positional, not procedural.
- Owen is raising the possibility that clients aren't knowingly creeping scope — they're asking for what they thought was already included. That's a shared-definition failure, not a bad-faith one.
- Sofia is questioning whether "price better" is even the right goal — it may be that the category of work (fixed-fee, scope-ambiguous web projects) is itself the problem.

**Confirmed causes:**
- Scope documents are written at a level of abstraction that makes expansion invisible and indefensible
- No real enforcement mechanism behind change orders

**Suspected causes:**
- No shared written definition of what "done" means at a granular enough level
- Sales process creates pressure to agree rather than specify

**Unknowns:**
- Whether clients are knowingly creeping or genuinely believe they're asking for what was agreed
- Whether the developer's positioning allows them to walk away from or pause work when change orders are declined

---

## Step 4 — Solution Generation

### Bernard
> "The historical solution to fixed-price contract overruns is always the same: specification before pricing, not pricing before specification. Don't price from a brief — price from a defined deliverable list. If the client hasn't provided enough information to define the deliverables, that's a discovery engagement, which you charge for separately. The firms that survive fixed-fee work treat discovery as a paid phase, not a free precondition to winning the project."

**Would not do:** Accept a brief and price it the same day. That's how every overrun starts.

### Isabel
> "The enforcement mechanism needs to be real. The change order process should state, in the contract, that work on out-of-scope items does not begin until a change order is signed. Not 'will be invoiced later' — does not begin. The client needs to experience a genuine pause to understand the process has teeth. A change order process that doesn't pause work is a wishlist, not a contract."

**Would not do:** Continue working while a change order is pending. That signals the process is optional.

### Nneka
> "The positioning issue needs to be addressed in the sales conversation, not in the contract. You need to establish, before signing, that you are the expert on what the work costs and that the client's budget is a data point, not a constraint you accept unilaterally. If the budget doesn't match the scope, say so clearly and offer options: reduce scope, increase budget, or phase the work. What you don't do is absorb the gap."

**Would not do:** Price to the client's budget when you know it's insufficient. That's agreeing to work for free before you've started.

### Owen
> "Run a specification session with the client before finalising the price. Walk them through every element of the deliverable and get them to confirm in writing — even just by email — what is and isn't included. This surfaces the requirements they assumed were obvious, and creates a shared record that makes scope expansion visible to both parties. When the client later asks for something new, you can reference the session. They're less likely to feel you're being difficult — they remember the conversation."

**Would not do:** Rely on the scope document alone as a communication tool. Documents don't create shared understanding; conversations do.

### Raj
> "Build a scope specification template and use it on every project. It should define: every page or view, every user action, every integration, every content type the client is responsible for, and a clear statement of what is explicitly not included. The 'not included' list is the most important part — it's where you close the gaps that clients assume are included. Scope documents without exclusions are open-ended by default."

**Would not do:** Use the client's brief as the scope document. Their brief describes what they want; your scope document defines what you're delivering.

### Sofia
> "Before any of this: decide what kind of business you're running. Fixed-fee works if and only if you can define the deliverable precisely enough to price it accurately. If your clients consistently can't or won't specify at that level, fixed-fee is structurally unsuited to the work. You may need to move to time-and-materials for anything above a certain complexity threshold, or to a hybrid model — fixed fee for a specified core, T&M for everything else. 'Pricing better' within the current model may be optimising a flawed system."

**Would not do:** Assume the model is correct and that the solution is a better number. The model itself needs examining.

---

## Step 5 — Recommended Workflow

**Do first — highest leverage, lowest uncertainty:**
Introduce a paid discovery phase. Before pricing any project, charge for a scoping session (2–5 hours, fixed fee) to produce a detailed specification. This filters out clients who won't engage seriously, produces the document needed to price accurately, and establishes you as someone who treats their own time as valuable. Price this session so it covers your time regardless of whether the project proceeds.

**Do next — once the specification exists:**
Rewrite scope documents to include an explicit exclusions list. Every feature or element not being built should be named. Add a clause that out-of-scope work requires a signed change order before it begins — not after, before. Brief clients on this verbally at kickoff, not just in the contract.

**Hold off on:**
Renegotiating rates in isolation. Higher rates on a vague scope produce the same outcome at a higher number.

**Watch for:**
Clients who resist the discovery phase or who won't commit to a specification. That resistance is signal. A client who can't define what they want is a client who will expand scope throughout delivery. Knowing this before pricing is worth more than any pricing fix.

---

## Step 6 — Open Questions

**1. Will your current clients pay for discovery?**
The paid discovery model is the most structurally sound fix — but it requires clients who accept it. If your current client base won't, the question becomes whether to change the client base or find a different model (T&M, hybrid). This is a market question the panel can't answer.

**2. At what point do you walk away?**
The change order process only works if declining a change order can result in work stopping. Whether you're willing and able to do that — financially, contractually, relationally — determines whether the fix has teeth.

**3. Is fixed-fee the right model for the work you're doing?**
Sofia's question remains open. If your projects are routinely complex enough that scope can't be fully defined upfront, fixed-fee may be the wrong model regardless of how well you price it. That's worth examining honestly before investing in process improvements that assume the model is sound.
