Published at [https://topka.substack.com/p/delete-the-codebase-can-you-have](https://topka.substack.com/p/delete-the-codebase-can-you-have) on August 9, 2026

---

Delete the Codebase. Can You Have It Back by Friday?

The old rule of thumb was that buying software beats building it. Writing code is (was) quite slow, but that’s not what made us buy software. It was the cost of owning.

Owning \= bug fixes \+ security patches \+ platform updates \+ migrations \+ monitoring \+ support tickets from your own colleagues. A monthly SaaS fee bought you a vendor who did most of that and amortised it across all of their customers. Whereas your in-house alternative has just you as its one customer.

So, we bought.

But sometimes we still built something. And the thing we built became the only place where the full knowledge of how our business operates was encoded. In code. 

And then the markets moved, requirements changed, platforms aged. The people who wrote the code might have left or moved on. And the code, the expensive artefact that we kept trying to fix and update became the thing slowing us down.

It's like using a twenty-year-old road atlas to drive three hundred kilometres to your summer house. Points A and B haven't moved but everything between them has. Your child does not know how to read a road atlas, and your notes in the margins of worn pages just make it worse.

Nobody uses a road atlas now. The roads still change. So we stopped storing the route and started re-building it every time we drive.

## Regeneration

The frontier labs are telling us that building software is fast and cheap now. They are broadly right about the first copy and very quiet about everything after it. A [Carnegie Mellon study](https://arxiv.org/abs/2511.04427) of 806 open-source projects that adopted Cursor found the velocity gain was real but gone within two months, while static analysis warnings rose 30% and code complexity 41% — and stayed there. [LinearB's analysis](https://linearb.io/blog/8-million-prs-engineering-productivity) of 8.1 million pull requests adds the other half: AI-assisted pull requests do almost no refactoring at all. The tools write new code. They don't clean up the old. The maintenance cost does not disappear, it gets bigger faster.

And buying changes too. SaaS is repricing to monetise AI features, and lock-in bites hard in year two, after the business case has already been signed off.

But there's a move available now that wasn't available before. If generating software is fast and cheap, the answer to a high maintenance cost is regeneration rather than repair. Yes, regeneration from scratch.

But does it cover everything? Regeneration answers the cost of the code itself: the fixes, the refactors, the boring framework upgrades, the rewrite that keeps getting deferred. It does not cover the operational burden though. Your data still has to migrate. Your integrations still have downstream consumers. You still need your IT to set up monitoring and access. And your users who learned the old screens are all still there. None of it regenerate.

That's still a real shift, because the logic layer what’s causing most of the "our tools slow us down" pain. Just don't sell yourself the version where the whole problem evaporates with regeneration.

## The specification is the source

We stopped storing compiled binaries. You keep source, your CI can build the binary whenever you need it.

Regeneration does the same thing one level up. The code becomes the build artefact. The specification becomes the source.

That's the reframe. You are not choosing whether to own software. You are choosing whether to own the description of how your business works, or to rent someone else's description of it.

Here's the test. If your codebase was deleted tonight, could you have a working equivalent by Friday? If yes, you own a specification and the code was an output. If not, you own code, and you're still in 2020\.

## Which is exactly what nobody is keeping

There's a chance today's builders have their solutions well described, because they had to describe them to AI to get them built. For sophisticated agentic engineering practitioners this is true. But I don't see it as widespread yet.

The prompt history lives in a chat window that gets closed. The reasoning behind a decision sits deep in a conversation, isn't in version control and isn't in the wiki. Nobody treats a chat session as an artefact worth keeping, because it doesn't look like one. It looks like typing.

So the thing I'm calling your main asset is the thing that is thrown away by default. Organisations are accumulating software whose specification existed for about forty minutes right until the creator was happy with the result.

Shadow software makes it even worse — code built outside IT oversight, it has no spec, no owner, and no one who can tell you why it does what it does. When the person who vibed it leaves, you inherit a black box you can't regenerate, because regeneration needs a description and it has left with them.

And specs rot on their own. Someone patches production on Friday night, the fix never makes it back into the spec, and the next regeneration quietly deletes it. That's the road atlas problem again, one layer up. A specification you don't maintain becomes exactly the legacy you were trying to escape.

## If you build

1. Don't rebuild what you already bought. Build on top of it, integrate with it, and build only the parts that are specific to your business.  
2. Break it into small pieces. When you regenerate, you want to regenerate a component, not the estate.  
3. Keep the specification in version control, next to the code, reviewed like code. Not in a Slack chat, not in someone's Notion, not in the head of the person who built it.  
4. Treat spec drift as an incident. If production and the specification disagree, one of them is wrong and you need to know which before you regenerate anything.

Building was expensive because owning was expensive. Owning got cheaper for the code and stayed expensive for everything around it. The part that got valuable is the description, and almost nobody is writing it down. 

Are you writing your specs? Could you regenerate your built code by Friday?