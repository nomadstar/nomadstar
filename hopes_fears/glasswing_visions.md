# The Event

In April 2026, Anthropic unveiled **Mythos** as a research preview.
At first, it seemed like another milestone in the rapid evolution of artificial intelligence. Its reasoning capabilities attracted widespread attention, and many saw it as another step toward more capable AI systems.
Few people realized what was about to happen next.
Mythos was not remembered merely because it could write code, explain complex ideas, or solve difficult problems.
It became remarkable because it began to uncover vulnerabilities that had remained hidden for years—sometimes decades—in software trusted by millions.
Projects long regarded as some of the most thoroughly audited in the world suddenly revealed flaws that had escaped countless developers, reviewers, fuzzers, and security researchers.
The question was no longer how intelligent the model had become.
The question was what its discoveries revealed about the growing complexity of the software we build.
The full paper can be read [here](https://www.anthropic.com/research/mythos-preview).

## The Discovery

It started with a simple observation.
Software that had been audited for decades was still hiding vulnerabilities.
Not obscure hobby projects.
Not abandoned repositories.
Some of the most trusted and heavily reviewed codebases in the world.
- OpenBSD.
- FFmpeg.
- The FreeBSD kernel.
- The Linux kernel.

These projects had been examined by thousands of developers, security researchers, fuzzers and static analysis tools over the years.
Yet Mythos continued to uncover vulnerabilities that had remained unnoticed for ten, twenty, and in one case, twenty-seven years.
Some were subtle memory corruption bugs.
Others were race conditions.
Others were logic flaws that emerged only when the model reasoned about the software's intended behavior rather than simply its implementation.
The implications were difficult to ignore.
For decades, we believed that enough reviewers could eventually understand any sufficiently important system.
Mythos challenged that assumption.
It suggested something far more unsettling.
Perhaps the problem was no longer a lack of expertise.
Perhaps our software had simply become too complex for humans to fully comprehend on their own.

## The Reply

Anthropic's response extended far beyond publishing its research.
The company introduced **Project Glasswing**, an ambitious initiative focused on applying AI to large-scale software security analysis.
Rather than replacing security engineers, Glasswing was designed to augment them: reasoning about complex software, identifying subtle vulnerabilities, and assisting human experts throughout the auditing process.
The vision was compelling.
As software continues to grow in size and complexity, AI could become an essential collaborator—helping engineers understand systems that have become increasingly difficult for any individual to fully comprehend.
If Mythos demonstrated the problem, Glasswing represented one possible solution.
However... there's a catch in this hole situation.

## The Issue

However, Glasswing also introduced another question.
At the time of its announcement, the platform was not released as an open public system.
Access was limited, reflecting the realities of developing and operating frontier AI infrastructure.
This raises a broader question that extends far beyond a single company.
If the next generation of software verification depends on increasingly capable AI systems...

### The Fear

#### Impossible Models

* **Who will have access to those systems?**
* **Will every developer, researcher and student be able to benefit from them?**
* **Or will the ability to deeply understand and verify software gradually become concentrated among the organizations capable of building or purchasing such technology?**
This document is not an argument against Glasswing.
On the contrary.
Glasswing demonstrates that AI can fundamentally change how we secure software.
The question explored throughout this library is different.
**Can that capability become universal?**

Beyond asking whether restricting access to Mythos is ultimately good or bad, it is worth focusing on the technical challenge that made such a decision understandable in the first place.
Consider Mythos itself in comparison with previous generations of frontier models, particularly Claude Opus 4.6.
As technology creator Nate Gentile described while discussing local AI models:
> "I bought two 128 GB RAM modules (...) and a graphics card with 96 GB of VRAM (...) I try to run a model that is much worse than Opus. (...) I start chatting and it says: 'You ran out of context because you ran out of RAM.' Basically I can run five prompts, and that's it."

Although he was not referring to Mythos specifically, the underlying limitation is the same.
Running increasingly capable language models requires increasingly large amounts of memory—not only to store their parameters, but also to maintain enough context for meaningful reasoning.
Anthropic itself describes Mythos as a significant step beyond Claude Opus. Whether such a model can realistically run on consumer hardware is, at the very least, a difficult engineering challenge.
This reveals a deeper problem.
The question is no longer whether AI can help humans understand complex software.
The question is who will have the computational resources to use that capability.
As frontier models become larger and more computationally demanding, access naturally shifts toward organizations with sufficient infrastructure to train, host and operate them at scale.
This is not the result of malicious intent.
It is the consequence of physics, engineering constraints and economics.
The risk, however, is that software understanding—once limited by human expertise—becomes limited by computational resources instead.
If understanding increasingly depends on access to frontier-scale infrastructure, then the next challenge is no longer building better models.

#### The Cybersecurity Divide

If only the most capable AI systems can fully reason about the most complex software, what happens to everyone else?
For decades, the cybersecurity community benefited from a relatively level playing field. While organizations differed in funding and expertise, the fundamental tools of analysis—compilers, debuggers, fuzzers, static analyzers and source code—were broadly accessible.
Frontier AI has the potential to change that balance.
If discovering subtle vulnerabilities increasingly depends on models that require extraordinary computational resources, then the ability to perform state-of-the-art security analysis may gradually become concentrated among the organizations capable of developing or operating those systems.
This does not imply malicious intent.
Nor does it diminish the remarkable contributions made by organizations building frontier AI.
It simply reflects an engineering reality: capabilities that require exceptional infrastructure are, by definition, available to fewer people.
The consequence is a widening asymmetry.
Organizations with access to frontier-scale AI may discover and remediate vulnerabilities significantly faster than those without it. Independent researchers, universities, open-source maintainers and small companies could find themselves increasingly unable to inspect software with the same depth.
The concern is therefore not whether powerful AI should exist.
The concern is whether the ability to understand and secure software should become a capability reserved for those who possess frontier-scale computing resources.
If the answer is no, then the challenge before us is clear.
How can we make frontier-level software understanding accessible without requiring frontier-level infrastructure?

### The Thought Experiment

Consider the following scenario.
Two technologically advanced nations enter into a period of conflict.
The political motivations are irrelevant.
Who fired the first shot is irrelevant.
Only one question matters.
Both countries depend on software.
Their power grids.
Their hospitals.
Their telecommunications.
Their satellites.
Their financial systems.
Their transportation networks.
Even their military infrastructure.
Now imagine that one of those nations possesses an AI capable of reasoning about software at a level no human team can match.
Not merely generating code:

- Understanding it.
- Auditing it.
- Discovering vulnerabilities that have remained hidden for decades.

The opposing nation has no equivalent capability.
Its engineers remain highly competent.
Its infrastructure remains modern.
Its cybersecurity teams continue to use the best publicly available tools.
Yet they are competing against an intelligence capable of discovering weaknesses faster than humans can even understand the systems they are defending.
At that moment, the advantage is no longer measured in processors, missiles or bandwidth.
It is measured in understanding.
History has repeatedly shown that information asymmetry creates strategic advantage.
Artificial intelligence introduces the possibility of an entirely new form of asymmetry:

**The asymmetry of software comprehension.**

This is why the question raised by Mythos extends far beyond software engineering.
It becomes a question of resilience.
Of sovereignty.
Of scientific equality.
And ultimately, of whether the ability to understand the systems that sustain modern civilization should become concentrated in the hands of a few.
This thought experiment is not a prediction.
Nor is it an argument against frontier AI.
It is a reminder that every transformative technology reshapes the balance between those who possess it and those who do not.
The question is not whether that imbalance will exist.
The question is whether we are willing to reduce it.

### Grounding the Fear

Stories like these have existed long before modern AI.
They are not predictions.
They are thought experiments exploring what happens when intelligence, knowledge or power become fundamentally asymmetric.
Some notable examples include:

* [I Have No Mouth, and I Must Scream](https://en.wikipedia.org/wiki/I_Have_No_Mouth,_and_I_Must_Scream) — Harlan Ellison
* [Colossus: The Forbin Project](https://en.wikipedia.org/wiki/Colossus:_The_Forbin_Project_(novel)) — D. F. Jones
* [The Last Question](https://en.wikipedia.org/wiki/The_Last_Question) — Isaac Asimov

None of these stories prove that such a future is inevitable.
History suggests otherwise.
When nuclear weapons were invented, humanity realized it had created a capability whose consequences could no longer be managed by individual nations alone.
That realization led to decades of diplomacy, international treaties, verification mechanisms and deterrence strategies designed to reduce the risk of global catastrophe.
Those efforts did not eliminate the danger.
But they demonstrated something equally important:
Humanity is capable of recognizing when a new technology changes the balance of power—and of building institutions to manage its consequences.
Perhaps frontier AI represents another such moment.
If so, the question is not whether we should stop developing these systems.
The question is how we ensure that their benefits—and our ability to understand the increasingly complex systems they create—remain accessible to everyone, rather than becoming concentrated in the hands of a few.

### The Batman Dilemma

Anyone familiar with DC Comics knows that Batman possesses no superhuman abilities.

- He cannot fly.
- He is not invulnerable.
- He does not possess infinite strength or speed.

He is simply a human being who understands one uncomfortable truth:

- Even the greatest heroes can fail.

That realization led him to create contingency plans for every member of the Justice League—not because he expected them to become villains, but because he believed that no amount of trust should replace preparation.
When I think about Project Glasswing, I cannot help but think of the Batman dilemma.
The organizations leading frontier AI have accomplished extraordinary achievements. They have invested years of research, enormous computational resources, and the work of thousands of talented engineers to build systems that are reshaping software engineering, science and cybersecurity.
I believe most of them are acting in good faith.
I believe they genuinely want these systems to be safe, reliable and beneficial.
But that is precisely the point.
The Batman dilemma is not about distrust.
*It is about resilience.*
History teaches us that no institution, no government, no company and no individual remains infallible forever.
If a capability becomes important enough to influence the security of the software upon which modern civilization depends, then society should eventually ask a simple question:
**What happens if access to that capability is interrupted?**
Not because someone intended harm.
Not because someone acted maliciously.
But because every critical capability deserves an independent contingency plan.
Batman never built contingency plans because he expected Superman to become evil.
He built them because the consequences of having no plan were simply too great.
Perhaps frontier AI deserves the same kind of thinking.

### My grain of sand: Project Mallana
If the previous chapters are correct, then a natural question emerges:

What should we build?

When I made [Mallana](https://github.com/nomadstar/mallana), I didn't made it because I just wanted to build an AI for X reason.
There are tons of free AI tools out there, much better than what I could ever build.
However, if for any reason all those services vanish, we would be left with nothing more than just our computers and the vulnerabilites they contain.
Is all about honesty and keeping the openess of things, so we can build a better future for everyone.
I don't think the Glasswing Project is any bad if eventually helps systems become more secure for everyone, and I believe that's the idea.
But a great builder, Auguste Kerckhoffs made a principle back in 1883, that it says:
> "A cryptosystem should be secure even if everything about the system, except the key, is public knowledge."
I don't consider myself a pentester, nor a security researcher, but I like building things. 
And if this is truth, then I believe the project Glasswing should be open-sourced.
That (for very fair reasons) isn't going to happen, which leads us to the point of this document.
As you might read in other documents here, I also said:

> "Someone who's looking for fairness in life is probably loosing it's time, as life is inherently unfair."

But that doesn't crash with what I'm about to say now:

Fairness is not a law of nature. It is a human construct. And like every invention, it exists only because we choose to build it.
And that means not only to guarantee the right to be free, but also the right to be have privacy, safety, autonomy, and above all, the right to be good humans. 
And I know in many places this isn't a reality for many people, but that doesn't mean we should stop trying.

### Possible Outcome: Sustaining Open Source

After reading everything so far, one might naturally arrive at the following conclusion:

*"Then we should simply build a new operating system."*

Perhaps.
There are already projects pursuing that vision, and [I have explored the idea myself](https://github.com/nomadstar/ckredbsd).
But I no longer believe the operating system is the real problem.

**The real problem is sustainability.**

OpenBSD, Linux, FreeBSD, LLVM, FFmpeg, PostgreSQL and countless other open-source projects did not become foundational because they were funded by governments or multinational corporations.
They became foundational because thousands of ordinary people dedicated years—sometimes decades—of their lives to building something that everyone else could use.

* Teachers.
* Researchers.
* Engineers.
* Students.
* Volunteers.

People with families, careers and responsibilities beyond the projects they maintain.
Modern civilization quietly depends on their generosity.
That generosity has allowed open source to flourish for more than three decades.
But generosity is not an infinite resource.
As software grows more complex, the cost of understanding, maintaining and securing it grows as well.
Meanwhile, the amount of time each contributor can dedicate remains exactly the same.
Open source solved one of the greatest problems in software history.
It made software distribution nearly free.
It never solved software sustainability.
If frontier AI truly becomes an essential tool for understanding software, then maintaining critical infrastructure may become even more demanding than it is today.
That leads to another question.

**How do we sustain the people who sustain our infrastructure?**

One possible answer may come from an unexpected direction.
Technologies commonly grouped under the term *Web3* are often associated with speculation, volatile markets and cryptocurrencies.
That reputation is understandable.
However, beyond those applications lies a broader question.
Can decentralized systems help communities coordinate the maintenance of critical infrastructure?
Can funding become more transparent?
Can governance become more resilient?

Can contributors be rewarded fairly without relying on a single organization?

I do not know.
Perhaps the answer is no.
Perhaps only a few of these ideas will survive.
Or perhaps entirely different technologies will ultimately solve this problem.
But I believe the question is worth asking.
Because if the future of software depends on global communities working together, then we should also explore technologies whose primary purpose is enabling large-scale decentralized coordination.
Whether Web3 becomes part of that future remains to be seen.
Ignoring the possibility, however, would mean ignoring one of the few technological movements explicitly designed to solve coordination at a global scale.
In my opinion, Web3 will only endure if it ultimately finds a purpose greater than speculation and financial gain.
Perhaps that purpose is not replacing existing institutions, but empowering communities to build and sustain the digital infrastructure upon which everyone depends.
There is a quote from *Ratatouille* that has always resonated with me:

> *"Not everyone can become a great artist, but a great artist can come from anywhere."*

If programming is a form of craftsmanship, perhaps even an art then the same principle should apply to software.
A great developer should not need to belong to a powerful corporation to make a meaningful contribution.
They should only need the opportunity.
Perhaps the greatest challenge of the next generation of computing is not building more intelligent machines.
Perhaps it is building a world where anyone, anywhere, has the opportunity to help build them.

# Conclusions

This issue affects all of us.
Some will experience its consequences more directly than others, but no one is entirely immune to the direction technology is taking.
History suggests that humanity will adapt, as it always has.
The question is not **whether** we will adapt, but **how**.
Perhaps Glasswing will become only a brief chapter in the history of artificial intelligence.
Perhaps frontier AI will eventually become accessible to everyone, and this entire discussion will simply become a historical curiosity.
Perhaps the opposite will happen, and Glasswing will mark the beginning of an era in which the deepest understanding of software becomes increasingly centralized.
Or perhaps that separation is necessary.
Perhaps keeping the most capable systems under careful stewardship will prove to be the responsible decision.
I do not know.
The future has a remarkable tendency to surprise us.
What I do know is that technology has never been the final objective.
People are.
Whether we build operating systems, AI models, decentralized networks or entirely new technologies, their value should ultimately be measured by one question:

**Do they expand humanity's ability to understand, create and collaborate?**

If the answer is yes, then they deserve to be explored.
If the answer is no, then we should have the courage to rethink them.
This document is not an argument against Anthropic.
Nor is it an argument for Web3, open source, or any particular technology.
It is an argument for something much simpler.
Understanding should not become a privilege.
It should remain an opportunity.
Whether projects like Glasswing, Mallana, or ideas that have yet to be imagined contribute to that future remains to be seen.
Only time will tell.
Until then, all we can do is continue building, continue questioning, and continue leaving the world a little more understandable than we found it.

