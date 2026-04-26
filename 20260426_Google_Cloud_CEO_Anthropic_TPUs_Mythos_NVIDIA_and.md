---
podcast: "Matthew Berman"
episode: "Google Cloud CEO: Anthropic, TPUs, Mythos, NVIDIA and more"
link: https://podwise.ai/dashboard/episodes/7843975
publish-time: "2026-04-24"
save-time: "2026-04-26"
---
# Summary

Google Cloud CEO Thomas Kurian details how the company maintains a competitive edge in AI infrastructure by leveraging proprietary TPU silicon and long-term capital planning. By controlling the full stack—from chip manufacturing to data center deployment—Google avoids the compute constraints faced by other frontier labs while simultaneously monetizing tokens and hardware for third-party competitors. The discussion highlights the shift toward agentic workflows, where AI models autonomously manage tasks across enterprise systems, necessitating specialized inference chips and ultra-low latency storage. Kurian emphasizes that Google’s strategy balances internal model development with broad platform services, including continuous red teaming and automated code repair to address cybersecurity risks. As demand for compute grows, Google prioritizes energy efficiency and distributed data center deployment to sustain long-term growth and support the next generation of 10-trillion-parameter models.

# Takeaways

* Owning the full technology stack—from custom silicon design to data center manufacturing—provides a sustainable competitive advantage in a market where compute capacity is chronically constrained.
* TPUs are transitioning from AI-specific accelerators into general-purpose infrastructure, with significant adoption in capital markets and high-performance computing sectors.
* Shifting data center deployment from traditional construction to a manufacturing-based model, where entire rows of machines are pre-tested and deployed, significantly reduces cycle times and increases scalability.
* Agentic AI, which involves delegating multi-step tasks and computer control to models, requires specialized memory management and storage architectures to maintain cost-effectiveness for consumer-facing applications.
* Separating hardware into dedicated training and inference chips optimizes unit economics and energy efficiency, providing a necessary financial buffer to fund the massive capital requirements of AI development.
* The emergence of AI-driven cyber threats necessitates a shift toward "continuous red teaming" and automated code repair, where models are used to identify and patch vulnerabilities at a speed impossible for human teams.
* Software engineering productivity is increasingly defined by functional output rather than lines of code, with AI tools handling debugging and security reviews to augment the efficiency of senior engineering talent.
* Popular open-source libraries represent the largest attack surface for AI-assisted cyber threats, requiring proactive, automated hardening to maintain the security of the broader software ecosystem.

# Q & A

**Q: Why does Google have sufficient TPU capacity when other frontier labs like OpenAI and Anthropic are constantly compute-constrained?**

A: Our ability to maintain capacity comes from years of long-term planning and a multi-layered strategy. We diversified our energy sources and locked in real estate for data centers well before the current AI surge. Critically, we shifted our data center deployment model from traditional construction to manufacturing. By deploying capacity at a higher granularity—such as entire rows or racks of machines that are pre-tested in a central location—we significantly reduced our cycle time. Furthermore, because we have been building our own silicon for over a decade, we are not solely dependent on external supply chains. We see our TPUs as general-purpose infrastructure, serving our own Gemini models, other AI labs, and even high-performance computing customers like the Department of Energy, which allows us to aggregate demand and secure favorable terms from our supply chain vendors.

---

**Q: If AGI is the ultimate goal, why not hoard all your compute capacity for your own models instead of selling it to competitors?**

A: You have to generate sufficient cash flow to fund this level of R&D. Venture capital cannot fund these companies indefinitely; as compute costs scale, the business must become self-sustaining. We view selling compute as a lever to generate that cash flow. We balance our investments across our own internal needs, our capital requirements, and the needs of our customers. If you are running a loss-leader business without making enough money from inference to cover the massive costs of training, your options become very limited as the gap widens. By monetizing our infrastructure, we ensure we have the resources to continue innovating.

---

**Q: How do you change the hearts and minds of the broader U.S. demographic regarding the negative sentiment toward data centers and AI job displacement?**

A: We focus on demonstrating the tangible, positive impact of AI in society. For example, we work with the largest health insurer in Germany, where they use Gemini to assist agents. There was significant anxiety about job displacement, but they haven't let anyone go; instead, they reduced the time to research and answer complex customer queries from 23 minutes to a few seconds. We also work with the American Society for Clinical Oncology to help doctors navigate complex, overlapping care guidelines for patients with multiple conditions. By applying AI to solve real-world problems—like wealth management advice for average citizens through Citigroup or drug discovery for Merck—we show that AI is a tool for efficiency and quality, not just a replacement for labor.

---

**Q: What does the decision to split your 8th generation chips into separate inference and training-focused silicon tell us about the future of AI workloads?**

A: Workloads have evolved through three distinct phases. First, we had search-like experiences with many input tokens and fewer output tokens. Second, we moved to content generation, where the volume of output tokens grew significantly. Now, we are in the agentic phase. Agents need to maintain state in memory for long periods—potentially 6 to 12 hours—to perform tasks. This shift informed our chip design in several ways. We needed to optimize for the KV cache to avoid expensive memory shuffling and ensure the system can interact with classical compute machines. We also designed the inference chip to be air-cooled so it can be deployed in more locations to manage latency, whereas training can be centralized in large, water-cooled clusters.

---

**Q: Where do you see the next big bottleneck for artificial intelligence?**

A: The next bottleneck will be the cost of running virtual machines for consumer-facing agents. Right now, consumers cannot afford to have VMs running indefinitely to manage their tasks. If an agent is scheduling travel by interacting with eight different websites, it needs to be efficient. We need to engineer the cost structure so that we can activate and deactivate VMs instantly as tasks are completed. If we want to reach everyone, we have to solve the cost of local storage and compute overhead for these agentic workflows. That is why we are co-designing across the entire stack—from the agent model down to the storage and compute systems—to make that cost structure viable.

---

**Q: How do you reconcile the strategy of powering competitors like Anthropic while simultaneously competing with them in the enterprise market?**

A: Google is a platform company, and in a platform business, different parts of the organization will inevitably compete with different players. While we are determined to be best-in-class with Gemini and our enterprise toolchain, we also recognize that customers want choice and access to our TPU infrastructure. This is simply the nature of being a platform provider. We see this dynamic across the industry; for instance, Apple has signed a contract to use our models, even though that might seem to compete with our Android ecosystem. We focus on providing the best platform, and that includes supplying the infrastructure that allows others to build their own models.

---

**Q: How is Google adopting the frontier of agentic coding while maintaining high security and quality standards for your services?**

A: We use an internal coding harness called JetSki, and the feedback from our engineers feeds directly into the reinforcement loop for Gemini. We don't measure productivity by lines of code, as senior engineers write more compact, efficient code than junior ones. Instead, we focus on function and quality. We have integrated Gemini into our cloud to scan for security vulnerabilities automatically. We also use AI to assist in peer reviews, which allows senior engineers to focus on the most complex issues rather than being a bottleneck. Furthermore, we are introducing agents that perform continuous red teaming—constantly attacking our systems to identify vulnerabilities—and agents that assist in patching and deploying fixes, which is essential when shipping features at high velocity.

---

**Q: How do you address the risk of AI-driven cyber attacks, especially given that adversaries will likely use these models to scan popular open-source libraries?**

A: This is a reality we must manage by being faster on the defense than the attackers are on the offense. We have three practical responses. First, if models are used to find vulnerabilities, we must use models to help fix them, as humans cannot keep up with the volume of issues. Second, we use agents for continuous red teaming, as a monthly manual audit is no longer sufficient. Third, we build tools to help prioritize which vulnerabilities are the most critical to address first. While adversaries will target open-source libraries because they offer the largest surface area, we are active contributors to that community and will provide the tools to help them harden their code against these new AI-assisted threats.

# Outlines

