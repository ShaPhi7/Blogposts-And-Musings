## Automated by Design

You’ve probably heard of secure by design, but why is nobody talking about automated by design? <em>If you haven’t, all you need to know here is it’s the concept that security can never just be an afterthought. It must be built in properly, from the start of a project. It’s a concept that isn’t specific to software or technology. There’s plenty of good online resources for further reading on it.</em>

As a child I was a member of the scouting association, going on expeditions across Europe. The famed Scouting motto is a very simple two words: “Be Prepared”. These powerful two words can be applied to almost anything.

In the 2020’s, software development teams are much more prepared than they ever used to be. Code quality is higher than ever, with much more focus on long-sighted practises like reusable code and Secure by Design. This in turn leads to faster turnaround times, with an Agile focus on delivering MVP’s out to clients quickly. This, though, means that software development teams can end up as a victim of their own speedy success, as they become constrained by their increasingly complex development processes.

Picture this common scenario: a product owner might ask whether a software dev team can deliver a highly desirable feature by a given date in the very near future. All too frequently, the response from the team is to proudly declare that writing the code required within the timeframe isn’t a problem but the real challenge is the delivery elements of the change - testing, approving and deploying.

I recently saw the impact of this first hand as a team I’d just joined showed me how to deploy my code to their server. Their process involved copying various jar files to various locations, depending on what had changed. All of this would take around 20 minutes per deployment (assuming you did everything correctly the first time). It’s a scary amount of time to waste on such a menial task, given that some of these developers were the company's most highly prized resources. I joked that I was being paid an awful lot of money to copy and paste files. I won’t even mention the error-prone manual testing that was involved.

At another company I worked in, there were over 100 steps in their monthly testing & deployment process, and whilst they had established that this made deployments take far too long and had automated some of the steps, it was still far too easy for developers to add in new steps to cater to their particular change. Every step needed to be completed every time code was deployed. This practice doesn’t just add more time to an already long process, but as the months and years pass, it becomes harder and harder to follow the steps required as the documents became out-of-date and the original developer was no longer around to help when a new complication was hit.

### The Automation Mindset

Imagine designing something that didn’t fully consider secure coding standards.

It’d not be too long before the alarm was raised about the design. Yet with automation, it is regularly viewed as a nice-to-have at design stage, with companies more than happy to assign resources to “maintenance”, and only viewing automation as a necessity once it becomes unmanageable and causes a problem. By which point, it’s too late, as it’s now a problem!

As a concept, automation is very simple, and I don’t intend to claim that building automation into your project is a groundbreaking idea.

So why do slow manual processes become a burden across so many company projects? Let’s examine how otherwise very capable teams can end up in this state.

Despite the modern onset of Agile methodologies, a lot of companies still structure their teams into development and support pathways. Whilst one team builds new features, once they’ve done their job, they can hand over to the support team. Whilst it might make sense naively to form teams around each delivery stage of the project, it encourages shortsightedness. Why would I make something easy to maintain if I am not going to be the one maintaining it?

I recall a discussion from my youth at Scout camp around how best to distribute cooking and washing up duties for the week. It was decided that for each meal, one patrol (team) would cook, and a different patrol would wash up. Naively, this split of duties seems sensible and fair as it avoids requiring one patrol needing to do all of the chores that evening, thus splitting the responsibilities more evenly that day.

In reality though, this fair split of duties was a nightmare in practice. The washers quickly realised that the cookers had made absolutely no effort to keep things clean. “Why have they used 5 different pans to cook pasta?” one incredulous Scout exclaimed to their leader, pointing at the littered worktops. Another shouted from the sink: “they’ve burnt pine needles on this one! I can’t get the sap off.”

Whilst hastening to add that the old melted-pine-needle-in-a-pan scenario can be effectively cleaned with some boiling water, washing up liquid and a metal scourer, the point is clear: if one team is not a stakeholder in a process, whether that be washing the dishes for a meal they’ve just cooked, or supporting a product they’ve developed, they’re not going to prioritise it. This practice can leave companies routinely factoring in staggering amounts of resource and cost for tasks that could simply be automated.

