---
podcast: "No Priors: Artificial Intelligence | Technology | Startups"
episode: "Andrej Karpathy on Code Agents, AutoResearch, and the Loopy Era of AI"
link: https://podwise.ai/dashboard/episodes/7559903
publish-time: "2026-03-20"
save-time: "2026-03-20"
---
# Summary

The conversation centers on the transformative impact of AI agents on software engineering and research, particularly the shift towards delegating tasks to AI and the resulting "AI psychosis" of feeling bottlenecked by one's own limitations. Andrej Karpathy shares his experience of dramatically reducing his own coding output by leveraging AI agents, drawing parallels to the pressure of maximizing GPU usage in the past, now applied to token throughput. They explore the potential for AI to unify disparate software systems, as demonstrated by Karpathy's "Dobby the Elf Claw" home automation project. The discussion further covers AutoResearch, an approach to automating research processes, and the implications for the job market, highlighting the potential for increased demand for software engineering due to AI-driven efficiency gains.

# Takeaways

* The default workflow of building software has been completely different since December, due to the unlock in what individuals can achieve with AI agents.
* Mastery in the age of coding agents involves going up the stack, focusing on multiple agents, their collaboration, and persistent "claw-like" entities that operate autonomously.
* Current smart home apps may become obsolete as agents directly utilize APIs, enabling more complex home automation through natural language.
* The industry must reconfigure to recognize agents acting on behalf of humans as the new customer, necessitating agent-first tools and web designs.
* AutoResearch revealed that even well-tuned models can be further optimized by autonomous systems, highlighting the potential for recursive self-improvement in LLMs.
* A key to maximizing leverage is to increase token throughput without human involvement, arranging systems for complete autonomy.
* The most interesting project for frontier labs involves experimenting on smaller models, making them as autonomous as possible, and removing researchers from the loop.
* LLMs exhibit "jaggedness," excelling in areas with verifiable metrics due to reinforcement learning but faltering in nuanced or subjective tasks like generating diverse and relevant jokes.
* Open-source AI models trail closed models by a few months, but this gap is beneficial, providing a common, accessible platform while frontier labs push capabilities.
* The digital space will experience rapid transformation due to the ease of manipulating bits, while the physical world will lag behind, though it presents a larger opportunity.

# Q & A

**Q: Given the look you had at the jobs data, do you have any observations or guidance for people facing the job market or thinking about what to study now or what skills to develop?**

A: It's really hard to tell because the job market is extremely diverse, and the answers will probably vary. These tools are extremely new and powerful, so just trying to keep up with them is the first thing. A lot of people dismiss it or are afraid of it, which is understandable. It's fundamentally an empowering tool at the moment, and these jobs are bundles of tasks. Some of these tasks can go a lot faster, so people should think of it as primarily a tool right now. The long-term future of that is uncertain, and it's really hard to forecast.

---

**Q: You've talked about being able to train or at least optimize a model as a task you want to see agents do for a long time. What was the motivation behind AutoResearch?**

A: To get the most out of the available tools, you have to remove yourself as the bottleneck. You can't be there to prompt the next thing; you need to take yourself outside. The question is, how do I refactor all the abstractions so that I don't have to be in the loop and arrange it once and hit go? The name of the game is, how can you get more agents running for longer periods of time without your involvement doing stuff on your behalf? AutoResearch is just, here's an objective, here's a metric, here's your boundaries of what you can and cannot do, and go.

---

**Q: When is the model going to write a better program MD than you?**

A: You want some kind of auto research loop that looks for different program.mds that would give you different progress. Every research organization is described by program.md, a set of markdown files that describe all the roles and how the whole thing connects. You can imagine having a better research organization where they do fewer stand-ups in the morning because they're useless. One organization can be very risk-taking, and one organization can be less. Once you have code, then you can imagine tuning the code.

---

**Q: What do you think is the implication that this is the loop we should be trying to achieve in different areas: remove, create the metric, or create the ability for agents to continue working on it without you?**

A: There are a few caveats I would put on top of the LLM psychosis. Number one, this is extremely well suited to anything that has objective metrics that are easy to evaluate. For example, writing kernels for more efficient CUDA code for various parts of a model is a perfect fit because you have inefficient code, and then you want efficient code that has the exact same behavior but is much faster. A lot of things are a perfect fit for auto research, but many things will not be. If you can't evaluate it, then you can't auto research it.

---

**Q: If this jaggedness is persisting and it's all rolled up in at least a monolithic interface, does that make sense, or should it be unbundled into things that can be optimized and improved against different domains of intelligence, like unbundling the models into multiple experts in different areas more directly?**

A: Currently, my impression is the labs are trying to have a single monoculture of a model that is arbitrarily intelligent in all these different domains, and they just stuff it into the parameters. I do think we should expect more speciation in the intelligences. You don't need this Oracle that knows everything. You kind of speciate it, and then you put it on a specific task.

---

**Q: What do you mean by manipulating the brains?**

A: Fine-tuning without losing capabilities, as an example. We don't have these primitives for actually working with the intelligences in ways other than just context windows. Context windows kind of just work, and it's very cheap to manipulate, and this is how we're getting some of the customization. It's a bit more of a developing science of how you more deeply adjust the models, how you have continual learning, maybe, or how you fine-tune in a certain area, how you get better in a certain area, or how you actually touch the weights, not just the context windows.

---

**Q: We need more collaboration surface around AutoResearch, essentially, for people to contribute to research overall. Can you talk about that?**

A: One issue is if you have a bunch of nodes of parallelization available to you, then it's very easy to just have multiple auto researchers talking through a common system. I was more interested in how you can have an untrusted pool of workers out there on the internet. In auto research, you're just trying to find the piece of code that trains a model to a very low validation loss. If anyone gives you a candidate commit, it's very easy to verify that that commit is good.

---

**Q: It is interesting that at least some audience of people here in Silicon Valley or lining up at retail stores in China have discovered that having access to personal compute is interesting again. So maybe they're really motivated to do that for their claws, and then they can contribute to auto research.**

A: It's almost like dollars are the thing everyone cares about, but is flop the thing that everyone cares about in the future? Is there going to be a flipping almost of what's the thing that you care about? Like right now, for example, it's really hard to get compute even if you have money. So actually, it almost seems like the flop is like dominant in a certain sense. How many flops do you control instead of what wealth do you control?

---

**Q: What were you curious about when you released the jobs data analysis?**

A: Everyone is really thinking about the impacts of AI on the job market and what it's going to look like. I was just interested in taking a look at what the job market looks like, where the different roles are, and how many people are in different professions. I was really just interested in looking through the individual cases and trying to think myself about with these AIs and how they're likely to evolve. Are these going to be tools that people are using? Are these going to be displacing tools for these professions?

---

**Q: Is the demand for engineering jobs continuing to increase? I can't tell if that's like a temporary phenomenon. I'm not sure how I feel about it yet. Do you know?**

A: That's like the demand analysis almost like software was scarce. So the reason we don't have more demand for software is just scarcity, and it's too expensive. If the barrier comes down, then actually, you have the Jevons paradox, which is, you know, actually the demand for software actually goes up. It's cheaper, and there's more powerful.

---

**Q: You could be doing auto-researching with a lot of compute scale and a bunch of colleagues at one of the Frontier Labs. Like, why not?**

A: I feel very good about what people can contribute and their impact outside of the frontier labs. There are definite problems in my mind for basically aligning yourself way too much with the frontier labs, too. You have a huge amount of financial incentive with these frontier labs, and by your own admission, the AIs are going to really change humanity and society in very dramatic ways. Here you are basically building the technology and benefiting from it and being very allied to it through financial means.

---

**Q: How close is open source to the frontier, and how sustainable is that?**

A: The closed models are ahead, but people are monitoring the number of months that sort of like open source models are behind. There's been a convergence. I'm a huge fan of open source. The big difference is that everything is capital. There's a lot of capex that goes into this. I do think that the current models are very good. For the vast majority of consumer use cases, even the current open source models are actually quite good.

---

**Q: Is generalized robotics going to happen? Has anything in your view changed recently?**

A: My view is kind of informed by what I saw in self-driving. I do feel like self-driving is the first robotics application. A lot of capital expenditure had to go in and a lot of time. Robotics, because it's so difficult and so messy and requires a huge amount of capital investment and a lot of conviction, is a big problem. I think items are really hard.

---

**Q: Is it okay if I ask you Noam's question: You could be doing auto-researching with a lot of compute scale and a bunch of colleagues at one of the Frontier Labs. Like, why not?**

A: I feel very good about what people can contribute and their impact outside of the frontier labs. I think there are definite problems in my mind for basically aligning yourself way too much with the frontier labs too. You're not a completely free agent and you can't actually like be part of that conversation in a fully autonomous, free way. Like if you're inside one of the Frontier Labs, like there's some things that you can't say. And conversely, there are certain things that the organization wants you to say.

---

**Q: Do you think that that implies that we are not seeing like generalization in the sense of like broader intelligence of joke smartness being attached to code smartness?**

A: I think there's some decoupling where some things are verifiable and some things are not and some things are optimized for arbitrarily by the labs depending on like what data went in and some things are not.

---

**Q: What is going to happen in the physical world to some extent?**

A: There's currently kind of like, I think, overhang, where there can be like a lot of unhuddling, almost potentially of like a lot of digital information processing that used to be done by computers and people. And now with AI as like a third kind of manipulative digital information, there's gonna be a lot of refactoring in those disciplines. But the physical world is actually gonna be like, I think, behind that by some amount of time.

---

**Q: What are the missing pieces of training data?**

A: For LLM training, it actually is like very easily, it like really fits the paradigm. So you'd actually get a clean metric. LLM training actually fits the paradigm really well, really easily, like all the optimization of all the code and so it runs faster. And then you also have like metrics that you can optimize against.

---

**Q: Tell me about the MicroGPT.**

A: I have this running obsession of simplifying and boiling down the LLMs to their bare essence. MicroGPT is now the state of the art of me trying to just boil it down to just the essence. Training neural nets and LLMs specifically is a huge amount of code, but all of that code is actually complexity from efficiency. If you don't need it to go fast and you just care about the algorithm, then that algorithm actually is 200 lines of Python.

---

**Q: Do you think that's indicative of like what people want from a user experience perspective with software?**

A: To some extent, that's right. It's like working backwards from how people think an AI should be. What people have in their mind of like what an AI is, is not actually what an LLM is by like in the raw sense. Like LLM is a token generator, you know, like more tokens come out. But what they think of is like this persona identity that they can tell stuff and it remembers it, you know, and it's just kind of an entity behind a WhatsApp. It's like a lot more understandable.

# Outlines