## Strategic TPU Capacity Planning and Monetization
[(00:00)](https://podwise.ai/dashboard/episodes/7843975?locate=0)
Google maintains sufficient compute capacity through long-term planning, diversification of energy sources, and a shift from traditional construction to manufacturing for data centers. By owning proprietary silicon, the company avoids being compute-constrained, a common issue for other frontier labs. Monetization strategies include selling tokens, chips, and infrastructure access to diverse segments, including capital markets and high-performance computing. This diversification ensures consistent cash flow to fund ongoing R&D while balancing internal Gemini model requirements with external demand.

---

## Sustainable Data Center Deployment and Energy Efficiency
[(08:03)](https://podwise.ai/dashboard/episodes/7843975?locate=483)
Data center expansion focuses on minimizing local grid impact and maximizing energy efficiency. Strategies include investing in behind-the-meter energy technology, which allows for grid cross-connection during supply shortages, and utilizing advanced thermodynamic exchange for cooling. By distributing data centers across multiple locations rather than concentrating them in one area, the company reduces the burden on local resources. These facilities prioritize industry-leading Power Usage Effectiveness (PUE) to ensure minimal incremental energy consumption per megawatt of compute.

---

## Societal Impact and Enterprise Productivity
[(11:27)](https://podwise.ai/dashboard/episodes/7843975?locate=687)
AI adoption in the enterprise sector demonstrates significant efficiency gains without necessarily causing job displacement. Case studies include health insurers reducing research time from 23 minutes to seconds and oncology societies using AI to navigate complex treatment guidelines. While public concern regarding job displacement remains high, the focus is on applying technology to augment human capabilities. Internal productivity gains are being leveraged to increase hiring in go-to-market and engineering roles, particularly in cybersecurity, where agents are used for continuous red teaming and vulnerability detection.

---

## System-Level Co-Design and Chip Architecture
[(17:46)](https://podwise.ai/dashboard/episodes/7843975?locate=1066)
TPU performance is driven by system-level co-design rather than just silicon specifications. The architecture features high-bandwidth optical torus networks and massive memory capacity, enabling efficient training and inference. The decision to split chip development into specialized training (T) and inference (I) units reflects the evolving needs of AI workloads. This approach optimizes unit economics and energy efficiency, allowing for predictable latency and high throughput. The long-term strategy emphasizes compiler optimization and software stack integration, such as JAX and XLA, to maintain a competitive total cost of ownership.

---

## Agentic Workflows and Infrastructure Bottlenecks
[(24:32)](https://podwise.ai/dashboard/episodes/7843975?locate=1472)
The evolution of AI models from search-based chatbots to agentic systems capable of controlling computers and managing complex tasks has fundamentally changed infrastructure requirements. These agents necessitate longer memory retention and efficient storage solutions, such as the newly introduced managed Lustre and Rapid Storage systems. A primary future bottleneck is the cost of running virtual machines for consumer-facing agents, which requires engineering more efficient cost structures. Co-designing across the entire stack—from the agent down to the storage and compute layers—is essential to scaling these capabilities.

---

## Platform Strategy and Model Scaling
[(35:01)](https://podwise.ai/dashboard/episodes/7843975?locate=2101)
Operating as a platform company involves balancing internal model development with supplying competitors like Anthropic. This strategy allows for broad market reach and ecosystem growth. Scaling models to 10 trillion parameters remains feasible through disaggregated serving techniques that optimize throughput and memory usage. The focus is shifting toward using structured data and complex enterprise workflows to improve model accuracy and reasoning. Synthetic data and trajectory optimization harnesses are increasingly used to refine model performance, ensuring that scaling remains effective for both training and inference.

---

## Agentic Coding and Cybersecurity Defense
[(41:46)](https://podwise.ai/dashboard/episodes/7843975?locate=2506)
Agentic coding tools are transforming software engineering by automating debugging, code review, and vulnerability detection. While these tools increase shipping velocity, maintaining quality requires a hybrid approach where AI assists senior engineers in peer reviews. Cybersecurity is a critical focus, with agents deployed to perform continuous red teaming and automated patching. The industry faces the challenge of securing open-source libraries, which are primary targets for exploitation. The long-term goal is to build robust, self-correcting systems that can identify and fix vulnerabilities faster than human developers, ensuring secure deployment at scale.

# Keywords

|Keywords|Explanation|
|---|---|
|TPU (Tensor Processing Unit)|A custom-designed hardware accelerator developed by Google specifically to speed up machine learning tasks. In the transcript, it is described as a highly efficient, general-purpose infrastructure used for both training massive AI models and running inference.|
|Gemini|A family of multimodal AI models created by Google that can process and generate text, code, and media. The transcript highlights its role as a core component of Google's enterprise AI platform, used for tasks ranging from clinical research to financial advice.|
|AGI (Artificial General Intelligence)|A theoretical form of artificial intelligence that can perform any intellectual task that a human can do. The speakers discuss it as the long-term goal for many frontier AI labs, driving the intense demand for compute capacity.|
|Inference|The process of using a pre-trained AI model to generate answers, predictions, or content based on new input. The transcript emphasizes that as training costs rise, generating revenue through inference has become a critical business requirement for AI companies.|
|CUDA|A parallel computing platform and programming model developed by NVIDIA that allows software to use GPUs for general-purpose processing. It is mentioned as a key factor in the AI industry that helps deliver high performance and favorable economics for many developers.|
|JAX|An open-source machine learning framework developed by Google that is designed for high-performance research and numerical computing. It is cited as a vital part of the software stack that enables compiler optimization and efficient training on TPU hardware.|
|PUE (Power Usage Effectiveness)|A metric used to measure how efficiently a data center uses energy, calculated by the ratio of total power consumed to the power delivered to the IT equipment. The transcript notes that Google focuses on maintaining an industry-leading PUE to ensure their data centers are as sustainable as possible.|
|Lustre|A high-performance parallel file system designed for large-scale data storage and processing. It is mentioned in the transcript as a storage solution that enables massive datasets to be read quickly by large clusters of chips during the training process.|
|Tokens|The basic units of text or data that AI models process, which can represent parts of words or characters. The transcript explains that companies often monetize AI services by charging customers based on the number of tokens processed or generated.|
|Anthropic|An AI research and safety company known for developing the Claude series of models. The transcript identifies them as a significant player in the AI field that competes with Google while simultaneously relying on Google's TPU infrastructure for their computing needs.|

# Highlights

- [(03:43)](https://podwise.ai/dashboard/episodes/7843975?locate=223) We make great margins no matter how we sell it because we own our own IP. We are not just a distributor for other people's IP.
- [(06:12)](https://podwise.ai/dashboard/episodes/7843975?locate=372) Venture capital cannot fund you indefinitely. As compute costs grow, if you are not making enough money from inference to cover the cost of training, the number of sources you can go to gets smaller.
- [(07:02)](https://podwise.ai/dashboard/episodes/7843975?locate=422) It is better to have your own chips and demand than not having your own chips. If you don't, you are reselling other people's stuff.
- [(44:51)](https://podwise.ai/dashboard/episodes/7843975?locate=2691) The most complex computer in the world is a cloud. It makes a PC look like a toy.

# Transcript

**Speaker 1:**
[(00:00)](https://podwise.ai/dashboard/episodes/7843975?locate=0)
We're not just a distributor of other people's IP. We own our own IP.

**Matthew Berman:**
[(00:03)](https://podwise.ai/dashboard/episodes/7843975?locate=3)
But how do you change the hearts and the minds of the broader U.S. demographic with regards to artificial intelligence? Mythos, I think it's rumored to be the first 10 trillion parameter model.

**Speaker 1:**
[(00:17)](https://podwise.ai/dashboard/episodes/7843975?locate=17)
It's better to have your own chips and demand than not having your own chips.

**Matthew Berman:**
[(00:21)](https://podwise.ai/dashboard/episodes/7843975?locate=21)
Where's the next big bottleneck?

**Speaker 1:**
[(00:22)](https://podwise.ai/dashboard/episodes/7843975?locate=22)
The next big bottleneck will be largely around...

**Matthew Berman:**
[(00:25)](https://podwise.ai/dashboard/episodes/7843975?locate=25)
Is there some line in the sand, some benchmark you would determine Gemini is no longer safe to release publicly?

**Speaker 1:**
[(00:31)](https://podwise.ai/dashboard/episodes/7843975?locate=31)
We have more demand than we can possibly meet from all the other AI labs.

**Matthew Berman:**
[(00:36)](https://podwise.ai/dashboard/episodes/7843975?locate=36)
Thomas, what keeps you up at night? All right, Thomas, thank you for joining me today. We're at the Google Cloud campus and I really appreciate your time today.

**Speaker 1:**
[(00:47)](https://podwise.ai/dashboard/episodes/7843975?locate=47)
Thanks for having me.

**Matthew Berman:**
[(00:48)](https://podwise.ai/dashboard/episodes/7843975?locate=48)
I am super excited to talk to you. I have a bunch of questions for you. The first question I've been thinking about so much lately is TPU capacity. When you look at the other frontier labs like Anthropic and OpenAI, all they talk about is being compute constrained. But then you see Google over here who, you know, you have the full stack,  you have your own chips, But you're not only serving your own inference, you're training,  you're selling inference. You are also allowing some of your competitors to build on top of your own chips. You're also selling your own chips. How do you have so much capacity or how do you think about it,  whereas the other frontier labs can't seem to get enough?

**Speaker 1:**
[(01:29)](https://podwise.ai/dashboard/episodes/7843975?locate=89)
If you think about what percentage of the world are we monetizing,  and in some places we monetize the tokens as the token and the chip. In other places, we monetize the token, somebody else's model, but using a chip underneath it. And part of the reason is we go back many, many years and we do long-term planning. And so when we saw this AI moment coming,  we looked at a number of different factors to ensure we were not physically constrained. We diversified how many energy sources we had. We locked in real estate so we could build datacenters. We changed how we manufacture datacenters. We don't build them in construction.

[(02:13)](https://podwise.ai/dashboard/episodes/7843975?locate=133)
We shifted a lot more to manufacturing because manufacturing can always do faster than you can do with construction. We reduced cycle time to deploy machines. All of that was stuff we've done and that helps us capacity-wise. Then on the silicon side, we've always We've worked with NVIDIA as a partner,  but we've also wanted to build our own silicon and we've done it for I think it's like 11th year now or 12th year. 8th generation TPU will be announced at our event.

**Matthew Berman:**
[(02:42)](https://podwise.ai/dashboard/episodes/7843975?locate=162)
Yeah, we're going to talk about that.

**Speaker 1:**
[(02:43)](https://podwise.ai/dashboard/episodes/7843975?locate=163)
And so that's something we've got real art of doing over and over and over and delivering that advantage over and over and it's something we've delivered. And the interesting thing is we see demand now from not just from the AI labs,  But from other segments, you'll see Citadel, for example,  in capital markets talking about how they're using our TPUs. You'll see Department of Energy and high-performance computing customers talk about it. So we're also seeing TPUs becoming more general-purpose infrastructure, not just for AI algorithms.

**Matthew Berman:**
[(03:17)](https://podwise.ai/dashboard/episodes/7843975?locate=197)
So when you're looking at monetizing TPUs across all of the different avenues that you have to allocate your compute,  how does it compare? Maybe if you want to share specific numbers, great,  but if you're looking at just comparing and contrasting selling a TPU versus allowing Anthropic or OpenAI to serve their inference through your infrastructure versus your own Gemini models. How do those different avenues compare?

**Speaker 1:**
[(03:43)](https://podwise.ai/dashboard/episodes/7843975?locate=223)
We balance investments across all these and we make great margins no matter which way we're selling it because we own our own IP. We're not just a distributor for other people's IP. I think that's helped us and you've seen us improve both top line and operating margin. We've also moved TPUs now as, for example, when you look at capital markets,  One of the things we find that's very interesting is that algorithmic trading was done using numerical computation,  which was largely done on traditional compute. That's been constrained by the Moore's law. The incremental improvement you see generation to generation is getting slower,

[(04:21)](https://podwise.ai/dashboard/episodes/7843975?locate=261)
 and so many of the top firms have seen the huge improvements they can get by shifting to inference. Instead of doing computation using numerical techniques, if you shift to inference,  you can write the improvements you're seeing in inference time. And as they've come in, they want our machines in their venues where it's closer to where the exchanges are,  for example. So we've started taking TPUs and making it available in other people's data center for some of our key customers. And that's a slightly different Business model and we have, you know, in in macro,  I would say diversification improves product because you see requirements from many places.

[(05:05)](https://podwise.ai/dashboard/episodes/7843975?locate=305)
Diversification and monetization also helps us grow. I mean, when we deal with supply chain vendors, for example, because we are using these chips,  not just for our own needs, but also offering them a market, they say,  well, Google's demand is a sum total of a much larger pool. And as a result, we get favorable terms.

**Matthew Berman:**
[(05:24)](https://podwise.ai/dashboard/episodes/7843975?locate=324)
I want to stick on this point for a moment longer. Compute demand is infinite. I mean, even just for the R&D side, why not just hoard the compute? Why not just keep it? And to put a finer point on it,  if AGI is really the goal that all of the AI labs are heading towards and whoever hits it first and is able to scale it out wins,  it seems like keeping the capacity For yourself,  keeping it for your own models is actually quite beneficial. What am I missing?

**Speaker 1:**
[(05:55)](https://podwise.ai/dashboard/episodes/7843975?locate=355)
You have to make money to fund all of this.

**Matthew Berman:**
[(05:57)](https://podwise.ai/dashboard/episodes/7843975?locate=357)
Google makes a ton of money.

**Speaker 1:**
[(05:59)](https://podwise.ai/dashboard/episodes/7843975?locate=359)
But you have to keep generating cash flow to do it. And this is one more lever for us to generate sufficient cash flow. And the amount we allocate to other people is balanced always against our own needs and our own capital requirements. And you know, no matter which lab you're in, Venture capital cannot fund you indefinitely. And as compute costs grow,  if you're running a loss leader business where you're losing money and you're not making enough money from inference and other techniques to cover the cost of training,  as that gap widens, the number of sources you can go to gets smaller.

**Matthew Berman:**
[(06:35)](https://podwise.ai/dashboard/episodes/7843975?locate=395)
I've been talking about how Google is in such a unique position. They have the cash cows. They have the chips, they have the models. Does your Gemini team ever come to you and say like, we don't have enough? I know I'm really sticking on this point,  it's just so wild for me to hear where these other companies are just not able to keep up.

**Speaker 1:**
[(06:54)](https://podwise.ai/dashboard/episodes/7843975?locate=414)
There's always demand for these things, and I think for the next 10 years,  there will always be more demand than supply. And that's a good place to be in if you have your own chip. If you don't, you're reselling other people's stuff. And in a capacity-constrained environment, your unit economics get more expensive. And in our case, because we control the chip, The unit economics remain attractive. So that is going to be an advantage for us because we own the silicon.

**Matthew Berman:**
[(07:25)](https://podwise.ai/dashboard/episodes/7843975?locate=445)
So if you look at the whole pie of your TPUs, of your compute infrastructure,  can you talk a little bit about what the split is between training inference,  selling TPUs, serving inference for other labs?

**Speaker 1:**
[(07:37)](https://podwise.ai/dashboard/episodes/7843975?locate=457)
Broad brush, I think we don't talk about the details, so I'm not going to go through every element. But broad brush, if you look in macro, cloud is about half of Alphabet's capital,  and it's growing because it's growing much faster, as you know. So that's like a split. And then on our side, a significant part of our growth is coming from Gemini and our models. And so you can use that as a rough approximation.

**Matthew Berman:**
[(08:02)](https://podwise.ai/dashboard/episodes/7843975?locate=482)
Okay. You mentioned data centers and building out data centers. Can you explain what the difference is between construction and manufacturing when you're talking about data centers?

**Speaker 1:**
[(08:12)](https://podwise.ai/dashboard/episodes/7843975?locate=492)
Yeah, it's just what is the unit at which you're deploying capacity? You could take, for example, a rack of machines, assemble it in a datacenter. You could take an entire row of machines and deploy it in a datacenter. The higher the grain at which you can deploy, the more you can pre-construct it,  pre-test it in a central location, which means you're much faster in deployment.

**Matthew Berman:**
[(08:38)](https://podwise.ai/dashboard/episodes/7843975?locate=518)
When you're planning deployment of a new datacenter, You're probably more aware than anybody,  there's a pretty negative sentiment about data centers in the U.S. specifically. I think it's 20% favorability. How do you think about that? How do you think the broader AI industry can start to change the opinion,  change the sentiment around artificial intelligence and specifically deploying data centers, which gives the US a strategic advantage? I tend to be very optimistic about AI in general. How do you think about that?

**Speaker 1:**
[(09:12)](https://podwise.ai/dashboard/episodes/7843975?locate=552)
What people are really concerned about on data centers is a couple of things. Number one, will energy costs in my state or my county go up? Second, will there be sufficient employment in the local community in which the data center operates? There's a couple of things that we're doing. First one is we're investing in behind-the-meter technology where we're not taking energy off the grid and we cross-connect to the grid if the state wants it so that in case there's short supply on the grid,  our energy can fuel the grid.

[(09:48)](https://podwise.ai/dashboard/episodes/7843975?locate=588)
We're investing in alternate forms of energy because we think that the traditional mode of generate and distribute is not necessarily the only way that energy supply will come into the market. And so one of the things we're looking at is,  can you reduce the unit cost of energy with new forms of energy delivery created by the demand for AI,  but then can serve the broader market? Third, we take a lot, we pay a lot of attention to making sure the unit of energy we're consuming,  what's called PUE, that we have the best in the industry, meaning If you need 100 megawatts of compute,  how little incremental megawatts do you need from the energy source so you're not wasting energy?

[(10:34)](https://podwise.ai/dashboard/episodes/7843975?locate=634)
And we're by far the most efficient at that in the world. And there's a thousand things that go into that on thermodynamic exchange, how we do heating, all of that. Lastly, we're investing in the communities in which we're in. And to avoid the communities feeling like Google's deploying in one giant location,  we distribute it in many places so that no individual state feels like we're becoming a big burden on their resources. And we've had a great track record. I travel to many, many of our data centers. And when you go to the local economy and see the kids in the school systems and you see The employees who operate our data centers who are super important to us,

[(11:18)](https://podwise.ai/dashboard/episodes/7843975?locate=678)
 how much economic development we bring to those rural communities where we think that's part of our responsibility.

**Matthew Berman:**
[(11:25)](https://podwise.ai/dashboard/episodes/7843975?locate=685)
That's fantastic. What about the broader sentiment and not the local community? Because when you go in, you create jobs, you're investing,  you're not using the electricity and driving up the prices directly. That's all wonderful,  but how do you actually change the hearts and the minds of the broader US demographic with regards to artificial intelligence?

**Speaker 1:**
[(11:50)](https://podwise.ai/dashboard/episodes/7843975?locate=710)
That's going to be a process, you know,  and I think it's finding places Where you can apply the technology in a way that's good for society rather than just,  you know, causing issues where people are worried about job displacement. I'll give you just a few examples of things.

**Matthew Berman:**
[(12:08)](https://podwise.ai/dashboard/episodes/7843975?locate=728)
Please.

**Speaker 1:**
[(12:09)](https://podwise.ai/dashboard/episodes/7843975?locate=729)
You'll see in our, you know, keynote a company called Signal. We do not talk about it. They're a health insurer based in Germany. They're the largest health insurer in Germany. They today deploy A lot of agents built on Gemini Enterprise to help their teams do work. The really interesting thing was there was a lot of anxiety when we started the work with them that it would mean job displacement. They have not let go anybody. And in fact,  what they found is the accuracy with which and the speed with which they can answer questions from people about Am I eligible for this treatment or not? It's cut down from, in some cases, 23 minutes to research and answer, now to less than a few seconds.

[(13:00)](https://podwise.ai/dashboard/episodes/7843975?locate=780)
And so that's improved efficiency, it's improved quality of the customer care, and they've not let go a single job. We work, for example, with the American Society for Clinical Oncology. They're the largest, 51,000 members, every oncologist in the United States. They wanted an application where AI was helping a doctor sitting down to deal with a patient to understand standard of care guidelines,  which is this person's come in, they have breast cancer, what's the guideline? It turns out they're also diabetic. I can't prescribe chemo if they're diabetic of this kind. There's a lot. These rules are incredibly complicated. In many cases, they overlap. And they wanted some help on providing answers.

[(13:48)](https://podwise.ai/dashboard/episodes/7843975?locate=828)
The answers have to be 100% correct. You can have a hallucination. And we've helped them. And it helps doctors take care of patients. And the feedback from their membership has been incredibly rewarding to see. So there are lots of examples. And we always say the most important thing, Citigroup, for example, is building a wealth advisor. So today, if you think of the average citizen, If you're a high net worth person,  you can go to a private bank and your wealth management professional advise you. If you're an average person who doesn't have those financial resources, you may not get high quality advice. Citigroup is building a wealth advisor. They're going to be showing it at the event,

[(14:30)](https://podwise.ai/dashboard/episodes/7843975?locate=870)
 which allows you to use our reasoning and task management capabilities in Gemini to advise people and also to help them take investment actions if they want. So these are examples of Things that society is going to find beneficial. It takes time to get the balance between the AI is going to cause massive job displacement to also hear from this side of things. And that's part of the journey we're on as a society.

**Matthew Berman:**
[(15:01)](https://podwise.ai/dashboard/episodes/7843975?locate=901)
I do agree. I think job displacement in particular is something the general population in the US is extremely worried about. Let me ask you directly for your organization, Google Cloud,  Now that you're seeing your engineers and other parts of your organization be more productive because of artificial intelligence,  more automation, are you hiring? Are you letting go folks? Are you stable? Where are you on that front?

**Speaker 1:**
[(15:27)](https://podwise.ai/dashboard/episodes/7843975?locate=927)
We're adding people for products and sales. We're hiring a lot of people in a go-to-market organization. We're hiring a lot of forward-deployed engineers. And in places where we're building new product, we're adding capability. Like an example, I will tell you, Here's an example of what people don't see. A long time ago, we said as models became more sophisticated in understanding code,  Second, as models learn how to use computers to do tasks,  there are lots of things they can do amazingly well. But one of the issues with understanding code is they can also find vulnerabilities in code. So enormous anxiety about cybersecurity vulnerabilities from some of the new models.

**Matthew Berman:**
[(16:12)](https://podwise.ai/dashboard/episodes/7843975?locate=972)
We're going to talk about that.

**Speaker 1:**
[(16:13)](https://podwise.ai/dashboard/episodes/7843975?locate=973)
Made a decision a long time ago to do three things. Number one, Helping improve Gemini as a way to detect issues in code,  and we have a lot of customers using it. Second, helping build a model that can repair code. Because if you're finding vulnerabilities very quickly, people may not be able to keep up. So can a model assist you in fixing it? We have new capability coming for that. When we acquired this company WIS, you'll see us showing new capability with WIS. It's really about continuous detection. People call it continuous red teaming. We're going to show three different types of agents.

[(16:54)](https://podwise.ai/dashboard/episodes/7843975?locate=1014)
An agent that continually attacks you to make sure your vulnerabilities are being fixed and you don't get caught off guard,  which you couldn't do before. An agent that prioritizes the issues that have been discovered so that you can get,  okay, these are the ones I really need to fix. And then a third one that helps you fix them.

**Matthew Berman:**
[(17:12)](https://podwise.ai/dashboard/episodes/7843975?locate=1032)
I'm glad to hear you're still hiring. You're more productive and hiring. There are companies out there, I think Block is the big one. Jack Dorsey put out this blog post, Block laid off half of their organization,  blamed AI or pointed at AI as the reason. What do you think the difference is between how Google sees this productivity increase and is still increasing employment versus Block who said,  no, we're actually gonna transform the company, we need half as many people and we're gonna do things better. Where's the discrepancy there?

**Speaker 1:**
[(17:46)](https://podwise.ai/dashboard/episodes/7843975?locate=1066)
Every company has demand for its products and services and each CEO makes their own decisions. We're seeing plenty of demand and so we're investing.

**Matthew Berman:**
[(17:55)](https://podwise.ai/dashboard/episodes/7843975?locate=1075)
Let's talk about NVIDIA for a moment. Jensen just did a podcast with Tarkesh and he talked about how NVIDIA and their architecture is the cheapest on a per token basis overall total cost of ownership. That's because of CUDA and NVLink networking tooling, delivering better tokenomics. Do you agree with that assessment? Do you think Google is the best overall total cost of ownership? And if not, how does Google catch up?

**Speaker 1:**
[(18:25)](https://podwise.ai/dashboard/episodes/7843975?locate=1105)
We have a lot of customers who say we are the best total cost of ownership.

**Matthew Berman:**
[(18:29)](https://podwise.ai/dashboard/episodes/7843975?locate=1109)
I guess that was the answer, right?

**Speaker 1:**
[(18:30)](https://podwise.ai/dashboard/episodes/7843975?locate=1110)
I mean, the reality is, if you're an AI lab, you choose the best platform. It's not just our own teams that use it. We have more demand than we can possibly meet from all the other AI labs. And so I would just tell you that they would not be asking for TPU if you were much more expensive.

**Matthew Berman:**
[(18:51)](https://podwise.ai/dashboard/episodes/7843975?locate=1131)
Is a big factor of what makes TPU special the speed? I've noticed the Gemini family of models is very fast. And as a speed maxi myself, I very much appreciate the speed. And typically when you're looking at ASICs, they're specialized, they tend to be a lot faster than the generalized GPU. Is that a selling point for a lot of AI labs or for your own customers? Or are they still saying quality all day, quality, quality?

**Speaker 1:**
[(19:19)](https://podwise.ai/dashboard/episodes/7843975?locate=1159)
It's a combination, I would say, three core elements, because I think it's not the chip, it's the system. TPU system, for example, AT has 9600 chips. 8i is, I think, 1152, all on a single optical torus network. So there's incredibly high bandwidth, super predictable latency across all the chips in a pod. And that gives you, for example,  when you look at the speed with which we're able to take stuff out of the memory for processing and to put stuff back in memory,  it's extraordinarily efficient. Just to give you an example, 8T, the training chip, can fit two petabytes of memory in a single system. Two petabytes is like a hundred times the size of all the Library of Congress digitized.

[(20:12)](https://podwise.ai/dashboard/episodes/7843975?locate=1212)
Because it's the super low latency network, your throughput from memory into the chips themselves are extremely fast. Third, if you look above that layer, from a programming stack point of view,  you have a lot of tools that Google has built and given to the industry that's used for compiler optimization. For example, JAX, we've done great work with PyTorch, XLA, Pathways. These are all technology that Google's built, and so you put all of that together. Even if you look at inference, VLLM, there's a number of technologies that we super optimize. It's that whole stack that makes that TPU system so efficient and so powerful. You see that measure through what we call good put.

[(21:04)](https://podwise.ai/dashboard/episodes/7843975?locate=1264)
Good put is how much effective throughput are you seeing. We also made some decisions a long time ago, like three, four years ago,  for instance, We saw that energy, to your point earlier,  on energy was going to be short supply. So we focused on optimizing the dollars per watt or tokens per watt. And I think that's another element that you see a lot of people wanting.

**Matthew Berman:**
[(21:29)](https://podwise.ai/dashboard/episodes/7843975?locate=1289)
So you've talked a little bit about planning and the TPU, remind me, you said 11 years?

**Speaker 1:**
[(21:34)](https://podwise.ai/dashboard/episodes/7843975?locate=1294)
Yes.

**Matthew Berman:**
[(21:35)](https://podwise.ai/dashboard/episodes/7843975?locate=1295)
11 years ago. It's kind of wild to see that a decision made so long ago, long in the tech world,  has bared so much fruit in the last few years. Change, how much variance in your planning happens based on what you're seeing in the market today? Do the decisions that you made years and years ago apply and they're just steadfast or are you having to change things constantly?

**Speaker 1:**
[(22:03)](https://podwise.ai/dashboard/episodes/7843975?locate=1323)
I would say the history we have across the different layers of the stack Has compounded over time. When we did TensorFlow, we realized you needed a large scale distributed programming model for training and we built JAX,  for example. That was something that was compounded on our history of learning from what people were trying with TensorFlow and needing a new distributed training model. Some of these accumulate over time because we learn from what we're doing from prior and we're making new improvements. We're also incredibly attuned to the market, listening to customers, making decisions like people asked us,  why did you build 8i, the inference chip?

[(22:50)](https://podwise.ai/dashboard/episodes/7843975?locate=1370)
It's because we've seen that as you eventually, no matter how rich you are,  you cannot fund training without making money on inference. And so you have to at least cover the cost of your training from a breakeven point of view over time. You can't just always depend on venture capitalists to fund you. And so we said there's going to be a big demand for inference. We knew what the factors we needed to optimize for inference. And, you know, frankly, the demand for the inference, the 8i has been way, way more than we expected.

**Matthew Berman:**
[(23:25)](https://podwise.ai/dashboard/episodes/7843975?locate=1405)
Let's talk about the 8th Gen chip. So this is the first time where you have split out two different chips,  family, but two different chips, one for inference, one for pre-training. First, just confirm Ironwood was more built for inference?

**Speaker 1:**
[(23:44)](https://podwise.ai/dashboard/episodes/7843975?locate=1424)
Ironwood was a mixture. It was used for training and inference. Yeah, I think there was people, people run, for example, inference, there's a lot of diurnality to it. During the daytime, people wake up and they ask a bunch of questions at night. Even some people still sleep. At that time, a lot of people were using a spot for inference. Like post-training, a lot of people were doing on-spot instances at night. It's a general-purpose chip. With eight, T is mostly for training. Some people are considering using it for inference, and I is primarily for inference,  although people with smaller models also use it for training.

**Matthew Berman:**
[(24:31)](https://podwise.ai/dashboard/episodes/7843975?locate=1471)
Based on the fact that you decided to split the chips,  what does that say about where the workloads are heading? What do you see today and then what do you think we're going to see over the next,  let's say, five years? Where are the major workloads going to be?

**Speaker 1:**
[(24:45)](https://podwise.ai/dashboard/episodes/7843975?locate=1485)
So you see that in the work we're doing with Gemini as much as in the silicon. So if you look at Gemini, we've seen sort of three phases, if you will, with the models. The first phase was where people were asking the model a set of questions. And it was answering, and you may iterate on it in a multi-turn,  but it was primarily kind of a search chatbot-like experience. So our Gemini Enterprise product does provide the ability to do search and answer questions. It also added deep research to do deep analysis. Then the second phase came along where People used to use diffusion models primarily to create content,  like images, audio, video.

[(25:38)](https://podwise.ai/dashboard/episodes/7843975?locate=1538)
And then with 2.5 Nano Banana, we added media in was always true,  but media out became part of the main model. And so we saw people from creative, for example, WPP,  a variety of CPG firms using Gemini Enterprise,  our Enterprise AI platform to create content. And there's all kinds of content creation now going on with it. Then the models became really good at dealing with the abstractions of the world. When I say abstraction of the world, if you go to a company,  the model has to be hooked into a variety of different systems. That is to talk to your CRM system, to ask and answer questions about customers. It may have to look at your supply chain and planning systems.

[(26:29)](https://podwise.ai/dashboard/episodes/7843975?locate=1589)
As the models became really good at dealing with those,  and the ultimate abstraction is abstracting the rest of the world as a computer. Because if you can talk to a computer, the computer can talk to everything. Because all these forms of software are just abstractions for how a computer can talk to it.

**Matthew Berman:**
[(26:47)](https://podwise.ai/dashboard/episodes/7843975?locate=1607)
Do you think that is the ultimate abstraction? A model being able to control computers, computer use, browser use?

**Speaker 1:**
[(26:53)](https://podwise.ai/dashboard/episodes/7843975?locate=1613)
But understanding the information that comes from those systems as well. It's not just I can talk to a computer,  but I need to be able to respond to the information that computer gives me. Do you see what I mean? And so that's then led to this notion of agent. An agent is a module, let's call it that, that you can delegate tasks to. The agent describes itself as a set of skills and it knows how to operate a set of tools,  and then it can operate those, including a computer and do tasks on your behalf. Now for us, that allows people Whether it's Xfinity using us to schedule and manage all their customer care,

[(27:35)](https://podwise.ai/dashboard/episodes/7843975?locate=1655)
 Walmart using us for a variety of things in their organization from planning to scheduling,  Bosch in manufacturing using us. Merck has talked about how they're using us for research and patient from the drug discovery out to delivering to patients the whole cycle being automated. And that's the next phase of evolution. And so part of it is we're sort of co-designing as the skills of the model advance,  we're able to broaden the set of things that can be done.

**Matthew Berman:**
[(28:08)](https://podwise.ai/dashboard/episodes/7843975?locate=1688)
Tie it back to how that informs the decision to split up the two chips between inferencing and training.

**Speaker 1:**
[(28:14)](https://podwise.ai/dashboard/episodes/7843975?locate=1694)
So if you look back when you asked search a question, the first phase,  there were a lot more input tokens than output tokens when you asked the model a set of questions. Because you would ask it a very complicated, long, described question and it would say this is the answer. Then when you came to content generation, you would give it a simple prompt,  create a video that shows my dog wearing a Superman cape and driving a car. And then it would take a while to generate the output tokens. So that generated a very different mix of tokens, of the type of tokens. Multimodality was one big thing, and then the volume of output tokens grew. Then you come along to agents.

[(29:01)](https://podwise.ai/dashboard/episodes/7843975?locate=1741)
It informed chip design in three or four different ways. It informed us on how long you need to maintain stuff in memory. So for example, what kind of KV cache would you want? Because now you're delegating something that could run for 6, 7, 12 hours. You don't want to be shuffling things in and out as tokens because they get expensive. So that's one example of something. Second example, You want this system to operate a computer. By the way, that computer is a traditional classical compute machine. So when people asked us, how did that inform your chip effort? We not only work with Intel, we all have our own ARM chips.

[(29:44)](https://podwise.ai/dashboard/episodes/7843975?locate=1784)
We built that because we saw general purpose compute usage coming from these tools. When you run for inference an agent that does many different steps,  there are things about how you want to hold and pin objects in memory in the model so that the model runs things super efficiently because that can really optimize the cost of inference. There are many things we've done internally on how the chip can hold things in memory,  And then because people wanted even a practical example,  people want inference in many locations because they want to manage latency,  unlike training where you can put it in a few big locations. So a practical example is 8i can be run in non-water-cooled mode.

[(30:32)](https://podwise.ai/dashboard/episodes/7843975?locate=1832)
So that you can put it in many more locations because air cooling is still the primary thing in most data centers. So there's a lot of thought that goes into these decisions. I'm just giving you three simple examples to illustrate.

**Matthew Berman:**
[(30:44)](https://podwise.ai/dashboard/episodes/7843975?locate=1844)
Yeah,  I think the agent piece is really interesting because it really changes the way that those tokens are actually used in practice. Obviously NVIDIA talks a lot about extreme co-design. Google seems like they have extreme co-design on every layer. First, talk about with agentic usage, especially if you're doing a lot of read and writes to a hard drive or you know,  there's like a lot of pieces that you need to optimize for. What's the latest thing that you've optimized for in the TPU stack? And then where do you think the next big bottleneck is based on agentic usage growth?

**Speaker 1:**
[(31:20)](https://podwise.ai/dashboard/episodes/7843975?locate=1880)
So we look at the whole system all the time. A couple examples, we're announcing two new storage solutions next week. One is our managed Lustre solution. We've improved it to run 10 terabytes per second throughput. It is really designed for large-scale training. So you can cross-connect it to a giant cluster, and because you have large datasets,  you can read them from the large-scale Lustre cluster now into a large training fleet for super-efficient scale. So that's one. Second thing we introduced is a new ultra low latency inference storage system called Rapid Storage. The idea is you can centrally keep the information you want to inference on in Cloud storage,  but you can mount it close to where,

[(32:23)](https://podwise.ai/dashboard/episodes/7843975?locate=1943)
 think of it as a forward proxy like thing,  wherever your inference chips are running. From your inference processor down to the storage system, rapid storage to fetch for inference, It's incredibly fast. It's 15 terabits per second. So you get ultra low latency. You want to optimize all this stuff on a common network backbone. So we're introducing a new form of networking called Virgo,  which gives you ultra low connectivity speed across a giant cluster. So there are many, many other parts to the stack we're also co-designing because of agents coming in. And the idea is to give people the most efficient cost structure to run agents with the best performance and quality.

**Matthew Berman:**
[(33:11)](https://podwise.ai/dashboard/episodes/7843975?locate=1991)
Where's the next big bottleneck?

**Speaker 1:**
[(33:13)](https://podwise.ai/dashboard/episodes/7843975?locate=1993)
The next big bottleneck will be largely around when consumers use virtual machines. Let's say I'm a consumer at home. I build an agent. The agent is going to schedule travel for me, just hypothetically, if you're going on vacation. You ask it to do a bunch of tasks like go look up eight travel sites which are exposed as tools. This common thing now people call MCPs or APIs. Let's go find all the travel sites. Let's say it's booking a trip to Europe or to Southeast Asia, run that,  calculate for me the total cost and tell me my budget. Consumers cannot afford to have VMs running forever. It's extremely expensive, as you know. So people want to activate, deactivate VMs whenever a task gets done.

[(34:07)](https://podwise.ai/dashboard/episodes/7843975?locate=2047)
Because these tools need local storage, these virtual machines can be oversubscribed,  but you can also have local disk from which you read and write super efficiently. That's going to be a bottleneck because it's going to directly affect how widespread you can make this technology available. Because companies can pay for stuff. Obviously, the cheaper and more efficient, they can use more stuff. But if you want to bring this to consumers, you know, for them, it gets expensive very quickly. And if you want to reach everybody, you're going to have to engineer the cost structure of these things. And having, again, that ability to go across the layers from the agent down to Gemini,

[(34:54)](https://podwise.ai/dashboard/episodes/7843975?locate=2094)
 down to the storage system and the compute systems, that allows us to co-design.

**Matthew Berman:**
[(34:59)](https://podwise.ai/dashboard/episodes/7843975?locate=2099)
Thank you for sharing that. I want to talk about Anthropic a little bit. Anthropic is one of Google's customers. They are a unique company in a lot of ways. Claude is one of Google's biggest rivals at the same time,  yet you are essentially their backbone for a lot of the training,  a lot of the inference. How do you think about that decision? And I know we touched on it earlier, but I want to go into more detail. How do you think about powering Anthropics models and then they are also competing with Google? Is that the AWS playbook where it's power everybody and We're just not going to play favorites or is it something different?

**Speaker 1:**
[(35:39)](https://podwise.ai/dashboard/episodes/7843975?locate=2139)
Google is a platform company. So when you're a platform company, different parts of the business compete with different players in the market. Some parts of your business may supply them and some part of the business may compete with them. We're determined to be best in class in the models. We're very proud of what we've done, not just with Gemini, the model,  but also the whole tool chain that we're bringing around Gemini with our enterprise portfolio of tools. At the same time, there are customers who want, for example, our TPUs,  and so Anthropic is an example of them. And it's just part of being a platform company.

[(36:18)](https://podwise.ai/dashboard/episodes/7843975?locate=2178)
It's the same way that people ask us, how well do you optimize your model with Apple? Apple, for example, has signed a contract with us for the model, as you know. And so people go, isn't that competing with your Android platform and ecosystem? Yes, but that's part of being a platform company.

**Matthew Berman:**
[(36:37)](https://podwise.ai/dashboard/episodes/7843975?locate=2197)
I think I'm kind of stuck on the Anthropic piece because they are competing on the enterprise level where Apple is not. I'm just thinking you're powering them and then at a certain point we may get,  and although there's plenty of TPU capacity to go around right now, as you said,  but at a certain point there might have to be a difficult decision. How do you make that decision of Well,  can we give the capacity to an Anthropic or do we keep it for Gemini? Do we keep it for our own research? How do you make that decision?

**Speaker 1:**
[(37:08)](https://podwise.ai/dashboard/episodes/7843975?locate=2228)
We have an executive team with Sundar and we discuss these and as any mature company, we make those decisions. There's difficult calls every day. For instance, we have demand not just from Anthropic. So what percentage for, even if you said there's X amount for Gemini and there's Y amount for the rest of the world,  what amount do you give Anthropic versus the hundreds of other labs and other customers ask us for it? That's all complicated decisions that anybody has to make. What I'll tell you is this, it's better to have your own chips and demand than not having your own chips.

**Matthew Berman:**
[(37:44)](https://podwise.ai/dashboard/episodes/7843975?locate=2264)
Yeah, well said. Mythos, you kind of hinted at it a little bit. I think it's rumored to be the first 10 trillion parameter model. Is Google playing in the 10 trillion parameter model space yet? Are you close to it? Where are you in that life cycle?

**Speaker 1:**
[(38:01)](https://podwise.ai/dashboard/episodes/7843975?locate=2281)
You'll see new stuff from us on Gemini with announcements coming both at Next and soon after. I think on the capability of the model, we're very proud of where Gemini is. I mean, it's been state-of-the-art for a long time. We have a new version of Gemini coming very, very soon. And from all the benchmarks we've seen, we've been very confident on that as well.

**Matthew Berman:**
[(38:24)](https://podwise.ai/dashboard/episodes/7843975?locate=2304)
So, hypothetically, if you think about a 10 trillion parameter model,  based on what you oversee on the TPU side,  is that even a feasible size to serve in the current state of the world?

**Speaker 1:**
[(38:37)](https://podwise.ai/dashboard/episodes/7843975?locate=2317)
We've had a capability to do disaggregated serving,  which allows us to scale very large dense models super well,  and that's been in place for a long time. And so we're able, we would not design a model that we couldn't serve. And so we're very confident of TPUs can serve the largest models in the world. And most importantly,  our serving stack We use for disaggregated serving by definition is the most efficient on TPU of all the model providers in the industry. So we're very confident we can serve the largest models, particularly the largest Gemini models.

**Matthew Berman:**
[(39:14)](https://podwise.ai/dashboard/episodes/7843975?locate=2354)
Does this mean that we're not seeing any slowdown on the scaling pre-training side? You're not feeling it at all because there was for a while in the industry,  people talking about pre-training is slowing down. Now let's focus on RL. Let's focus on the thinking time. You're not seeing that at all.

**Speaker 1:**
[(39:30)](https://podwise.ai/dashboard/episodes/7843975?locate=2370)
We're not seeing that from the point of view of chip design or system design or lack of capacity or any of that.

**Matthew Berman:**
[(39:38)](https://podwise.ai/dashboard/episodes/7843975?locate=2378)
And then what about the underlying data? Are you seeing more effective use of synthetic data?

**Speaker 1:**
[(39:45)](https://podwise.ai/dashboard/episodes/7843975?locate=2385)
We are seeing, I mean, I'll give you two or three examples of things we are seeing. Historically, a lot of the data that was fed into models Was unstructured data like text, audio, video, files, etc. Those continue to grow,  but the reality of those is like there are many elements in an enterprise context which make them actually really simple to deal with. When you ask a question to an agent and you have the agent respond and tell you,  tell me the citation or where did you derive this answer from? It's easy if it's in a document because you can just show a link to that document. Now, just imagine you ask the model a question,  tell me how much inventory we'll need to meet demand for this product.

[(40:32)](https://podwise.ai/dashboard/episodes/7843975?locate=2432)
That is going to translate to a query on a system like an SAP system or some kind of supply chain system. That's dynamically going against a set of tables. So first being accurate on decomposing that query into which table is it getting it from and showing the response like where is the citation,  like how do I know the answer that you gave me is correct is a much more complicated problem. And so because of the work we do in enterprise,  we're able to feed Gemini a lot more cycles into our trajectory optimization harness with structured data,  complex things like complex fields. Have you ever seen a, when you talk about computer use in a browser use,

[(41:22)](https://podwise.ai/dashboard/episodes/7843975?locate=2482)
 if you ever see an enterprise application with a thousand fields, dropdown lists, et cetera,  There's no consumer app that would ever have that complexity. So being in this space also allows us to teach. Our Gemini system some of those things and put it into the harness.

**Matthew Berman:**
[(41:41)](https://podwise.ai/dashboard/episodes/7843975?locate=2501)
Let's continue on harnesses and agentic coding in general. I've been doing a lot of coding myself. There was kind of a viral tweet that went around about somebody who had a friend at Google who basically said Google isn't on the frontier of agentic coding internally. What's your take on that? How has Google adopted agentic coding? And especially, again, I have to bring up Anthropic, the rate at which they're shipping is incredible. How is Google adopting the frontier of agentic coding today?

**Speaker 1:**
[(42:14)](https://podwise.ai/dashboard/episodes/7843975?locate=2534)
We have a lot of engineers using Jetski, which is our internal coding harness. And that feedback has been going directly to DeepMind in that reinforcement loop. And it's improving quality of Gemini for coding every day. And we have a lot of people in my organization using it.

**Matthew Berman:**
[(42:32)](https://podwise.ai/dashboard/episodes/7843975?locate=2552)
One thing I've noticed, I'm more productive than ever. I'm shipping so fast. I'm having so much fun doing it. I'm not reviewing every line of code. Actually, I'm reviewing very few lines of code. But Google can't do that. I have little toy projects. Google, you have high stakes projects and services and products that you're serving. How can you both Be on the frontier of agentic coding and be producing so many lines of code,  but also making sure that you're maintaining that quality. Also make sure that you are actually reviewing every single line of code that gets deployed.

**Speaker 1:**
[(43:10)](https://podwise.ai/dashboard/episodes/7843975?locate=2590)
So when we talk about soft engineering productivity, we look at it slightly differently than is reported externally. So if you work in a company that builds products like Google does,  the reality is that there are two or three examples of things that you find that are really important. Like a senior engineer writes much more compact code than a junior engineer. So we don't count how many lines of code as a measure because that's generally,  you know, a weaker engineer writes a lot more code to do the same tasks that a senior engineer does.

**Matthew Berman:**
[(43:46)](https://podwise.ai/dashboard/episodes/7843975?locate=2626)
It's kind of a cliche, right? Over the years, don't count lines of code. But I think now more than ever, it's just the shipping speed overall.

**Speaker 1:**
[(43:54)](https://podwise.ai/dashboard/episodes/7843975?locate=2634)
So it's how much functions do we add that's important. The second thing, we've always had a tradition at Google that When you go to check in code,  you need peer review. Typically, the peer review is done by senior managers, right? And they become the bottleneck. So we've introduced and people are using Gemini. And we, for example, recently in cloud introduced it to scan for security vulnerabilities in code. So it's not just that the tool is being used to generate code, we're also using it to inspect code. And that helps us get when the senior engineers come in for the review,  a bunch of free work has been done. The third one is for the long term, in any real software company,

[(44:38)](https://podwise.ai/dashboard/episodes/7843975?locate=2678)
 the bulk of the time of the engineers where they find doing less productive work is debugging issues. So we built a version of Gemini. And one of the things we're going to show next week is, you know,  what's the most complex computer in the world? The most complex computer in the world is a cloud. It makes a PC look like a toy. We've taken all of our Cloud and exposes as tools to the model. Now we're using Gemini to troubleshoot incidents happening. And so that's also helped us improve the speed with which people can function and in turn improve the quality of the model itself. So there's a number of dimensions through which we look at the issue.

**Matthew Berman:**
[(45:23)](https://podwise.ai/dashboard/episodes/7843975?locate=2723)
But as productivity increases and you're shipping more features more quickly,  I know lines of code is not the measurement,  but it's certainly an output of this increased velocity. There comes a point where you just cannot review every single line of code. And then I think kind of if you think about abstracting and going beyond that,  there's a point at which humans are understanding the actual code less and less over time,  especially as you mentioned, if you're using AI to review the code, to debug. So if you're having AI create code, AI review code,  Are we losing the core understanding of code and the functionality being deployed?

**Speaker 1:**
[(46:05)](https://podwise.ai/dashboard/episodes/7843975?locate=2765)
That's a risk that we have to manage as an industry. People talk about, I'm going to give you a prompt and the prompt is going to generate a block code. And you don't need to understand the code because you understand the prompt. In reality, for a complex system, the prompt will not explain all the potential behavior of the system, right?

**Matthew Berman:**
[(46:27)](https://podwise.ai/dashboard/episodes/7843975?locate=2787)
Yeah.

**Speaker 1:**
[(46:27)](https://podwise.ai/dashboard/episodes/7843975?locate=2787)
And so, for example, how do you deal with exceptions? And so that's something that I think every time you find this one area,  like some time ago, people said, you won't need all these soft engineers. And then Along comes the model and finds a lot of security vulnerabilities. Just when we need a ton of software engineers to work with models,  like we're introducing a version of our model that can actually fix bugs,  fix security vulnerabilities specifically. But you still need a human to use the tool and focus on it. Sometimes the industry over-rotates and so you say you don't need anybody just when you need it. We take a much longer-term view of things.

[(47:17)](https://podwise.ai/dashboard/episodes/7843975?locate=2837)
We're constantly looking at, for instance, Do you need a supervisor model? Today, we're going to look at code in a different way to actually review the code. That's why when I said we still do peer review of the code and we're helping our senior engineers use the tool to do the reviews. Then the question comes, will the tool be self-aware enough? If it generated the code, will it find an issue with code that it generated because it's not self-aware of certain patterns? That's something we're looking at approaches to solve. Our goal has always been to make sure we have the best model is to apply it at scale. And in my team alone, we have thousands of people using it every single day.

[(48:01)](https://podwise.ai/dashboard/episodes/7843975?locate=2881)
I mean, if you walk just over there to the campus,  you can see people like six different windows open,  one in which they're coding, one in which they're compiling, one in which they're You know,  deploying and testing and another one where they've got a background job running to run code review. I mean,  there's a lot of people using the JetSki tool harness and it's part of just evolving how work is getting done.

**Matthew Berman:**
[(48:26)](https://podwise.ai/dashboard/episodes/7843975?locate=2906)
You touched on cybersecurity. Let's finish on that. Anthropic decided the Mythos model was too advanced in the cybersecurity capabilities to release publicly, at least not yet. For Google, how do you think about that? What was your reaction? And then also, is there some line in the sand,  some benchmark that you think or you would determine Gemini is no longer safe to release publicly?

**Speaker 1:**
[(48:51)](https://podwise.ai/dashboard/episodes/7843975?locate=2931)
We're working through that and what would that line be. But our issue has been, so if Mythos finds a set of issues,  What percentage of those issues could be found with an open source model? And the reason I mentioned open source model is no matter how much you defend and you can say,  well,  I'll make sure closed source models don't fall in adversaries and open source models for sure are going to be falling into adversaries.

**Matthew Berman:**
[(49:17)](https://podwise.ai/dashboard/episodes/7843975?locate=2957)
And they're just getting better.

**Speaker 1:**
[(49:18)](https://podwise.ai/dashboard/episodes/7843975?locate=2958)
And they're getting better. So sooner or later, some part of this,  it may not be all of the patterns,  but some part of it can be detected. So what should you do in response? And we are unique because we're a hyperscaler, we're a model provider, and we also have a cybersecurity organization,  both our Mandiant team and WIS. So we've done three practical things. If people are going to find issues using a model,  you need to have a model help fix issues because they're going to find them way faster than humans can fix. So you need a model to help fix. And so we're looking at something there. Second, if they're going to find issues with models,

[(50:02)](https://podwise.ai/dashboard/episodes/7843975?locate=3002)
 they're going to use the model and computer use to launch a large-scale attack. And so to defend that, using like, I'll red team my system once a month is not going to be sufficient. So introducing agents that can do continuous red teaming and agents that can actually help fix For example,  it's one thing to fix the code. It's the second thing to find all the places the old code was running and remove it,  and then deploy the new code that's been patched and updated. That's the second piece. The third piece is there's so much code out there. What do I start with? So again, that's another thing where we built tools to help people identify and prioritize what.

**Matthew Berman:**
[(50:51)](https://podwise.ai/dashboard/episodes/7843975?locate=3051)
Is this an argument for or against open source software, not models, but software? If you're open source, all your code is out there. It is ripe for models to go look at it, find vulnerabilities and exploit them. Closed source, you don't have that problem. But on the other hand, open source is going to get hardened much more quickly. What is your take on that? Is that an argument for or against?

**Speaker 1:**
[(51:15)](https://podwise.ai/dashboard/episodes/7843975?locate=3075)
No, we as Google use a ton of open source and we contribute a ton of open source. We're going to help the open source community using our tools to actually go fix these things. I'm just pointing out the reality of where things are is that adversaries are going to use the model and the first place they're going to try and scan is popular open source libraries. Because that gives them the maximum surface area to try and attack. And so those are all elements where we think it's important to go and address and fix and we're in process with the rest of the industry.

**Matthew Berman:**
[(51:49)](https://podwise.ai/dashboard/episodes/7843975?locate=3109)
Thomas, last question for you. What keeps you up at night?

**Speaker 1:**
[(51:52)](https://podwise.ai/dashboard/episodes/7843975?locate=3112)
We, you know, we're balancing so many things, making sure we have to, one part of your discussion,  do we have right on long-term plans for capital infrastructure, for data centers, networks,  enough of those lovely TPUs to go around? Second, are we constantly pushing the domain problems, the important problems? Three years ago when we said, We should solve the problem of as AI gets better,  cyber is going to be definitely an area that's affected. And when we made the offer to buy Wiz, people asked like, why would you guys be doing that? When we look at our Gemini enterprise platform, just to give you an example,  between January and now, our token count has jumped from 10 billion a minute.

**Matthew Berman:**
[(52:42)](https://podwise.ai/dashboard/episodes/7843975?locate=3162)
I'm the CEO of Gemini Enterprise.

**Speaker 1:**
[(52:42)](https://podwise.ai/dashboard/episodes/7843975?locate=3162)
Gemini has jumped from 1 billion to 16 billion a minute. And the number of enterprise users of Gemini Enterprise has jumped by 40% sequentially. So we're always looking at how we're solving the right problems for customers and users. And that's always the focus for us. And as long as we keep pushing aggressively The technology is evolving so quickly that when something happens,  you got to have solutions before that occurs to the most part. And our teams have done an amazing job and we're super proud of what they've done and looking forward to the event.

**Matthew Berman:**
[(53:25)](https://podwise.ai/dashboard/episodes/7843975?locate=3205)
Thomas, thank you so much. I really appreciate it.