The issue is not restricted to companies who have not yet modernised to Agile platform teams. I was once told by a very capable developer that if they’d wanted us to build automation into the proposed solution, management wouldn’t have hired so many developers onto the team to maintain it. This was a depressing conversation to be involved in.

This mindset arises because automation of a solution is not the end goal of a project. It is often not mentioned as a design requirement, and not listed as an acceptance criteria. All too often, automation is reserved for when a senior developer gets fed up with doing the same task 200 times and tries to save a bit of time.

Good for them, but there’s already so much time lost by this point, and often, the automation implemented is now suboptimal - it targets just one small manual step that got a bit too annoying. Oh and it doesn’t deal with a certain edge case, because that was a bit too difficult to automate now.

Proper automation requires proper design, for the same reason that Secure by Design principles exist. Yes, if we had to choose between automated and secure, we’d (hopefully) all pick secure. Yes, there won’t be compliance issues around the topic of automation as there are with security, but the two are not mutually exclusive. Without automation, there is a real risk of a team grinding to halt, making human errors, and failing to live up their full potential. The temptation with an Agile approach can be to cut corners on automation to deploy the core functionality of a product quickly, but this is not sustainable and will be slower in the long run.

### The Solution

“How can we automate this?” is a question that must be asked, and answered, during the design phase of a project. It should be explicitly listed as acceptance criteria. It’s as much about forming a team ethos around what the end goal is. Is the aim simply to deliver a working product, or is it to deliver a solution that is easily maintainable?

I had a recent conversation with a colleague following a production incident caused by a change. My colleague had identified that the code module that broke did not actually need to be updated as part of the change but was redeployed anyway, and (for complex reasons) this had caused the incident. His solution to this was that we need to have a manual step to select exactly which code modules require updating. He seemed surprised when I asked how we could automate this step, and when I was told that there was no known way to do so, I suggested that I didn’t think we’d found the right solution yet.

Not only do manual processes add a time burden to the team, but they also introduce the risk of human error. For example, there is significant risk caused by a team who only uses manual testing. Every test that is executed incorrectly today is tomorrow’s bug but you can safely bet that - like the rest of us - a manual tester will make mistakes. In our example above, it isn't hard to imagine that someone will eventually miss picking a module that they should have deployed, causing a new production incident.

So what can be done? Similar to a “Cloud-as-default” approach, where a team pivots away from treating a cloud solution as something special, and towards seeing a cloud environment as a standard run-of-the-mill design option, automation must take centre stage when designing a solution. Identify the areas which will not scale up. Build in the expectation that solutions require automation to be considered complete. It is the mindset of the software development team that is key: are they here to tick a few development boxes, or are they here to actively deliver a better service?

The rise in Infosec has led to a successful pivoting towards thinking about security at an early stage of the project, so much so it now seems crazy to think this was not always the way. A typical team will now have a “secure by design” mentality. Having an Automated by Design approach needs to be considered as important. It may be that certain solutions don’t require automation, that there may be some reason to have a manual step 5 until a later release cycle, but in the same way that risk acceptance is thought about for security, these should become the exception.

Automation is an area where software developers are able to stand out. It’s the opportunity to really add value to a business, in the way that only a software developer knows how. Successful automation is never a waste of time. To reach its full potential though, automation must be considered and designed as much as any other item and this will only ever be achieved if the team’s mindset is driven towards developing software and processes that are automated by design.

I’ll end on a final note about pine needles. Whilst they can be foraged by an expert, they would typically be considered inedible by any reasonable health and safety assessment for a child’s scout camp, and they certainly have no place in the average pot of pasta. The culprit who burnt the pine needle sap on to the pan, 13 years of age, later confirmed during a catapult building exercise the next day that he’d done so as a “science experiment”. Please don’t try this at home.