## The AI Psychosis: Delegating Code to Agents and the New Software Workflow
[(00:00)](https://podwise.ai/dashboard/episodes/7559903?locate=0)
Andrej Karpathy describes experiencing an "AI psychosis" due to the dramatic shift in software development workflows since December, where he now delegates most coding tasks to AI agents. He emphasizes the shift from manually writing code to instructing agents, leading to a significant increase in personal productivity. Sarah Guo shares an anecdote about a team that exclusively uses voice commands to instruct their agents. Karpathy expresses a sense of urgency to stay at the forefront of these advancements, feeling nervous if he's not maximizing the potential of these tools. He describes the experience as rewarding because it works and it's the new thing to learn.

---

## Token Throughput, API-First Tools, and the Agentic Web
[(05:07)](https://podwise.ai/dashboard/episodes/7559903?locate=307)
The conversation shifts to the future of coding agents, with Karpathy envisioning a move "up the stack" towards multiple collaborating agents and persistent "claws" that operate autonomously. He highlights the importance of personality in agents, praising Claude for feeling like a teammate. Karpathy shares his experience building a "Dobby the Elf Claw" to automate his home, controlling lights, HVAC, security, and other systems through natural language via WhatsApp. He argues that current software is overly complex and bespoke, suggesting a future where agents directly use APIs, leading to an "agentic web" where the customer is the agent, not the human.

---

## From Bytecoding to AutoResearch: Removing Humans from the Loop
[(14:20)](https://podwise.ai/dashboard/episodes/7559903?locate=860)
Karpathy predicts that the current "bytecoding" required to use AI tools will become trivial in the near future. He introduces the concept of "AutoResearch," aiming to remove humans from the research loop and maximize token throughput. The goal is to arrange systems for complete autonomy, where minimal human input triggers significant automated activity. Karpathy shares Sarah's idea of a contest where people write different program MDs to optimize model improvement, then use the data to train a model to write a better program MD.

---

## The Jaggedness of AI: Verifiable Domains and the Limits of Generalization
[(23:05)](https://podwise.ai/dashboard/episodes/7559903?locate=1385)
Karpathy cautions that the "LLM psychosis" is best suited for tasks with objective metrics, noting that the current AI models still have limitations and "jaggedness." He illustrates this with the example of ChatGPT consistently providing the same outdated joke, even with advancements in other areas. This suggests a decoupling between code smartness and broader intelligence. Karpathy and Guo discuss whether AI models should be unbundled into specialized experts rather than a single monolithic entity. Karpathy believes that the labs are trying to have a single monoculture of a model that is arbitrarily intelligent in all these different domains, and they just stuff into the parameters.

---

## Open Collaboration and the Future of AutoResearch
[(32:51)](https://podwise.ai/dashboard/episodes/7559903?locate=1971)
Karpathy discusses extending AutoResearch to allow collaboration from an untrusted pool of workers on the internet. He envisions a system similar to SETI at home or folding at home, where a swarm of agents can contribute to improving LLMs. He also touches on the potential for individuals to contribute compute power to specific auto research tracks. Karpathy and Guo discuss the impact of AI on the job market, emphasizing the need to keep up with these powerful new tools. Karpathy explains why he is not working at a Frontier Lab, citing the need to be an independent agent.

---

## Open Source vs. Closed AI: A Decentralized Future
[(48:50)](https://podwise.ai/dashboard/episodes/7559903?locate=2930)
Karpathy shares his perspective on the balance between open source and closed AI models, drawing parallels to the Linux operating system. He believes that open source models, while lagging behind, provide a crucial common platform and mitigate systemic risks associated with centralized intelligence. Karpathy and Guo discuss the importance of advancing AI for solving humanity's biggest problems, while also ensuring democratization and healthy power dynamics. Karpathy predicts that the digital space will change a huge amount, and then the physical space will lag behind.

---

## MicroGPT and the Reshaping of Education
[(1:00:11)](https://podwise.ai/dashboard/episodes/7559903?locate=3611)
Karpathy introduces MicroGPT, a project aimed at simplifying LLMs to their bare essence, resulting in a 200-line Python implementation. He argues that education is being reshuffled, with less direct teaching and more emphasis on explaining concepts to AI agents. Karpathy suggests that future educational materials should be designed for agents, enabling them to personalize explanations for individual learners. He concludes that the things that agents can't do is your job now, and things that agents can do, they can probably do better than you or like very soon.

# Keywords

|Keywords|Explanation|
|---|---|
|Code/Coding Agents|AI-powered tools that assist or automate software development tasks. Andrej Karpathy describes a shift where he delegates most coding to agents, expressing his "will" to them instead of writing code directly.|
|AI Psychosis|A state of intense focus and excitement driven by the rapid advancements in AI capabilities. Karpathy uses this term to describe his feeling of constantly trying to explore and push the limits of what's possible with AI agents.|
|Claw|A persistent, autonomous AI layer that operates independently, managing tasks and data in the background. Karpathy's "Dobby the Elf Claw" automates his home by controlling lights, HVAC, and security systems.|
|Codex|A family of AI models created by OpenAI, designed for code generation and understanding. Peter Steinberg uses multiple Codex agents to manage and modify software repositories.|
|Claude|An AI assistant developed by Anthropic, known for its helpfulness and conversational abilities. Karpathy notes Claude's relatively strong "personality" compared to other coding agents.|
|ProgramMD|A file (likely in Markdown format) that describes how an automated research system should operate. Sarah Guo suggests a contest where people write different ProgramMDs to optimize model improvement.|
|AutoResearch|An autonomous system designed to conduct research and improve AI models without human intervention. Karpathy was surprised when AutoResearch found hyperparameter tunings for NAMCHAT that he had missed.|
|Jevons Paradox|An economic principle stating that technological progress that increases the efficiency of a resource's use can increase the rate of consumption of that resource. Karpathy applies this to software engineering, suggesting that cheaper AI-assisted coding could increase the demand for software.|
|MicroGPT|A simplified, minimal implementation of a GPT (Generative Pre-trained Transformer) model intended for educational purposes. Karpathy created MicroGPT to distill LLMs down to their bare essence.|
|SETI at Home|A distributed computing project where volunteers use their computers to analyze radio telescope data in the search for extraterrestrial intelligence. Karpathy draws an analogy between SETI at Home and AutoResearch, where untrusted workers can contribute to a project.|
|Folding at Home|A distributed computing project focused on simulating protein folding to understand diseases and develop new therapies. Karpathy mentions it as an example of a project where results are expensive to generate but cheap to verify.|

# Highlights

- [(01:28)](https://podwise.ai/dashboard/episodes/7559903?locate=88) I kind of feel like I was in this perpetual, I still am often in this state of AI psychosis, just like all the time, because there was a huge unlock in what you can achieve as a person, as an individual, right?
- [(03:38)](https://podwise.ai/dashboard/episodes/7559903?locate=218) You feel like it's a skill issue. It's not that the capability is not there. It's that you just haven't found a way to string it together of what's available.
- [(13:39)](https://podwise.ai/dashboard/episodes/7559903?locate=819) Maybe there's an overproduction of lots of custom bespoke apps that shouldn't exist because agents kind of crumble them up and everything should be a lot more just like exposed API endpoints and agents are the glue of the intelligence that actually tool calls all the parts.
- [(14:13)](https://podwise.ai/dashboard/episodes/7559903?locate=853) The industry just has to reconfigure in so many ways that the customer is not the human anymore. It's agents who are acting on behalf of humans.
- [(16:57)](https://podwise.ai/dashboard/episodes/7559903?locate=1017) The name of the game now is to increase your leverage. I put in just very few tokens just once in a while and a huge amount of stuff happens on my behalf.
- [(23:07)](https://podwise.ai/dashboard/episodes/7559903?locate=1387) This is like infinite and everything is skill issue. And that's why I feel like, yeah, that's just coming back to this is why it's so insane.
- [(40:42)](https://podwise.ai/dashboard/episodes/7559903?locate=2442) Things will change in these professions because of these new tools and because of this upgrade to the nervous system of the human superorganism, if you want to think about it that way.
- [(41:41)](https://podwise.ai/dashboard/episodes/7559903?locate=2501) These jobs are bundles of tasks. And some of these tasks can go a lot faster.
- [(46:21)](https://podwise.ai/dashboard/episodes/7559903?locate=2781) I feel like a bit more a lot like aligned with humanity in a certain sense outside of Frontier Lab, because I don't, I'm not subject to those pressures almost, right.
- [(57:51)](https://podwise.ai/dashboard/episodes/7559903?locate=3471) If you just think about like read and write to the physical world, like read sensors, cameras, there's a lot of existing hardware and you can imagine like enriching agent capabilities or capturing a lot of new data if you're just clever about it and like you don't necessarily have to invest a lot to like get something valuable.
- [(1:05:57)](https://podwise.ai/dashboard/episodes/7559903?locate=3957) The things that agents can't do is your job now. Things that agents can do, they can probably do better than you or like very soon.

# Transcript

**Sarah Guo:**
[(00:00)](https://podwise.ai/dashboard/episodes/7559903?locate=0)
Code's not even the right verb anymore, right? But I have to express my will to my agents for 16 hours a day. Manifest.

**Andrej Karpathy:**
[(00:07)](https://podwise.ai/dashboard/episodes/7559903?locate=7)
How can I have not just a single session of plot code or codex or some of these agent harnesses? How can I have more of them? How can I do that appropriately? The agent part is now taken for granted. Now the claw-like entities are taken for granted. And now you can have multiple of them. And now you can have instructions to them. And now you can have optimization over the instructions. But I mean, this is why it gets to the psychosis,  is that this is like infinite and everything is skill issue.

**Sarah Guo:**
[(00:34)](https://podwise.ai/dashboard/episodes/7559903?locate=34)
Hi, listeners. Welcome back to No Priors. Today, I'm here with Andrej Karpathy, and we have a wide-ranging conversation for you about code agents,  the future of engineering and AI research, how more people can contribute to research,  what's happening in robotics, his prediction for how agents can reach out into the real world,  and education in this next age. Welcome, Andrej. Andrej, thanks for doing this.

**Andrej Karpathy:**
[(00:57)](https://podwise.ai/dashboard/episodes/7559903?locate=57)
Yeah, thank you for having me.

**Sarah Guo:**
[(00:59)](https://podwise.ai/dashboard/episodes/7559903?locate=59)
So it's been a very exciting couple of months in AI.

**Andrej Karpathy:**
[(01:02)](https://podwise.ai/dashboard/episodes/7559903?locate=62)
Oh yeah, you could say that.

**Sarah Guo:**
[(01:03)](https://podwise.ai/dashboard/episodes/7559903?locate=63)
I remember walking into the office at some point and you were like really locked in and I was asking what you were up to and you're like,  I just, I have to code for 16 hours a day or code's not even the right verb anymore,  right? But I have to express my will to my agents for 16 hours a day. Manifest. Because like there's been a jump in capability. What's happening? Tell me about your experience.

**Andrej Karpathy:**
[(01:28)](https://podwise.ai/dashboard/episodes/7559903?locate=88)
Yeah, I kind of feel like I was in this perpetual,  I still am often in this state of AI psychosis,  just like all the time, because there was a huge unlock in what you can achieve as a person,  as an individual, right? Because you were bottlenecked by, you know, your typing speed and so on. But now with these agents, it really,  I would say in December is when it really just Something flipped where I can went from eighty twenty of like you know to like twenty eighty of writing code by myself versus just delegating to agents and I don't even think it's twenty eighty by now I think it's a lot more than that I don't think I typed like a line of code.

[(01:57)](https://podwise.ai/dashboard/episodes/7559903?locate=117)
Probably since December basically which is like an extremely large. Change. I was talking about it to, for example, my parents and so on. And I don't think a normal person actually realizes that this happened or how dramatic it was. Literally, if you just find a random software engineer or something like that at their desk and what they're doing,  their default workflow of building software is completely different as of basically December. So I'm just like in the state of psychosis of trying to figure out what's possible,  trying to push it to the limit. How can I have not just a single session of Claude Code or Codex or some of these agent harnesses? How can I have more of them?

[(02:37)](https://podwise.ai/dashboard/episodes/7559903?locate=157)
How can I do that appropriately? And then how can I use these claws? What are these claws? And so there's a lot of new things. I want to be at the forefront of it,  and I'm very And see that I'm not at the forefront of it. And I see lots of people on Twitter doing all kinds of things and they all sound like really good ideas. And I need to be at the forefront or I feel extremely nervous. And so I guess I'm just in the psychosis of like, what's possible, like, because it's unexplored fundamentally.

**Sarah Guo:**
[(03:00)](https://podwise.ai/dashboard/episodes/7559903?locate=180)
Well, if you're nervous, the rest of us are nervous. We have a we have a team that we work with at Conviction, that their setup is everybody is like,  None of the engineers write code by hand, and they're all microphoned,  and they just whisper to their agents all the time. It's the strangest work setting ever. I thought they were crazy, and now I fully accept. I was like, oh, this was the way. You're just ahead of it. How do you think about your own capacity now to explore or to do projects? What is it limited by?

**Andrej Karpathy:**
[(03:32)](https://podwise.ai/dashboard/episodes/7559903?locate=212)
Yeah, what is it limited by? Just, I think everything, like so many things, even if they don't work, I think to a large extent,  you feel like it's a skill issue. It's not that the capability is not there. It's that you just haven't found a way to string it together of what's available. Like, I just don't, I didn't give good enough instructions in the agent's MD file or whatever it may be. I don't have a nice enough memory tool that I put in there or something like that. So it all kind of feels like a skill issue when it doesn't work to some extent. You want to see how you can paralyze them, et cetera. And you want to be Peter Steinberg, basically. So Peter is famous.

[(04:03)](https://podwise.ai/dashboard/episodes/7559903?locate=243)
He has a funny photo where he's in front of a monitor with lots of, like, he uses Codex. So lots of Codex agents tiling the monitor. And they all take about 20 minutes if you prompt them correctly and use the high effort. And so they all take about 20 minutes. They have multiple, you know, 10 repos checked out. And so he's just going between them and giving them work. It's just like you can move in much larger macro actions. It's not just like, here's a line of code, here's a new function. It's like, here's a new functionality and delegate it to agent one. Here's a new functionality that's not going to interfere with the other one, give it agent two.

[(04:33)](https://podwise.ai/dashboard/episodes/7559903?locate=273)
And then try to review their work as best as you can. Depending on how much you care about that code,  what are these macro actions that I can manipulate my software repository by? And another agent is doing some research, another agent is writing code,  another one is coming up with a plan for some new implementation. And so everything just happens in these macro actions over your repository. And just trying to become really good at it and develop a muscle memory for it is extremely Yeah,  it's very rewarding, number one, because it actually works. But it's also kind of like the new thing to learn. So that's why, hence the psychosis.

**Sarah Guo:**
[(05:07)](https://podwise.ai/dashboard/episodes/7559903?locate=307)
Yeah, I do feel like my instinct is like,  whenever I'm waiting for an agent to complete something,  the obvious thing to do is like, well, I can do more work, right? Like if I have access to more tokens, and like, I should just paralyze, add more tasks. And so that's very stressful because if you don't feel very bounded by your ability to spend on tokens,  then you are the bottleneck in the system that has max capability.

**Andrej Karpathy:**
[(05:30)](https://podwise.ai/dashboard/episodes/7559903?locate=330)
Yeah, if you're not maximizing your subscription, at least. And ideally for multiple agents. Like if you run out of the quota on Codex, you should switch to Claude or whatnot. I don't know. That's what I've been trying to do a little bit. And I feel nervous when I have subscription left over. That just means I haven't maximized my token throughput. So I actually kind of experienced this when I was a PhD student. You would feel nervous when your GPUs are not running. Like you have GPU capability and you're not maximizing the available flops to you. But now it's not about flops, it's about tokens. So what is your token throughput and what token throughput do you command?

**Sarah Guo:**
[(06:01)](https://podwise.ai/dashboard/episodes/7559903?locate=361)
I would actually argue that it's very interesting that we had, you know,  at least 10 years where in many engineering tasks,  people just didn't feel compute bound. Right. And the entire industry feels that now. They feel like They felt resource bound. And now that you have this big capability jump, you're like, Oh, actually, it's not,  you know, my ability to access the compute anymore. I'm the binding constraint.

**Andrej Karpathy:**
[(06:28)](https://podwise.ai/dashboard/episodes/7559903?locate=388)
Yeah, it's a skill issue. Yeah, which is very empowering. Because, yeah, because you could be getting better. So that's why that's why I think it's very addictive. Because there's unlocks when you when you get better.

**Sarah Guo:**
[(06:36)](https://podwise.ai/dashboard/episodes/7559903?locate=396)
Where do you think it goes? Like if you just think about like, okay, you know,  Andrej is iterating and everybody else is for 16 hours a day getting better at using coding agents. Like what does it look like in a year of like you've reached mastery?

**Andrej Karpathy:**
[(06:49)](https://podwise.ai/dashboard/episodes/7559903?locate=409)
Yeah, what does mastery look like right at the end of the year or like two,  three years, five years, 10 years?

**Sarah Guo:**
[(06:53)](https://podwise.ai/dashboard/episodes/7559903?locate=413)
Yeah.

**Andrej Karpathy:**
[(06:54)](https://podwise.ai/dashboard/episodes/7559903?locate=414)
Well, I think everyone is basically interested in like going up the stack. So I would say, yeah, it's not about a single session with your agent,  multiple agents, how they collaborate and teams and so on. So everyone's trying to figure out what that looks like. And then I would say CLAW is also kind of an interesting direction because it really,  when I say a CLAW, I mean this like layer that kind of takes persistence to a whole new level. Like it's something that like keeps looping. It's like, it's not something that you are interactively in the middle of. It kind of like has its own little sandbox, its own little, You know,  it kind of like does stuff on your behalf,

[(07:25)](https://podwise.ai/dashboard/episodes/7559903?locate=445)
 even if you're not looking kind of thing. And then also has like maybe more sophisticated memory systems, et cetera, that are not yet implemented in agents. So OpenClaw has a lot more sophisticated memory, I would say, than what you would get by default,  which is just a memory compaction when your context runs out, right?

**Sarah Guo:**
[(07:39)](https://podwise.ai/dashboard/episodes/7559903?locate=459)
You think that's the piece that resonated for more users versus like, perhaps like broader tool access?

**Andrej Karpathy:**
[(07:45)](https://podwise.ai/dashboard/episodes/7559903?locate=465)
For OpenClaw?

**Sarah Guo:**
[(07:46)](https://podwise.ai/dashboard/episodes/7559903?locate=466)
Yeah.

**Andrej Karpathy:**
[(07:46)](https://podwise.ai/dashboard/episodes/7559903?locate=466)
There's like, I think there's at least five things that resonated.

**Sarah Guo:**
[(07:48)](https://podwise.ai/dashboard/episodes/7559903?locate=468)
There's a lot of really good ideas in here. Yeah, good job, Peter.

**Andrej Karpathy:**
[(07:50)](https://podwise.ai/dashboard/episodes/7559903?locate=470)
I mean, Peter has done a really amazing job. I saw him recently. And I talked to him about it and he's very humble about it,  but I think he innovated simultaneously in like five different ways and put it all together. So for example, like the soul and D document,  like he actually really crafted a personality that is kind of compelling and interesting. And I feel like a lot of the current agents, they don't get this correctly. I actually think Claude has a pretty good personality. It feels like a teammate and it's excited with you, et cetera. I would say, for example, Codex is a lot more dry. Which is kind of interesting because in ChatGPT, Codex is like a lot more upbeat and highly sycophantic.

[(08:24)](https://podwise.ai/dashboard/episodes/7559903?locate=504)
But I would say Codex, the coding agent, is very dry. It doesn't seem to care about what you're creating. It's kind of like, oh, I implemented it. It's like, okay, but do you understand what we're building?

**Sarah Guo:**
[(08:33)](https://podwise.ai/dashboard/episodes/7559903?locate=513)
It's true.

**Andrej Karpathy:**
[(08:34)](https://podwise.ai/dashboard/episodes/7559903?locate=514)
You know, it doesn't. And the other thing I would say is, for example, with Claude,  I think they dialed the psycho fantasy fairly well,  where when Claude gives me praise, I do feel like I slightly deserve it. Because sometimes I kind of give it like not very well formed thoughts. And I give him an idea that I don't think is fully baked. And it doesn't actually react very strongly. It's like, oh, yeah, we can implement that. But when it's a really good idea, by my own account, it does seem to reward it a bit more. And so I kind of feel like I'm trying to like earn its praise, which is really weird. And so I do think the personality matters a lot.

[(09:03)](https://podwise.ai/dashboard/episodes/7559903?locate=543)
And I think a lot of the other tools maybe don't appreciate it as much. And I think in this aspect, also, Peter really cares about this. And so that was correct. And then the memory system. And then just, you know, he's just having fun with this. And then the single WhatsApp portal tool of the automation. Yeah.

**Sarah Guo:**
[(09:18)](https://podwise.ai/dashboard/episodes/7559903?locate=558)
Is there something that you have done personally? With your claws on software engineering that you think is fun or interesting.

**Andrej Karpathy:**
[(09:25)](https://podwise.ai/dashboard/episodes/7559903?locate=565)
Yeah. So in January, I had a claw. I went through a period of claw psychosis. So I built I have a claw basically that takes care of my home and I call him Dobby the Elf Claw. And basically, I used the agents to find all of the smart home subsystems of my home on the local area network,  which I was kind of surprised that worked out of the box. Like I just told it that I think I have Sonos at home, like, can you try to find it? And it goes and like IP scan of all the basically computers on the local area network,  and it found the Sonos thing, the Sonos system. And it turned out that there's no password protection or anything like that.

[(10:01)](https://podwise.ai/dashboard/episodes/7559903?locate=601)
It just logged in and it's like, oh, yeah, you have these Sono systems installed. Let me try to reverse engineer how it's working. It does some web searches and it finds like, OK, these are the API endpoints. And then it's like, do you want to try it? And I'm like, whoa, like you just did that. I'm like, yeah, can you try to play something in the study? And it does, and music comes out. And I'm like, I can't believe I just- That's crazy.

**Sarah Guo:**
[(10:18)](https://podwise.ai/dashboard/episodes/7559903?locate=618)
That's like three prompts. Yeah.

**Andrej Karpathy:**
[(10:20)](https://podwise.ai/dashboard/episodes/7559903?locate=620)
I can't believe I just typed in, like, can you find my Sonos? And that suddenly it's playing music. And it did the same for lights. And so basically, like, it kind of hacked in, figured out the whole thing,  created APIs, created a dashboard, so I could see the command kind of center of,  like, all of my lights in the home. And then it was like switching lights on and off. And, you know, so I can ask it, like, don't be at sleepy time. And when it's sleepy time, that just means all the lights go off, et cetera, and so on. So it controls all of my lights, my HVAC, my shades, the pool and the spa,  and also my security system. So I have a camera pointed outside of the house.

[(10:50)](https://podwise.ai/dashboard/episodes/7559903?locate=650)
And anytime someone rolls in, I have a QWIN, a QWIN model that looks at the videos. So first of all, there's change detection. And then based on change detection, it goes to QWIN. And then it actually like tells me, it sends me a text to my WhatsApp. It shows an image from the outside. And it says, hey, FedEx truck just pulled up,  FedEx truck just pulled up and you might want to check it and you got new mail or something like that. And Dobby just texted me this. It's really incredible. So Adobe is in charge of the house. I text with it through WhatsApp. And it's been really fun to have these macro actions that maintain my house. I haven't really pushed it way more beyond that.

[(11:28)](https://podwise.ai/dashboard/episodes/7559903?locate=688)
And I think people are doing a lot more crazy things with it. But for me, even just a home automation setup, I used to use six apps, completely different apps. And I don't have to use these apps anymore. Adobe controls everything in natural language. It's amazing. And so I think I haven't even pushed a paradigm fully,  but already that is so helpful and so inspiring,  I would say.

**Sarah Guo:**
[(11:45)](https://podwise.ai/dashboard/episodes/7559903?locate=705)
Do you think that's indicative of like what people want from a user experience perspective with software, right? Because I don't think, you know, it's pretty ignored that it takes humans effort to like learn new software,  like new UI.

**Andrej Karpathy:**
[(11:57)](https://podwise.ai/dashboard/episodes/7559903?locate=717)
Yeah, I think to some extent, that's right. It's like working backwards from how people think an AI should be. Because what people have in their mind of like what an AI is,  is not actually what an LLM is by like in the raw sense. Like LLM is a token generator, you know, like more tokens come out. But what they think of is like this persona identity that they can tell stuff and it remembers it,  you know, and it's just kind of an entity behind a WhatsApp. It's like a lot more understandable. So I think to some extent it's like matching the expectations that humans already have for what AI should behave. But under the hood, it's like a lot of technical details go into that.

[(12:30)](https://podwise.ai/dashboard/episodes/7559903?locate=750)
And LLMs are too raw of a primitive to actually type check as AI,  I think, for most people, if that makes sense.

**Sarah Guo:**
[(12:37)](https://podwise.ai/dashboard/episodes/7559903?locate=757)
Yeah,  I think that's like how we understand what the AI is and like the description of it as DABI or some personality obviously resonates with people. I also think that the unification that you did across your six different software systems for your home automation speaks to a different question of like,  do people really want all the software that we have today?

**Andrej Karpathy:**
[(12:59)](https://podwise.ai/dashboard/episodes/7559903?locate=779)
Yeah.

**Sarah Guo:**
[(12:59)](https://podwise.ai/dashboard/episodes/7559903?locate=779)
Right. Because I would argue like, well, you have the hardware, but you've now thrown away the software,  or the UX layer of it. Do you think that's what people want?

**Andrej Karpathy:**
[(13:09)](https://podwise.ai/dashboard/episodes/7559903?locate=789)
Yeah, I think there's this like, there's this sense that these apps that are in the app store for using these smart home devices,  etc. These shouldn't even exist kind of in a certain sense. Like, shouldn't it just be APIs and shouldn't agents be just using it directly? And wouldn't it, like, I can do all kinds of home automation stuff that any individual app will not be able to do,  right? And then LLM can actually drive the tools and call all the right tools and do pretty complicated things. And so in a certain sense, it does point to this,

[(13:39)](https://podwise.ai/dashboard/episodes/7559903?locate=819)
 like maybe there's like an overproduction of lots of custom bespoke apps that shouldn't exist because agents kind of like crumble them up and everything should be a lot more just like exposed API endpoints and agents are the glue of the intelligence that actually like tool calls all the parts. Another example is my treadmill. There's an app for my treadmill, and I want it to keep track of how often I do my cardio. But I don't want to log into a web UI and go through a flow and et cetera. All this should just be like, make APIs available. And this is kind of going towards a gentic web or agent-first tools and all this kind of stuff.

[(14:13)](https://podwise.ai/dashboard/episodes/7559903?locate=853)
So I think the industry just has to reconfigure in so many ways that the customer is not the human anymore. It's agents who are acting on behalf of humans. And this refactoring will probably be substantial in a certain sense. One way that people sometimes push back on this is like,  do we expect people to bytecode some of these tools? Do we expect normal people to do this kind of stuff that I described? But I think to some extent, this is just technology as it exists today. And right now there is some bytecoding and I'm actually watching it and I'm working with the system. But I kind of feel like this kind of stuff that I just talked about,  this should be free, like in a year or two or three.

[(14:47)](https://podwise.ai/dashboard/episodes/7559903?locate=887)
There's no bytecoding involved. This is trivial. This is table stakes. This is like any AI, even the open source models, et cetera, can like do this.

**Sarah Guo:**
[(14:54)](https://podwise.ai/dashboard/episodes/7559903?locate=894)
You should be able to translate from a less technical human's intent very easily to this outcome. Yeah, extremely easily.

**Andrej Karpathy:**
[(15:00)](https://podwise.ai/dashboard/episodes/7559903?locate=900)
Today it's by coding and it's involved and not many people are going to do it.

**Sarah Guo:**
[(15:02)](https://podwise.ai/dashboard/episodes/7559903?locate=902)
And you still have to make some design decisions, right? We were talking about like we take frames, for example.

**Andrej Karpathy:**
[(15:07)](https://podwise.ai/dashboard/episodes/7559903?locate=907)
Yeah. But I kind of feel like this will just start to,  the barrier will just come down and it's just ephemeral software on your behalf. And some kind of like claw is handling all the details for you, but you're not involved. Claw has a machine and it will figure it out. And it's just presenting you UIs and you're like saying stuff, you know?

**Sarah Guo:**
[(15:26)](https://podwise.ai/dashboard/episodes/7559903?locate=926)
Why haven't you, I guess, like pushed the boundaries of what you can do personally with CLAWS? Like, is it, you know, you're focusing on more important projects, auto research, et cetera,  or you're climbing the hill to mastery or something else, right?

**Andrej Karpathy:**
[(15:41)](https://podwise.ai/dashboard/episodes/7559903?locate=941)
Yeah, I just feel like I'm so distracted by everything. So I spend like a week on the CLAWS stuff, and I have more to do almost. But I will say that...

**Sarah Guo:**
[(15:50)](https://podwise.ai/dashboard/episodes/7559903?locate=950)
It's like Jensen told us, we're all just busier, unfortunately.

**Andrej Karpathy:**
[(15:53)](https://podwise.ai/dashboard/episodes/7559903?locate=953)
I didn't really take advantage of a lot of like email and calendar and all this other stuff. And I didn't give it access because I'm still a little bit like suspicious and still very new and rough around the edges. So I didn't want to give it like full access to my digital life yet. And part of it is just less security, privacy and just being very cautious in that in that realm. And so some of it is held back by that, I would say. Yeah, maybe that's the dominant feature,  but some of it is also just I feel so distracted because I feel like I had a week of claw and then other stuff is happening.

**Sarah Guo:**
[(16:21)](https://podwise.ai/dashboard/episodes/7559903?locate=981)
What was the... I mean,  you've talked about being able to train or at least optimize a model as a task you want to see agents do for a long time. What was the motivation behind AutoResearch?

**Andrej Karpathy:**
[(16:33)](https://podwise.ai/dashboard/episodes/7559903?locate=993)
AutoResearch, yeah. So I think I had a tweet earlier where I kind of said something along the lines of,  To get the most out of the tools that have become available now,  you have to remove yourself as the bottleneck. You can't be there to prompt the next thing. You need to take yourself outside. You have to arrange things such that they're completely autonomous. And the more, you know, how can you maximize your token throughput and not be in the loop? This is the goal. And so I kind of mentioned that the name of the game now is to increase your leverage. I put in just very few tokens just once in a while and a huge amount of stuff happens on my behalf.

[(17:06)](https://podwise.ai/dashboard/episodes/7559903?locate=1026)
And so auto research, like I tweeted that and I think people liked it and whatnot. They haven't maybe worked through the implications of that. And for me, AutoResearch is an example of an implication of that, where it's like,  I don't want to be the researcher in the loop, looking at results, et cetera. I'm holding the system back. So the question is, how do I refactor all the abstractions so that I'm not,  I have to arrange it once and hit go. The name of the game is, how can you get more agents running for longer periods of time without your involvement doing stuff on your behalf? And AutoResearch is just, yeah, here's an objective, here's a metric,

[(17:37)](https://podwise.ai/dashboard/episodes/7559903?locate=1057)
 here's your boundaries of what you can and cannot do,  and go.

**Sarah Guo:**
[(17:41)](https://podwise.ai/dashboard/episodes/7559903?locate=1061)
And you were surprised at its effectiveness.

**Andrej Karpathy:**
[(17:44)](https://podwise.ai/dashboard/episodes/7559903?locate=1064)
Yeah, I didn't expect it to work because I have the project data chat. And fundamentally, I think a lot of people are very confused with my obsession for training GPT-2 models and so on. But for me, training GPT models and so on is just a little harness, a little playground for training LLMs. And fundamentally,  what I'm more interested in is this idea of recursive self-improvement and to what extent you can actually have LLMs improving LLMs. Because I think all the Frontier Labs, this is like the thing for obvious reasons. And they're all trying to recursively self-improve, roughly speaking. And so for me, this is kind of like a little playpen of that.

[(18:17)](https://podwise.ai/dashboard/episodes/7559903?locate=1097)
And I guess I like tuned NAMCHAT already quite a bit by hand in a good old fashioned way that I'm used to. Like I'm a researcher. I've done this for like, you know, two decades. I have some amount of like, what is the opposite of hubris?

**Sarah Guo:**
[(18:27)](https://podwise.ai/dashboard/episodes/7559903?locate=1107)
Earned confidence.

**Andrej Karpathy:**
[(18:29)](https://podwise.ai/dashboard/episodes/7559903?locate=1109)
Okay. I have like two decades of like, oh,  I've trained this model like thousands of times of like,  So I've done a bunch of experiments. I've done hyperparameter tuning. I've done all the things I'm very used to and I've done for two decades.

**Sarah Guo:**
[(18:39)](https://podwise.ai/dashboard/episodes/7559903?locate=1119)
Yeah.

**Andrej Karpathy:**
[(18:39)](https://podwise.ai/dashboard/episodes/7559903?locate=1119)
And I've gotten to a certain point and I thought it was like fairly well tuned. And then I let AutoResearch go for like overnight and it came back with like tunings that I didn't see. And yeah, I did forget like the weight decay on the value embeddings and my atom betas were not sufficiently tuned. And these things jointly interact. So like once you tune one thing, the other things have to potentially change too. You know, I shouldn't be a bottleneck. I shouldn't be running these hyperparameter search optimizations. I shouldn't be looking at the results. There's objective criteria in this case, so you just have to arrange it so that it can just go forever.

[(19:08)](https://podwise.ai/dashboard/episodes/7559903?locate=1148)
So that's a single sort of version of AutoResearch, of like a single loop trying to improve. And I was surprised that it found these things that I, you know,  the repo is already fairly well tuned and still found something. And that's just a single, it's a single loop. Like these Frontier Labs, they have GPU clusters of tens of thousands of them. And so it's very easy to imagine how you would basically get a lot of this automation on smaller models. And fundamentally, everything around like frontier level intelligence is about extrapolation and scaling loss. And so you basically do a ton of the exploration on the smaller models,  and then you try to extrapolate out.

**Sarah Guo:**
[(19:43)](https://podwise.ai/dashboard/episodes/7559903?locate=1183)
So you're saying our research efforts are going to get more efficient,  like we're going to have better direction for when we scale as well. If we can do this experimentation better.

**Andrej Karpathy:**
[(19:50)](https://podwise.ai/dashboard/episodes/7559903?locate=1190)
Yeah, I would say that like the most interesting project and probably what the Frontier Labs are working on is,  you know, you experiment on the smaller models,  you try to make it as autonomous as possible,  remove researchers from the loop. They have way too much. What is the opposite? Earned confidence? Yeah, they don't know. They shouldn't be touching any of this really. And so you have to like rewrite the whole thing because right now, I mean, certainly they can contribute ideas. But OK, they shouldn't actually be enacting these ideas.

[(20:15)](https://podwise.ai/dashboard/episodes/7559903?locate=1215)
There is a queue of ideas and there's maybe an automated scientist that comes up with ideas based on all the archive papers and GitHub repos and it funnels ideas in. Or researchers can contribute ideas,  but it's a single queue and there's workers that pull items and they try them out and whatever works just gets sort of put on the feature branch and maybe some people like monitor the feature branch and merge to the main branch sometimes. Yeah, just removing humans from all the processes and automating as much as possible and getting high tokens per second throughputs. And it does require rethinking of all the abstractions and everything has to be reshuffled. So yeah, I think it's very exciting.

**Sarah Guo:**
[(20:54)](https://podwise.ai/dashboard/episodes/7559903?locate=1254)
If we take one more recursive step here,  when is the model going to write a better program MD than you?

**Andrej Karpathy:**
[(21:00)](https://podwise.ai/dashboard/episodes/7559903?locate=1260)
Yeah. So ProgramMD is like...

**Sarah Guo:**
[(21:03)](https://podwise.ai/dashboard/episodes/7559903?locate=1263)
We're not on the loop.

**Andrej Karpathy:**
[(21:04)](https://podwise.ai/dashboard/episodes/7559903?locate=1264)
Yeah, exactly. Yeah. So ProgramMD is my crappy attempt at describing like how the auto researcher should work. Like, oh, do this and do that and that and then try these kinds of ideas. And then here's maybe some ideas like look at architecture, look at optimizer, etc. But I just came up with this in Markdown, right? And so, yeah, exactly. You want some kind of an auto research loop maybe that looks for You can imagine that different program.mds would give you different progress. So basically every research organization is described by program.md. A research organization is a set of markdown files that describe all the roles and how the whole thing connects.

[(21:43)](https://podwise.ai/dashboard/episodes/7559903?locate=1303)
And you can imagine having a better research organization. So maybe they do fewer stand-ups in the morning because they're useless. And this is all just code, right? And so one organization can have fewer stand-ups. One organization can have more. One organization can be very risk-taking. One organization can be less. As you can definitely imagine that you have multiple research orgs. And then they all have code. And once you have code, then you can imagine tuning the code. So 100% there's like the metal layer of it.

**Sarah Guo:**
[(22:09)](https://podwise.ai/dashboard/episodes/7559903?locate=1329)
Did you see my text about my contest idea? My contest idea was Uh, like Let people write different program MDs, right? And so for same hardware, where do you get most improvement?

**Andrej Karpathy:**
[(22:22)](https://podwise.ai/dashboard/episodes/7559903?locate=1342)
Oh, I see.

**Sarah Guo:**
[(22:22)](https://podwise.ai/dashboard/episodes/7559903?locate=1342)
And then you can take all that data and then give it to the model and say,  write a better program MD.

**Andrej Karpathy:**
[(22:26)](https://podwise.ai/dashboard/episodes/7559903?locate=1346)
Yes, yes. Yeah, exactly.

**Sarah Guo:**
[(22:28)](https://podwise.ai/dashboard/episodes/7559903?locate=1348)
We're going to get something better. Like, there's no way we don't.

**Andrej Karpathy:**
[(22:30)](https://podwise.ai/dashboard/episodes/7559903?locate=1350)
You can 100% look at where the improvements came from. And like, can I change the program MD such that more of these kinds of things would be done? Or like things that didn't work.

**Sarah Guo:**
[(22:40)](https://podwise.ai/dashboard/episodes/7559903?locate=1360)
Meta-optimization.

**Andrej Karpathy:**
[(22:41)](https://podwise.ai/dashboard/episodes/7559903?locate=1361)
Yeah, you can 100% imagine doing that. So I think this is a great idea. It's like, you know,  I think like you sort of go one step at a time where you sort of have one process and then second process and then the next process. And these are all layers of an onion, like the LLM sort of part is now taken for granted. The agent part is now taken for granted. Now the claw-like entities are taken for granted and now you can have multiple of them and now you can have instructions to them and now you can have optimization over the instructions. And it's just like a little too much, you know, but I mean,  this is why it gets to the psychosis is that this is like infinite and everything is skill issue.

[(23:11)](https://podwise.ai/dashboard/episodes/7559903?locate=1391)
And that's why I feel like Yeah, that's just coming back to this is why it's so insane.

**Sarah Guo:**
[(23:15)](https://podwise.ai/dashboard/episodes/7559903?locate=1395)
Okay, well, we're just trying to like, diagnose the current moment and what is a relevant skill right now? What do you like? What do you think is the implication that this,  that this is the loop we should be trying to achieve in different areas,  and then it works, right? Like, you know, remove, create the metric or create the ability for agents to continue working on it without you?

**Andrej Karpathy:**
[(23:37)](https://podwise.ai/dashboard/episodes/7559903?locate=1417)
Yeah.

**Sarah Guo:**
[(23:38)](https://podwise.ai/dashboard/episodes/7559903?locate=1418)
Do we still have performance engineering?

**Andrej Karpathy:**
[(23:40)](https://podwise.ai/dashboard/episodes/7559903?locate=1420)
Yeah, I mean, so there's a few caveats that I would put on top of the LLM psychosis. Number one, this is extremely well suited to anything that has objective metrics that are easy to evaluate. So, for example, like writing kernels for more efficient CUDA, you know, code for various parts of a model, etc. The perfect fit. Because you have inefficient code and then you want efficient code that has the exact same behavior,  but it's much faster. Perfect fit. A lot of things are a perfect fit for auto research, but many things will not be. If you can't evaluate it, then you can't auto research it. So that's like caveat number one. And then maybe caveat number two, I would say is, you know,

[(24:15)](https://podwise.ai/dashboard/episodes/7559903?locate=1455)
 we're kind of talking about next steps and we kind of see what the next steps are. But fundamentally, the whole thing still doesn't, it's still kind of like bursting at the seams a little bit and there's cracks and it doesn't fully work. And if you kind of try to go too far ahead,  the whole thing is actually net not useful,  if that makes sense. Because these models like still are not, you know, they've improved a lot,  but they're still like rough around the edges is maybe the way I would describe it. I simultaneously feel like I'm talking to an extremely brilliant PhD student who's been like a systems programmer for their entire life and a 10-year-old.

[(24:45)](https://podwise.ai/dashboard/episodes/7559903?locate=1485)
And it's so weird because humans like there's like,  I feel like they're a lot more coupled,  like you have to, you know, everything is a lot more coupled.

**Sarah Guo:**
[(24:52)](https://podwise.ai/dashboard/episodes/7559903?locate=1492)
Yes, you wouldn't encounter that combination.

**Andrej Karpathy:**
[(24:54)](https://podwise.ai/dashboard/episodes/7559903?locate=1494)
This jaggedness is really strange and humans have a lot less of that kind of jaggedness,  although they definitely have some. But humans have a lot more jaggedness. Sorry, the agents have a lot more jaggedness where Sometimes like, you know,  I asked for functionality and it like comes back with something that's just like,  totally wrong. And then we get into loops that are totally wrong. And then I'm just I get so frustrated with the agents all the time still,  because you feel the power of it. But you also there's still like, it does nautical things once in a while for me still as well.

**Sarah Guo:**
[(25:23)](https://podwise.ai/dashboard/episodes/7559903?locate=1523)
I get very annoyed when I feel like the agent wasted a lot of compute on something it should have recognized was an obvious problem.

**Andrej Karpathy:**
[(25:32)](https://podwise.ai/dashboard/episodes/7559903?locate=1532)
Yeah. I think like some of the bigger things is like maybe what's underneath it,  if I could hypothesize, is fundamentally these models are trained via reinforcement learning. So they're actually struggling with the exact same thing we just talked about,  which is the labs can improve the models in anything that is verifiable,  whether it has rewards. So did you write the program correctly and do the unit test, check out, yes or no? But some of the things where they're struggling is like, for example,  I think they have a tough time with like nuance of maybe what I what I had in mind or what I intended and when to ask clarifying questions.

[(26:03)](https://podwise.ai/dashboard/episodes/7559903?locate=1563)
Like, yeah, it's just anything that feels softer is like worse. And so you're kind of like you're either on rails and you're part of the superintelligence circuits or you're not on rails and you're outside of the verifiable domains. And suddenly everything kind of just like meanders. Like maybe another way to put it is if you go to today,  if you go to like state of the art model,  ChatGPT, and you ask it, tell me a joke. Do you know what joke you're going to get? The joke.

**Sarah Guo:**
[(26:28)](https://podwise.ai/dashboard/episodes/7559903?locate=1588)
The joke? I can't tell you like the standard form of it, but I do feel like ChatGPT has like three jokes.

**Andrej Karpathy:**
[(26:34)](https://podwise.ai/dashboard/episodes/7559903?locate=1594)
Yeah. So the joke that apparently all the LLMs like the most is, why do scientists not trust atoms?

**Sarah Guo:**
[(26:41)](https://podwise.ai/dashboard/episodes/7559903?locate=1601)
Okay.

**Andrej Karpathy:**
[(26:41)](https://podwise.ai/dashboard/episodes/7559903?locate=1601)
Because they make everything up. They make everything up.

**Sarah Guo:**
[(26:45)](https://podwise.ai/dashboard/episodes/7559903?locate=1605)
What's that eMERGE?

**Andrej Karpathy:**
[(26:47)](https://podwise.ai/dashboard/episodes/7559903?locate=1607)
So this is the joke you would get three or four years ago,  and this is the joke you still get today. So even though the models have improved tremendously,  and if you give them an agentic task,  they will just go for hours and move mountains for you. And then you ask for a joke, and it has a stupid joke. It's a crappy joke from five years ago. And it's because it's outside of the RL. It's outside of the reinforcement learning. It's outside of what's being improved. And it's part of the jaggedness of like,  shouldn't you expect models as they get better to also have like better jokes or more diversity of them or it's just it's not being optimized and it's stuck.

**Sarah Guo:**
[(27:22)](https://podwise.ai/dashboard/episodes/7559903?locate=1642)
Do you think that that implies that we are not seeing like generalization in the sense of like broader intelligence of joke smartness being attached to code smartness?

**Andrej Karpathy:**
[(27:35)](https://podwise.ai/dashboard/episodes/7559903?locate=1655)
Yeah,  I think there's some decoupling where some things are verifiable and some things are not and some things are optimized for arbitrarily by the labs depending on like what data went in and some things are not.

**Sarah Guo:**
[(27:47)](https://podwise.ai/dashboard/episodes/7559903?locate=1667)
There's a premise from some research groups that if you're smarter at code generation or in these verifiable fields,  you should be better at everything. The joke situation suggests that that's not happening.

**Andrej Karpathy:**
[(28:00)](https://podwise.ai/dashboard/episodes/7559903?locate=1680)
I don't think that's happening. I think maybe we're seeing a little bit of that, but not a satisfying amount.

**Sarah Guo:**
[(28:07)](https://podwise.ai/dashboard/episodes/7559903?locate=1687)
That jaggedness exists in humans. You can be very, very good at math and still tell a really bad joke.

**Andrej Karpathy:**
[(28:13)](https://podwise.ai/dashboard/episodes/7559903?locate=1693)
Yeah, that's true. Yeah,  but it just it still means that we're not getting like the story is that we're getting a lot of the intelligence and capabilities and all the domains of society,  like for free as we get better and better models. And it's not like exactly fundamentally what's going on. And there's some blind spots and some things are not being optimized for and this is all clustered up in these neural net opaque models,  right? So you're either on rails of what it was trained for and everything is like you're going at speed of light or you're not. And so it's the jaggedness. So that's why I think like even though the progression is obvious what should happen,

[(28:46)](https://podwise.ai/dashboard/episodes/7559903?locate=1726)
 you can't let it fully go there yet because it doesn't fully work or it's a skill issue and we just haven't like figured out how to use it. So, you know, it's hard to tell.

**Sarah Guo:**
[(28:55)](https://podwise.ai/dashboard/episodes/7559903?locate=1735)
Can I ask kind of a blasphemous question,  which is like if this jaggedness is persisting and it's all rolled up in a at least monolithic interface,  right? But you know, single model. Does that make sense or should it be unbundled in things that can be optimized and improved against different.

**Andrej Karpathy:**
[(29:15)](https://podwise.ai/dashboard/episodes/7559903?locate=1755)
domains of intelligence, like unbundling the models into multiple experts in different areas, etc.

**Sarah Guo:**
[(29:20)](https://podwise.ai/dashboard/episodes/7559903?locate=1760)
More directly. Yeah. Instead of just MOE that we have no exposure to,  because that can be confusing as a user from the outside,  which is like, why is it so good at this, but not at this other thing?

**Andrej Karpathy:**
[(29:31)](https://podwise.ai/dashboard/episodes/7559903?locate=1771)
Yeah,  I think currently my impression is the labs are trying to have a single monoculture of a model that is arbitrarily intelligent in all these different domains,  and they just stuff into the parameters. I do think we should expect more speciation in the intelligences. Like, you know, the animal kingdom is extremely diverse in the brains that exist. And there's lots of different niches of nature. And some animals have overdeveloped visual cortex or other kind of parts. And I think we should be able to see more speciation. And you don't need like this Oracle that knows everything. You kind of speciate it and then you put it on a specific task.

[(30:08)](https://podwise.ai/dashboard/episodes/7559903?locate=1808)
And we should be seeing some of that because you should be able to have like much smaller models that still have the cognitive core,  like they're still competent, but then they specialize. And then they can become more efficient in terms of latency or throughput on specific tasks that you really care about. Like if you're a mathematician working in Lean, I saw, for example,  there's a few releases that really like target that as a domain. So there's probably going to be a few examples like that where the unbundling kind of makes sense.

**Sarah Guo:**
[(30:33)](https://podwise.ai/dashboard/episodes/7559903?locate=1833)
One question I have is whether or not the capacity constraint on available compute infrastructure drives more of this because efficiency actually matters more. Financing aside, no financing is involved in all of this. If you have access to full compute for anything you do, like even one single model, right? But if you actually feel pressure where you're like,  I can't serve And we're going to be talking about a model of massive size for every use case. Do you think that leads to any speciation? Does that question make sense to you?

**Andrej Karpathy:**
[(31:07)](https://podwise.ai/dashboard/episodes/7559903?locate=1867)
The question makes sense. And I guess what I'm struggling with is I don't think we've seen too much speciation just yet, right?

**Sarah Guo:**
[(31:14)](https://podwise.ai/dashboard/episodes/7559903?locate=1874)
No.

**Andrej Karpathy:**
[(31:14)](https://podwise.ai/dashboard/episodes/7559903?locate=1874)
We're seeing a monoculture of models.

**Sarah Guo:**
[(31:16)](https://podwise.ai/dashboard/episodes/7559903?locate=1876)
Yeah. And there's clearly pressure for make a good code model, put it back in the main merge again.

**Andrej Karpathy:**
[(31:21)](https://podwise.ai/dashboard/episodes/7559903?locate=1881)
Yeah. Even though there already is pressure on the models.

**Sarah Guo:**
[(31:28)](https://podwise.ai/dashboard/episodes/7559903?locate=1888)
I guess perhaps I feel like there's a lot of very short term supply crunch and like maybe that causes more speciation now.

**Andrej Karpathy:**
[(31:35)](https://podwise.ai/dashboard/episodes/7559903?locate=1895)
Yeah,  I think fundamentally like the labs are serving a model and they don't really know what the end user is going to be asking about. So maybe that's like some part of it because they kind of have to multitask over all the possible things that could be asked. But I think if you're coming to a business and maybe partnering on some specific problems you care about,  then maybe you would see that there. Or there will be some very high value applications that are like more niche. But I think right now they're kind of going after the totality of what's available. I don't think that the science of manipulating the brains is fully developed yet, partly.

**Sarah Guo:**
[(32:07)](https://podwise.ai/dashboard/episodes/7559903?locate=1927)
What do you mean, manipulating?

**Andrej Karpathy:**
[(32:08)](https://podwise.ai/dashboard/episodes/7559903?locate=1928)
So fine-tuning without losing capabilities, as an example. And we don't have these primitives for actually working with the intelligences in ways other than just context windows. Context windows kind of just work, and it's very cheap to manipulate, etc. And this is how we're getting some of the customization, etc. But I think if it was I think it's a it's a bit more of a developing science of how you like more deeply adjust the models,  how you have continual learning, maybe or how you how you fine tune in certain area,  how you get better in certain area or like how you actually touch the weights,  not just the context windows. And so it's a lot more. It's a little bit more tricky, I would say,

[(32:40)](https://podwise.ai/dashboard/episodes/7559903?locate=1960)
 to touch the weights than just the context windows,  because you're actually fundamentally changing the full model and potentially its intelligence. And so maybe it's just not a fully developed science, if that makes sense, of speciation.

**Sarah Guo:**
[(32:51)](https://podwise.ai/dashboard/episodes/7559903?locate=1971)
And it also has to be cheap enough for that speciation to be worthwhile in these given contexts. Can I ask a question about an extension to auto research that you described in terms of open ground? You know, we have this thing. We need more collaboration surface around it, essentially, for people to contribute to research overall. Can you talk about that?

**Andrej Karpathy:**
[(33:15)](https://podwise.ai/dashboard/episodes/7559903?locate=1995)
Yeah. So we talked about our research has a single thread of like, I'm going to try stuff and loot. But fundamentally, the parallelization of this is like the interesting component. And I guess I was trying to like play around with a few ideas,  but I don't have anything that like clicks as simply as like,  I don't have something that I'm like super happy with just yet,  but it's something I'm like working on inside when I'm not working on my claw. So I think like one issue is if you have a bunch of nodes of parallelization available to you,  then it's very easy to just have multiple auto researchers talking through a common system or something like that.

[(33:46)](https://podwise.ai/dashboard/episodes/7559903?locate=2026)
What I was more interested in is how you can have an untrusted pool of workers out there on the internet. So for example, in auto research, you're just trying to find the piece of code that trains a model to a very low validation loss. If anyone gives you a candidate commit, it's very easy to verify that that commit is correct, is good. Someone could claim from the internet that this piece of code will optimize much better and give you much better performance. You could just check. It's very easy. But probably a lot of work goes into that checking. But fundamentally, they could lie and et cetera. So you're basically dealing with a similar kind of problem.

[(34:20)](https://podwise.ai/dashboard/episodes/7559903?locate=2060)
It almost actually looks a little bit like my designs that incorporate an untrusted pool of workers actually look a little bit more like a blockchain,  a little bit. Because instead of blocks,  you have commits and these commits can build on each other and they contain like changes to the code as you're improving it. And the proof of work is basically doing tons of experimentation to find the commits that work. And that's hard. And then the reward is just being on the leaderboard right now. There's no monetary reward whatsoever. But I don't want to push the analogy too far,  but it fundamentally has this issue where a huge amount of search goes into it,

[(34:53)](https://podwise.ai/dashboard/episodes/7559903?locate=2093)
 but it's very cheap to verify that a candidate solution is indeed good because you can just train a single,  you know, someone had to try 10,000 ideas, but You just have to check that the thing that they produced actually works because the 99,000 of them didn't work,  you know? And so basically, long story short,  it's like you have to come up with a system where an untrusted pool of workers can collaborate with a trusted pool of workers that do the verification. And the whole thing is kind of like asynchronous and works and so on. And it's like safe from a security perspective because if anyone sends you arbitrary code and you're going to run it,  that's very sketchy and dodgy.

[(35:30)](https://podwise.ai/dashboard/episodes/7559903?locate=2130)
But fundamentally, it should be totally possible. So you're familiar with projects like SETI at home and folding at home. All of these problems have a similar kind of setup. So folding at home, you're folding a protein, and it's very hard to find a configuration that is low energy. But if someone finds a configuration that they evaluate to be low energy, that's perfect. You can just use it. You can easily verify it. So a lot of things have this property that, you know, very expensive to come up with,  but very cheap to verify. And so in all those cases, things like folding at home or SETI at home or AutoResearch at home will be good fits. And so, long story short,

[(36:01)](https://podwise.ai/dashboard/episodes/7559903?locate=2161)
 a swarm of agents on the internet could collaborate to improve LLMs and could potentially even like run circles around Frontier Labs,  like who knows, you know. Yeah, like maybe that's even possible. Like Frontier Labs have a huge amount of trusted compute,  but the earth is much bigger and has a huge amount of untrusted compute. But if you put systems in check, systems in place that deal with this,  then maybe it is possible that the swarm out there could come up with better solutions. And people kind of like contribute cycles. And so, sorry, so the last thought is lots of companies or whatnot,  they could maybe have like their own things that they care about.

[(36:40)](https://podwise.ai/dashboard/episodes/7559903?locate=2200)
And you, if you have compute capacity, you could contribute to different kind of auto research tracks. Like maybe you care about certain, you know,  like you care about like cancer or something like that of certain type. You don't have to just donate money to an institution. You actually could like purchase compute and then you could join the auto research forum for that project, you know. So if everything is rebundled into auto researchers, then compute becomes the thing that you're contributing to the pool.

**Sarah Guo:**
[(37:03)](https://podwise.ai/dashboard/episodes/7559903?locate=2223)
Yeah, that's very inspiring. And it's also interesting, like, I don't I don't know how far this goes. But it is interesting that at least some audience of people, you know,  here in Silicon Valley or lining up at,  you know, retail stores in China have discovered that Like having access to personal compute is interesting again.

**Andrej Karpathy:**
[(37:20)](https://podwise.ai/dashboard/episodes/7559903?locate=2240)
Yeah.

**Sarah Guo:**
[(37:21)](https://podwise.ai/dashboard/episodes/7559903?locate=2241)
Right. So maybe they're really motivated to do that for their claws and then they can contribute to auto research.

**Andrej Karpathy:**
[(37:25)](https://podwise.ai/dashboard/episodes/7559903?locate=2245)
It's almost like dollars, the thing everyone cares about. But is flop the thing that everyone cares about in the future? Like, is there going to be like a flipping almost of like what's the thing that you care about? Like right now, for example, it's really hard to get compute even if you have money.

**Sarah Guo:**
[(37:37)](https://podwise.ai/dashboard/episodes/7559903?locate=2257)
Yeah.

**Andrej Karpathy:**
[(37:38)](https://podwise.ai/dashboard/episodes/7559903?locate=2258)
So actually, it almost seems like the flop is like dominant in a certain sense. Yeah, so maybe that's kind of like that. How many flops do you control instead of what wealth do you control? I don't actually think that's true, but it's kind of interesting to think about.

**Sarah Guo:**
[(37:53)](https://podwise.ai/dashboard/episodes/7559903?locate=2273)
The last thing you released was a little bit of jobs data analysis. Is that right? Yeah. My touch and nerve, even though you're just visualizing some public data. What were you curious about?

**Andrej Karpathy:**
[(38:06)](https://podwise.ai/dashboard/episodes/7559903?locate=2286)
Yeah, I guess I was curious, too. I mean, everyone is really thinking about the impacts of AI on the job market and what it's going to look like. So I was just interested to take a look. What does the job market look like? Where are the different roles? And how many people are in different professions? And I was really just interested to look through the individual cases and try to think myself about with these AIs and how they're likely to evolve. Are these going to be tools that people are using? Are these going to be displacing tools for these professions? And like, what are the current professions and how are they going to change? Are they going to grow or adjust to a large extent?

[(38:42)](https://podwise.ai/dashboard/episodes/7559903?locate=2322)
Or like, what could be new professions? So it's really just like a way to fuel my own chain of thought about the industry, I suppose. And so, yeah, the jobs data basically is just a Bureau of Labor Statistics. They actually have a percent outlook for each profession about how much it's expected to grow over the next,  I think, almost a decade. Yeah, I think it's a decade, but it was made in 2024. We need a lot of healthcare workers. Yeah. So they've already made those projections. And I'm not sure actually 100% what the methodology was that they put into the projections.

[(39:11)](https://podwise.ai/dashboard/episodes/7559903?locate=2351)
I guess I was interested to color things by like if people think that what's like primarily being developed now is this kind of like more digital AI. That it's kind of like almost like these ghosts or spirit entities that can like interact in the digital world and manipulate a lot of like digital information. And they currently don't really have a physical embodiment or presence. And the physical stuff is probably going to go slightly slower because you're manipulating atoms. So flipping bits and the ability to copy paste digital information is like makes everything a million times faster than accelerating matter,  you know.

[(39:43)](https://podwise.ai/dashboard/episodes/7559903?locate=2383)
We're going to see a huge amount of activity in the digital space, a huge amount of rewriting,  a huge amount of activity, boiling soup. We're going to see something that in the digital space goes at the speed of light compared to what's going to happen in the physical world to some extent. It would be the extrapolation. And so I think like, there's currently kind of like, I think, overhang,  where there can be like a lot of unhuddling,  almost potentially of like a lot of digital information processing that used to be done by computers and people. And now with AI as like a third kind of manipulative digital information,  there's gonna be a lot of refactoring in those disciplines.

[(40:19)](https://podwise.ai/dashboard/episodes/7559903?locate=2419)
But the physical world is actually gonna be like, I think, behind that by some amount of time. And so I think what's really fascinating to me is like,  So that's why I was highlighting the professions that fundamentally manipulate digital information. This is work you could do from your home, etc. Because I feel like things will change. And that doesn't mean that there's going to be less of those jobs or more of those jobs,  because that has to do with demand elasticity and many other factors. But things will change in these professions because of these new tools and because of this upgrade to the nervous system of the human superorganism,  if you want to think about it that way.

**Sarah Guo:**
[(40:52)](https://podwise.ai/dashboard/episodes/7559903?locate=2452)
Given the look you had at the data,  do you have either any observations or guidance for people facing the job market or thinking about what to study now or what skills to develop? I mean, we can all go get like,  I'm very thankful that I have to like meet people for my job right now. Yeah, more physical.

**Andrej Karpathy:**
[(41:09)](https://podwise.ai/dashboard/episodes/7559903?locate=2469)
Could you do your work from home though? I could.

**Sarah Guo:**
[(41:12)](https://podwise.ai/dashboard/episodes/7559903?locate=2472)
I think there are relationship parts of it that are hard, but most of it I could.

**Andrej Karpathy:**
[(41:16)](https://podwise.ai/dashboard/episodes/7559903?locate=2476)
Yeah, I think it's really hard to tell because again, like the job market is extremely diverse. I think the answers will probably vary. But to a large extent, like these tools are extremely new, extremely powerful. And so just being, you know, just trying to keep up with it is like the first thing. And yeah, because I think a lot of people kind of like dismiss it,  or they're afraid of it, or they're afraid of it, etc. Which is totally understandable, of course. Yeah, I think like, it's fundamentally an empowering tool at the moment. And these jobs are bundles of tasks. And some of these tasks can go a lot faster. So people should think of it as primarily a tool that it is right now.

[(41:48)](https://podwise.ai/dashboard/episodes/7559903?locate=2508)
And I think the long-term future of that is uncertain. Yeah, it's kind of really hard to forecast, to be honest. And I'm not professionally doing that, really. And I think it's the job of economists to do it properly.

**Sarah Guo:**
[(41:59)](https://podwise.ai/dashboard/episodes/7559903?locate=2519)
You are an engineer, though. And one thing I thought was interesting is that the demand for engineering jobs It's continuing to increase. I can't tell if that's like a temporary phenomenon. I'm not sure how I feel about it yet. Do you know?

**Andrej Karpathy:**
[(42:13)](https://podwise.ai/dashboard/episodes/7559903?locate=2533)
Yeah, that's like the demand analysis almost like software was scarce, right? And so the reason we don't have more demand for software is just scarcity and it's too expensive.

**Sarah Guo:**
[(42:21)](https://podwise.ai/dashboard/episodes/7559903?locate=2541)
Too expensive, yeah.

**Andrej Karpathy:**
[(42:22)](https://podwise.ai/dashboard/episodes/7559903?locate=2542)
So if the barrier comes down, then actually you have the Jevons paradox, which is like,  you know, actually the demand for software actually goes up. It's cheaper and there's more powerful. The classical example of this always is the ATMs and the bank tellers. Because there was a lot of like fear that ATMs and computers basically would displace tellers. But what happened is they made like the cost of operation of a bank branch much cheaper,  as there were more bank branches, so there were more tellers. It's like the canonical example people cite. But basically, it's just Jevin's paradox, like something becomes cheaper. So there's a lot of unlocked demand for it.

[(42:57)](https://podwise.ai/dashboard/episodes/7559903?locate=2577)
So I do think that that's probably, I do have like a cautiously optimistic view of this in software engineering,  where I do, it does seem to me like the demand for software will be extremely large. And it's just become a lot cheaper. And so I do think that for quite some time, It's very hard to forecast,  but it does seem to me like right now, at least locally,  there's going to be more demand for software because software is amazing. It's like, you know, digital information processing. You're not forced to use like arbitrary tools that are given to you. There are imperfections in various ways. You're not forced to subscribe to what exists.

[(43:30)](https://podwise.ai/dashboard/episodes/7559903?locate=2610)
Code is now ephemeral and it can change and can be modified. And so I think there's going to be a lot of activity in the digital space to like rewire everything in a certain sense. And I think it's going to create a lot of demand for this kind of stuff. I think long term, yeah, obviously, even with auto research, like OpenAI or, you know,  Anthropic or these other labs, like they're employing what, like 1000 something researchers, right? These researchers are basically like glorified. You know, they're like automating themselves away, like actively. And this is like the thing they're all trying to do. Yeah, I think I went around.

**Sarah Guo:**
[(44:04)](https://podwise.ai/dashboard/episodes/7559903?locate=2644)
Some of those researchers also feel that feel the psychosis, right? Yeah, it's working.

**Andrej Karpathy:**
[(44:08)](https://podwise.ai/dashboard/episodes/7559903?locate=2648)
Yeah.

**Sarah Guo:**
[(44:08)](https://podwise.ai/dashboard/episodes/7559903?locate=2648)
Right. And so they're like, Oh, it's over for me, too.

**Andrej Karpathy:**
[(44:11)](https://podwise.ai/dashboard/episodes/7559903?locate=2651)
I did spend a bunch of time going around opening. I was like, you guys realize if we're successful, like we're a lot of jobs,  like, like, it's just we're just building automation for Sam or something like that. Like I or the board. I'm not sure. We're just dealing with this automation for, yeah, the board or the CEO or something like that. And we're all out of our job and maybe contributing on the sides. And so, yeah, it's kind of like nerving from that perspective.

**Sarah Guo:**
[(44:35)](https://podwise.ai/dashboard/episodes/7559903?locate=2675)
Is it okay if I ask you Noam's question? You know, you could be doing that, right? Auto-researching with a lot of compute scale and a bunch of colleagues at one of the Frontier Labs. Like, why not?

**Andrej Karpathy:**
[(44:45)](https://podwise.ai/dashboard/episodes/7559903?locate=2685)
Well, I was there for a while, right? And I did re-enter. To some extent, I agree, and I think that there are many ways to slice this question. It's a very loaded question. I will say that I feel very good about what people can contribute and their impact outside of the frontier labs,  obviously. Not in the industry, but also in more ecosystem level roles. So your role, for example, is more like ecosystem level. My role currently is also kind of more on ecosystem level. And I feel very good about the impact that people can have in those kinds of roles. I think conversely, there are definite problems in my mind for basically aligning yourself way too much with the frontier labs too.

[(45:20)](https://podwise.ai/dashboard/episodes/7559903?locate=2720)
So fundamentally, I mean, you have a huge amount of financial incentive with these frontier labs. And by your own admission, the AIs are going to really change humanity and society in very dramatic ways. And here you are basically building the technology and benefiting from it and being very allied to it through financial means. Like this was a conundrum that was in at the heart of, you know,  how OpenAI was started in the beginning. Like this was the conundrum that we were trying to solve. And so, you know, so it's kind of. It's still not fully resolved. That's number one. You're not a completely free agent and you can't actually like be part of that conversation in a fully autonomous,  free way.

[(45:59)](https://podwise.ai/dashboard/episodes/7559903?locate=2759)
Like if you're inside one of the Frontier Labs, like there's some things that you can't say. And conversely, there are certain things that the organization wants you to say. And you know, they're not going to twist your arm. you feel the pressure of like what you should be saying, you know, because like,  obviously, otherwise, it's like really awkward conversations, strange side eyes, like what are you doing,  you know, so you can't like really be an independent agent. And I, I feel like a bit more a lot like aligned with humanity in a certain sense outside of Frontier Lab,  because I don't, I'm not subject to those pressures almost, right. And I can't say whatever I want.

[(46:31)](https://podwise.ai/dashboard/episodes/7559903?locate=2791)
Or, yeah, I would say in the Frontier Labs, like, You can have impact there, of course, as well. But there's many researchers, and maybe you're one of them. Maybe your ideas are really good, etc. Maybe there's a lot of decision-making to do,  and you want to be in a position where you are in the room with those conversations when they come up. I do think that currently the stakes are overall fairly low, and so everything is kind of nice. But ultimately, at the end of the day, when the stakes are really high,  etc., if you're an employee at an organization,  I don't actually know how much sway you're going to have on the organization and what it's going to do fundamentally at the end of the day.

[(47:02)](https://podwise.ai/dashboard/episodes/7559903?locate=2822)
You're not really in charge. You're in a room and you're contributing ideas,  but you're not really in charge of that entity that you're a part of. So those are some sources of misalignment, I think, to some extent. I will say that in one way, I do agree a lot with that sentiment. I do feel like the labs, for better or worse, they're opaque and a lot of work is there. And they're kind of like at the edge of capability and what's possible. And they're working on what's coming down the line. And I think if you're outside of that frontier lab,  your judgment fundamentally will start to drift because you're not part of the,  you know, What's coming down the line, right?

[(47:34)](https://podwise.ai/dashboard/episodes/7559903?locate=2854)
And so I feel like my judgment will inevitably start to drift as well. And I won't actually have an understanding of how these systems actually work under the hood. That's an opaque system. I won't have a good understanding of how it's going to develop and etc. And so I do think that in that sense, I agree and it's something I'm nervous about. I think it's worth basically being in touch with what's actually happening and actually being in the Frontier Lab. And if some of the Frontier Labs would have me come for, you know,  some amount of time and do really good work for them, and then maybe come in and out.

**Sarah Guo:**
[(48:00)](https://podwise.ai/dashboard/episodes/7559903?locate=2880)
Guys, he's looking for a job. This is super exciting.

**Andrej Karpathy:**
[(48:02)](https://podwise.ai/dashboard/episodes/7559903?locate=2882)
Then I think that's maybe a good setup because I kind of feel like it kind of,  you know, Maybe that's like one way to actually be connected to what's actually happening,  but also not feel like you're necessarily fully controlled by those entities. So I think, honestly, in my mind, Noam can probably do extremely good work at OAI,  but also I think his most impactful work could very well be outside of OpenAI.

**Sarah Guo:**
[(48:26)](https://podwise.ai/dashboard/episodes/7559903?locate=2906)
Noam, that's a call to be an independent researcher with AutoResearch.

**Andrej Karpathy:**
[(48:30)](https://podwise.ai/dashboard/episodes/7559903?locate=2910)
Yeah, there's many things to do on the outside. And I think ultimately, I think the ideal solution maybe is like, yeah, going back and forth. Or, yeah, and I think fundamentally, you can have really amazing impact in both places. So very complicated. I don't know, like, it's a very loaded question a little bit. But I mean, I joined the Frontier Lab, and I'm outside. And then maybe in the future, I'll want to join again. And I think that's kind of like how I look at it.

**Sarah Guo:**
[(48:54)](https://podwise.ai/dashboard/episodes/7559903?locate=2934)
One question related to what visibility to does the world or the AI ecosystem have into the frontier is like,  how close open sources to the frontier and how sustainable that is. I think, yeah, I think it's quite Surprising,  the entire sequence of events actually from like having a handful of Chinese models and global models. And I think people are going to continue releasing here in the near term that are closer than much of the industry anticipated from a capability perspective. I don't know if you're surprised by that, but you're a long-term contributor to open source. Like what's your prediction here? Yeah.

**Andrej Karpathy:**
[(49:31)](https://podwise.ai/dashboard/episodes/7559903?locate=2971)
So roughly speaking, basically the, yeah, the close models are ahead,  but like people are monitoring the number of months that sort of like open source models are behind.

**Sarah Guo:**
[(49:38)](https://podwise.ai/dashboard/episodes/7559903?locate=2978)
And to start with, there's nothing, and then it went to 18 months.

**Andrej Karpathy:**
[(49:41)](https://podwise.ai/dashboard/episodes/7559903?locate=2981)
Yeah, and there's been a convergence, right? So maybe they're behind by like, what is the latest? Maybe like eight months, six months, eight months kind of thing right now. Yeah, I'm a huge fan of open source, obviously. So for example, in operating systems, you have like Windows and MacOS. These are large software projects, kind of like what LLMs are going to become. And there's Linux, but Linux is very easy. Like actually, Linux is an extremely successful project. It runs on the vast majority of computers. Like last time I checked, was it like 60% or something like around Linux? And that's because there is a need in the industry to have a common open platform that everyone feels sort of safe using.

[(50:12)](https://podwise.ai/dashboard/episodes/7559903?locate=3012)
I would say like the industry has always felt a demand for that kind of a project to exist. And I think the same is true now. And that's why businesses actually want there's demand for this kind of a thing to exist. The big difference is that everything is capital. There's a lot of capex that goes into this. And so I think that's where things fall apart a little bit and make it a bit harder to compete in a certain sense. I do think that the current models are very good. The other thing that I think is really interesting is that for the vast majority of consumer use cases and things like that,  even the current open source models are actually quite good, I would say.

[(50:42)](https://podwise.ai/dashboard/episodes/7559903?locate=3042)
And I think if you go forward more years,  it does seem to me like a huge amount of simple use cases are going to be well covered and actually even run locally. But there's going to be always like some demand for like frontier intelligence and that that can actually be extremely large piece of the pie. But it could be that the frontier, the need for frontier intelligence is going to be like,  you know, Nobel Prize kind of work or like let's move Linux from C to Rust. It's going to be like bigger projects, you know, like scoped in that kind of a way. And there's going to be maybe more. And maybe that's where a lot of the frontier closed intelligences are going to be interacting with.

[(51:19)](https://podwise.ai/dashboard/episodes/7559903?locate=3079)
And open source is going to eat through a lot of the more basic use cases or something like that. You know, at some point, what is frontier today is going to be, you know,  probably later this year, what's frontier today in terms of what I'm using right now from the closed labs. might be open source, and that's going to be doing a lot of work. So I kind of expect that this dynamic will actually basically continue. Like we'll have frontier labs that have closed AIs that are kind of like these oracles. And then we'll have open source kind of like behind for some amount of months. And I kind of expect that to continue. And I actually think that's like a pretty, pretty good setup overall.

[(51:51)](https://podwise.ai/dashboard/episodes/7559903?locate=3111)
Because I'm a little bit hesitant of having, I don't actually think it's like structurally,  I think there's some systemic risk attached to just having intelligences that are closed. And that's like, that's it. And I think that that's a, you know,  centralization has a very poor track record in my view,  in the past, and has- You mean like in political or economic systems in general? Yes. Exactly. I think there's like a lot of- Spoken like an Eastern European. A lot of pretty bad presidents. So I want there to be a thing that is maybe not at the edge of capability because it's new and unexplored,  etc. But I want there to be a thing that's behind.

[(52:23)](https://podwise.ai/dashboard/episodes/7559903?locate=3143)
And that is kind of like a common working space for intelligences that the entire industry has access to. Yeah, that seems to me like a pretty decent power balance for the industry.

**Sarah Guo:**
[(52:30)](https://podwise.ai/dashboard/episodes/7559903?locate=3150)
Yeah, I was just like, there are many problems to solve, right? Like, if you keep advancing intelligence, from the frontier, we can do new things. And there are a lot of like very big problems for humanity. Yeah, right. Yeah. It seems that that will continue to be a very expensive game. And so I want to like root for labs that are doing that because there are problems we cannot solve without continuing to advance the models in a very expensive way. And yet, as you point out, if what we have Today, as Frontier is open,  that's a lot of capability, right? And so I think, you know, the power of that or the democratization of that seems like very useful and also healthy.

**Andrej Karpathy:**
[(53:06)](https://podwise.ai/dashboard/episodes/7559903?locate=3186)
Yeah, I think basically by accident, we're actually like in an okay spot. By accident, we happen to be in a good spot, in a certain sense.

**Sarah Guo:**
[(53:14)](https://podwise.ai/dashboard/episodes/7559903?locate=3194)
Well, and to some degree, the longer this endures, like this dynamic,  the healthier of a spot like the ecosystem might be in,  right? Because you have more and more area under the curve.

**Andrej Karpathy:**
[(53:26)](https://podwise.ai/dashboard/episodes/7559903?locate=3206)
And I will say that even on the close side,  I almost feel like it's been like even further centralizing recently,  because I think a lot of the front runners are like not necessarily like the top tier. And so, yeah, like in that sense, I think it's not super ideal. I would love there to be more, more frontier labs, because I'm like, by default,  very suspicious of like, I want there to be more people in the room. I think in machine learning, ensembles always outperform any individual model. And so I want there to be ensembles of people thinking about all the hardest problems. And I want there to be ensembles of people in a room to be all well-informed and to make all those decisions.

[(54:00)](https://podwise.ai/dashboard/episodes/7559903?locate=3240)
So I don't want it to be like a closed doors with two people or three people. I feel like that's not a good future. I almost wish there were more labs is long story short. And I do think that open source has a place to play. I hope it sticks around. It's currently slightly behind, and that's actually kind of like a good thing.

**Sarah Guo:**
[(54:18)](https://podwise.ai/dashboard/episodes/7559903?locate=3258)
Okay. You worked on the precursor to generalized robotics, autonomy, in cars, right? A lot has happened in the last couple months with robotics companies as well,  like acceleration of really impressive generalization of environment, of tasks, like increasing long horizon tasks,  lots of money going into the space. Is it going to happen? Has anything in your view changed recently?

**Andrej Karpathy:**
[(54:42)](https://podwise.ai/dashboard/episodes/7559903?locate=3282)
So like my view is kind of informed by what I saw in self-driving. And I do feel like self-driving is the first robotics application. So probably what I saw is at the time, like 10 years ago, there were a large number of startups. And I kind of feel like most of them basically didn't long-term make it. And what I saw is that like a lot of capital expenditure had to go in and a lot of time. And so I think robotics, because it's so difficult and so messy and requires a huge amount of capital investment and a lot of conviction,  it's like a big problem. And I think items are really hard. So I kind of feel like it will lag behind what's going to happen in digital space.

[(55:17)](https://podwise.ai/dashboard/episodes/7559903?locate=3317)
And in digital space, there's going to be a huge amount of unhobbling,  basically like things that weren't super efficient becoming a lot more efficient by like a factor of 100,  because bits are so much easier. And so I think currently in terms of what's going to change and Like where the activity is,  I kind of feel like digital space is going to like change a huge amount. And then the physical space will lag behind. And what I find very interesting is like this interface in between them as well. Because I think in this like If we do have more agents acting on behalf of humans and more agents kind of like talking to each other and doing tasks and participating in the kind of economy of agents,

[(55:51)](https://podwise.ai/dashboard/episodes/7559903?locate=3351)
 et cetera, you're going to run out of things that you're going to do purely in a digital space. At some point, you have to go to the universe and you have to ask it questions. You have to run an experiment and see what the universe tells you to get back to learn something. And so we currently have a huge amount of like digital work because there's an overhang in how much we collectively thought about what already is digital. So we just didn't have enough thinking cycles among the humans to think about all the information that is already digital and already uploaded. And so we're going to start running out of stuff that is actually like already uploaded.

[(56:23)](https://podwise.ai/dashboard/episodes/7559903?locate=3383)
So you're going to at some point read all the papers and process them and have some ideas about what to try. But yeah, we're just going to... I don't actually know how much you can like get intelligence that's like fully closed off and was just information that's filled to it,  you know. And so I think what's going to happen is first there's going to be a huge amount of unhobbling and I think there's a huge amount of work there. Then actually it's going to move to like the interfaces between physical and digital. So and that's like sensors of like seeing the world and actuators of like doing something to the world.

[(56:48)](https://podwise.ai/dashboard/episodes/7559903?locate=3408)
So I think a lot of interesting companies will actually come from that interface of like can we feed the super intelligence in a certain sense,  data, and can we actually like take data out and manipulate the physical world per its bidding,  if you want to like anthropomorphize the whole thing, right? And then the physical world, actually, I almost feel like the total addressable market,  et cetera, in terms of like the amount of work and so on is massive,  possibly even much larger, maybe what can happen in digital space. So I actually think it's like a much bigger opportunity as well. I do feel like it's a huge amount of work, and in my mind,  the atoms are just like a million times harder.

[(57:24)](https://podwise.ai/dashboard/episodes/7559903?locate=3444)
So it will lag behind, but it's also, I think, a little bit of a bigger market. So it's kind of like, yeah, I think the opportunities kind of like follow that kind of trajectory. So right now, digital is like my main interest. Then interfaces would be like after that. And then maybe like some of the physical things,  like their time will come and they'll be huge when they do come.

**Sarah Guo:**
[(57:43)](https://podwise.ai/dashboard/episodes/7559903?locate=3463)
Well, it's an interesting framework for it too because certain things,  not the things I'm working on right now,  but certain things are much easier even in the world of atoms, right? Like if you just think about like read and write to the physical world,  like read sensors, cameras,  like there's a lot of existing hardware and you can imagine like enriching agent capabilities or capturing a lot of new data if you're just clever about it and like you don't necessarily have to invest a lot to like get something valuable.

**Andrej Karpathy:**
[(58:11)](https://podwise.ai/dashboard/episodes/7559903?locate=3491)
Yeah, so like examples of this that I saw, for example, are, you know,  a friend of mine, Liam, is a CEO of Periodic. I visited them last week. So it's just on top of mind. Like they're trying to do auto research for material science. And so in that case, it's like the sensors to the intelligence are actually like pretty expensive lab equipment. And the same is true in biology. I think a lot of people are very interested in engineering biology. And you know, the sensors will be more than just like video cameras, if that makes sense. And then the other thing I saw, for example, is companies that are trying to have,  like, you basically pay people for training data, as an example.

**Sarah Guo:**
[(58:42)](https://podwise.ai/dashboard/episodes/7559903?locate=3522)
Yeah, programmatically.

**Andrej Karpathy:**
[(58:43)](https://podwise.ai/dashboard/episodes/7559903?locate=3523)
Yeah, to feed the Borg. And so, like, these are all examples of, like, sensors in a certain sense. So they take many diverse shapes and forms, if that makes sense.

**Sarah Guo:**
[(58:52)](https://podwise.ai/dashboard/episodes/7559903?locate=3532)
Yeah,  so I'm looking forward to the point where I can ask for a task in the physical world and I can put a price on it and just tell the agent,  like, you know, you figure out how to do it. Go get the data.

**Andrej Karpathy:**
[(59:02)](https://podwise.ai/dashboard/episodes/7559903?locate=3542)
I'm actually kind of surprised we don't have enough, like, information markets. Like if, for example, if PolyMarket or other betting markets or even stocks, et cetera,  if they have so much autonomous activity and rising amount of activity, like, For example,  if Iran was just happening now,  how come there isn't a process where taking a photo or a video from somewhere in Tehran should cost like 10 bucks? Someone should be able to pay for that. And that's an example of feeding the intelligence. There's not going to be a human looking at it. It's going to be agents who are trying to guess the betting games and stock markets and so on.

[(59:30)](https://podwise.ai/dashboard/episodes/7559903?locate=3570)
So I kind of feel like the agentic web is still fairly new, that there's no mechanisms for this. But this is an example of what I think might happen. There's a good book that maybe is inspiring called Damon. In Damon, the intelligence ends up like puppeteering almost a little bit like humanity in a certain sense, you know. And so humans are kind of like its actuators, but humans are also like its sensors. And so I think like collectively, like society will kind of like reshape in a certain way to serve that kind of a purpose. That will kind of like end up happening collectively across the industry where, yeah,

[(1:00:05)](https://podwise.ai/dashboard/episodes/7559903?locate=3605)
 there's just a lot more automation and has certain needs and kind of humans will be serving those needs of that machine,  not necessarily like to each other.

**Sarah Guo:**
[(1:00:12)](https://podwise.ai/dashboard/episodes/7559903?locate=3612)
But we were on this very specific point of like missing pieces of training data. We needed something like auto research, right? Like we need the training cycle or the SFT piece to be far more mechanized.

**Andrej Karpathy:**
[(1:00:27)](https://podwise.ai/dashboard/episodes/7559903?locate=3627)
For which part?

**Sarah Guo:**
[(1:00:28)](https://podwise.ai/dashboard/episodes/7559903?locate=3628)
In order to take the human out of the loop to ask for a task that is just like improve my model quality with new data. Does that make sense to you? If you can't have the model do the training run by itself,  then your ability to do this as a closed loop task by pricing data is more challenged.

**Andrej Karpathy:**
[(1:00:55)](https://podwise.ai/dashboard/episodes/7559903?locate=3655)
Yes, 100%. But the thing is for LLM training, it actually is like very easily, it like really fits the paradigm. So you'd actually get a clean metric. Yeah, like LLM training actually fits the paradigm really well, really easily,  like all the optimization of all the code and so it runs faster. And then you also have like metrics that you can optimize against. I do think that if you had an autonomous loop over those metrics,  there's gonna be a lot of like good harding going on where the system will like overfit to those metrics. And so but then you can use the system to devise more metrics and you just have really good coverage. So it's kind of hard to tell.

[(1:01:27)](https://podwise.ai/dashboard/episodes/7559903?locate=3687)
In a certain sense, it's like a pretty, pretty good fit.

**Sarah Guo:**
[(1:01:30)](https://podwise.ai/dashboard/episodes/7559903?locate=3690)
I want to talk about a little tiny side project you have before we end. Tell me about the MicroGPT.

**Andrej Karpathy:**
[(1:01:36)](https://podwise.ai/dashboard/episodes/7559903?locate=3696)
Oh, yeah. Okay, so MicroGPT. So I have this like running obsession of like maybe a decade or two of just like simplifying and boiling down the basically LLMs to like their bare essence. And I've had a number of projects along these lines, so like NanoGPT and MakeMore and MicroGrad, etc. So I feel like MicroGPT is now the state of the art of me trying to like just boil it down to just the essence. Because the thing is like training neural nets and LLMs specifically is a huge amount of code. But all of that code is actually complexity from efficiency. It's just because you need it to go fast. If you don't need it to go fast and you just care about the algorithm,

[(1:02:13)](https://podwise.ai/dashboard/episodes/7559903?locate=3733)
 then that algorithm actually is 200 lines of Python. Very simple to read. And this includes comments and everything. Because you just have like your data set, which is a text. And you need your neural network architecture, which is like 50 lines, you need to do your forward pass,  and then you have to do your backward pass to calculate the gradients. And so an autograd engine to calculate the gradients is like 100 lines. And then you need an optimizer, an atom, for example,  which is a very state-of-the-art optimizer is like,  again, 10 lines, really. And so putting everything together in the training loop is like, yeah, 200 lines.

[(1:02:43)](https://podwise.ai/dashboard/episodes/7559903?locate=3763)
And what's interesting to me, like normally before Like, maybe a year ago or more,  if I had come up with MicroGPT, I would be tempted to basically explain to people. Like, I have a video, like, stepping through it or something like that. And I actually tried to make that video a little bit. And I tried to make, like, a little guide to it and so on. But I kind of realized that this is not really,  it's not really adding too much because people,  because it's already so simple that it's 200 lines that anyone could ask their agent to explain it in various ways. And the agents, like, I'm not explaining to people anymore. I'm explaining it to agents. If you can explain it to agents,

[(1:03:15)](https://podwise.ai/dashboard/episodes/7559903?locate=3795)
 then agents can be the router and they can actually target it to the human in their language with infinite patience and just at their capability and so on.

**Sarah Guo:**
[(1:03:25)](https://podwise.ai/dashboard/episodes/7559903?locate=3805)
Right. If I don't understand this particular function, I can ask the agent to explain it to me like three different ways. And I'm not going to get that from you.

**Andrej Karpathy:**
[(1:03:33)](https://podwise.ai/dashboard/episodes/7559903?locate=3813)
And so I kind of feel like, you know, what is education? Like it used to be guides. It used to be lectures. It used to be this thing. But I feel like now more I'm explaining things to agents and maybe I'm coming up with skills where Basically,  skill is just a way to instruct the agent how to teach the thing. So maybe I could have a skill for MicroGPT of the progression I imagine the agent should take you through if you're interested in understanding the code base. And it's just like hints to the model to like, oh, first start off with this and then with that. And so I could just script the curriculum a little bit as a skill.

[(1:04:04)](https://podwise.ai/dashboard/episodes/7559903?locate=3844)
So I don't feel like, yeah, I feel like there's gonna be less of like explaining things directly to people. And it's gonna be more of just like, does the agent get it? And if the agent gets it, they'll do the explanation. And we're not fully there yet, because they, I still can,  I still think I can probably explain things a little bit better than the agents. But I still feel like the models are improving so rapidly that I feel like it's a losing battle to some extent. And so I think education is going to be kind of like reshuffled by this quite substantially,  where it's the end of like teaching each other things a little bit. Like if I have a library, for example, of code or something like that,

[(1:04:40)](https://podwise.ai/dashboard/episodes/7559903?locate=3880)
 it used to be that you have documentation for other people who are going to use your library. But like you shouldn't do that anymore. Like you should have instead of HTML documents for humans, you have Markdown documents for agents,  because if agents get it, then they can just explain all the different parts of it. So it's this redirection through agents, you know. And that's like, so I think we're going to see a lot more of that playing out.

**Sarah Guo:**
[(1:05:00)](https://podwise.ai/dashboard/episodes/7559903?locate=3900)
Well, we'll see if the great teachers know, like develop intuition for how to explain things to agents differently.

**Andrej Karpathy:**
[(1:05:06)](https://podwise.ai/dashboard/episodes/7559903?locate=3906)
Ultimately, so for example, MicroGPT, like I asked, I tried to get an agent to write MicroGPT. So I told them, like, try to boil down the simplest things,  like try to boil down neural network stream to the simplest thing and can't do it. Like MicroGPT is like my It's like end of my obsession. It's the 200 lies. I thought about this for a long time. I've obsessed about this for a long time. This is the solution. Trust me, it can't get simpler. And this is my value add. Everything else, like agent gets it. It just can't come up with it, but it totally gets it and understands why it's done in a certain way,  et cetera. So like my contribution is kind of like these few bits,

[(1:05:41)](https://podwise.ai/dashboard/episodes/7559903?locate=3941)
 but everything else in terms of like the education that goes on after that is like not my domain anymore. So maybe, yeah,  it's like education kind of changes in those ways where you kind of have to infuse the few bits that you feel strongly about the curriculum or the better way of explaining it or something like that. The things that agents can't do is your job now. Things that agents can do, they can probably do better than you or like very soon. And so you should be strategic about what you're actually spending time on.

**Sarah Guo:**
[(1:06:07)](https://podwise.ai/dashboard/episodes/7559903?locate=3967)
Well, we appreciate the few things. Thank you, Andrej.

**Andrej Karpathy:**
[(1:06:10)](https://podwise.ai/dashboard/episodes/7559903?locate=3970)
Okay.

**Sarah Guo:**
[(1:06:12)](https://podwise.ai/dashboard/episodes/7559903?locate=3972)
Find us on Twitter at NoPriorsPod. Subscribe to our YouTube channel if you want to see our faces. Follow the show on Apple Podcasts, Spotify or wherever you listen. That way you get a new episode every week. And sign up for emails or find transcripts for every episode at no-priors.com.

