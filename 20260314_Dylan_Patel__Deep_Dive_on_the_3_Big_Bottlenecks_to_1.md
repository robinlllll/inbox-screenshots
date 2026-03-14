---
podcast: "Dwarkesh Podcast"
episode: "Dylan Patel — Deep Dive on the 3 Big Bottlenecks to Scaling AI Compute"
link: https://podwise.ai/dashboard/episodes/7508210
publish-time: "2026-03-13"
save-time: "2026-03-14"
---
# Summary

The conversation centers on the future of AI compute, particularly bottlenecks in scaling AI capabilities. Dylan Patel, CEO of Semianalysis, provides insights into the semiconductor supply chain, power demands, and capital expenditures of major tech companies. He argues that while power and data centers were previous constraints, the focus has shifted to chip manufacturing, especially EUV lithography tools. Patel highlights Nvidia's strategic positioning and potential challenges for competitors like Google and even China. The discussion touches on the trade-offs between model size, compute efficiency, and the economic implications of AI infrastructure investments, suggesting a potential divergence between the US and China based on the speed of AI development.

# Takeaways

* Hyperscalers' massive CapEx spending isn't just for immediate compute needs; it includes long-term investments like turbine deposits and data center construction for future scaling.
* Anthropic's initial conservative approach to compute acquisition led to a situation where they now have to pay a premium for last-minute capacity or revenue-sharing agreements.
* The value of GPUs is increasing over time as models improve, because newer models can generate more valuable tokens from the same hardware.
* The biggest bottleneck preventing the scaling of AI compute by 2030 will be the semiconductor supply chain, particularly the availability of EUV tools.
* Nvidia gained a dominant position in 3nm chip allocation by signaling demand and securing capacity commitments earlier than competitors like Google and Amazon.
* Google sold TPUs to Anthropic because Anthropic recognized the value of that compute before Google's own leadership did.
* TSMC favors allocating capacity to CPU production over GPUs due to the perception of CPUs having more stable, long-term growth potential.
* The increasing cost of memory is leading to decreased consumer demand for smartphones and PCs, as manufacturers are unable to absorb the higher component prices.
* China's potential to dominate the semiconductor industry by 2035 depends on the timeline for achieving AGI; longer timelines favor China's ability to catch up and indigenize its supply chain.
* The most effective way to increase AI compute capacity is to modularize data center construction, shifting more of the work to factories for faster deployment and reduced labor needs.

# Q & A

**Q: Given that EUV lithography is essential for producing advanced chips, what would happen if we just went back to 7nm and used multi-patterning with DUV machines instead?**

A: We potentially do go crazy enough that this happens because we just need incremental compute and the compute is worth the higher cost, power, et cetera, of these chips. But it's also unlikely to some extent, to a large extent, because of, I think, just comparing, you know, some of these are like not fair comparisons, right? For example, you know, from A100, which is 312 teraflops to Blackwell, which is like 1,000-ish of FP16, or maybe it's 2,000 and then Rubin is like 5,000 or so FP16. It's not a fair comparison because these chips have vastly different design targets, right? At A100, that is what Nvidia optimized for was FP16, BF16 numerics. When you look at Hopper, they didn't care as much about that. They cared about FP8. When you look at Rubin, they don't care about FP16 and BF16 as much. They care mostly about FP4 and 6, right? And so numerics are what they've designed their chip for.

---

**Q: If EUV becomes a bottleneck, what if we just went back to 7 nanometer and do what China is doing currently in producing 7 nanometer ships with multi-patterning with DUV machines?**

A: There's a couple like, you know, okay, let's just say, let's redesign, let's make a new chip design on seven nanometers. Sure, we can do that. And then it's optimized for the numerics of the modern day. The performance difference is still going to be much larger than the flops difference you mentioned, right? Often it's easy to boil things down to flops per watt or flops per dollar. But that's actually not a fair comparison. And so this is where you can bring in, hey, let's look at Kimi K1 or DeepSeek. When you look at Kimi K2.5 and DeepSeek, when you look at these two models and you look at their performance on Hopper versus Blackwell on very optimized software, you get vastly different performance. And Most of this is not attributed to flops or numerics, right? Because those models are actually 8-bit. So it's not like Blackwell's and Hopper, they're both optimized for 8-bit and Blackwell's not really taking advantage of its 4-bit there. The performance gulf is actually much larger.

---

**Q: What is preventing us from just doing that with How many dies could you have a single chip and still get these tens of terabytes a second?**

A: Even within Blackwell, there are differences in performance when you're communicating on the chip versus across the chips. Those bounds are obviously much smaller than when you're going out of the entire chip, but each die versus within the package. And so anyways, when you scale the number of chips up, there is some performance loss. It's not just perfect, but it is way better than different entire packages. Now, how large can advanced packaging scale? The way Nvidia is doing it is co-auth the way Google and with Broadcom and MediaTek and Amazon, Tranium, all these chips are doing is called co-auth. But actually you can go and look back at what Tesla did with Dojo. Dojo, which they canceled and restarted. Anyways, Dojo was a chip that was the size of an entire wafer. They had 25 chips on it. And there were some trade-offs, right? They couldn't put HBM on it. But the positive side of it was that they had 25 chips on it. And so to date, it is still probably the best chip for running convolutional neural networks.

---

**Q: If we end up in this world in 2030, where the West has the most advanced process technology, but it has not ramped it up as much, whereas China, I don't know if you think by 2030, they would have EUV and, I don't know, 2 nanometer or whatever, but they are a semiconductor pill, so they're producing in mass quantity, I'm wondering what the year is where there's a crossover, where our advantage in process technology has faded enough and their advantage in scale has increased enough?**

A: By 2030, it's it's possible that they do. But but to date, right. All of China's seven nanometer and 14 nanometer capacity uses ASML DUV tools. And the amount that they can ship and import from ASML is large. But the point being that the vast majority of ASML's revenue, especially on EUV, all of it is outside of China. So the scale advantage is still in the favor of the, let's call it the West plus Taiwan, Japan, et cetera.

---

**Q: By 2030, do they have fully indigenized EUV?**

A: I think for sure, for sure. EUV, yes. And fully indigenized EUV by 2030? I think they'll have working tools. I don't think that they'll be able to manufacture A bunch yet right you know there's there's sort of having it work and then there's production hell right and ultimately like ASML had EUV working. In the early 2010s at some capacity. Right. Now, the tools were not accurate enough. They were not scaled for high production, scaled for high volume manufacturing, reliable enough. And then they had to ramp production. And that all took time. Production hell takes time. Right. Which is why it took another five to seven years to get EUV into mass production at a fab rather than just working in the lab.

---

**Q: If EUV becomes a bottleneck, what if we just went back to 7 nanometer and do what China is doing currently in producing 7 nanometer ships with multi-patterning with DUV machines?**

A: So I think, you know, we potentially do go crazy enough that this happens because we just need incremental compute and the compute is worth the higher cost, power, et cetera, of these chips. But it's also unlikely to some extent, to a large extent, because of, I think, just comparing, you know, some of these are like not fair comparisons, right? For example, you know, from A100, which is 312 teraflops to Blackwell, which is like 1,000-ish of FP16, or maybe it's 2,000 and then Rubin is like 5,000 or so FP16. It's not a fair comparison because these chips have vastly different design targets, right? At A100, that is what Nvidia optimized for was FP16, BF16 numerics. When you look at Hopper, they didn't care as much about that. They cared about FP8. When you look at Rubin, they don't care about FP16 and BF16 as much. They care mostly about FP4 and 6, right? And so numerics are what they've designed their chip for.

---

**Q: If we end up in this world in 2030, where the West has the most advanced process technology, but it has not ramped it up as much, whereas China, I don't know if you think by 2030, they would have EUV and, I don't know, 2 nanometer or whatever, but they are a semiconductor pill, so they're producing in mass quantity, what is the year where there's a crossover, where our advantage in process technology has faded enough and their advantage in scale has increased enough?**

A: To date, China still does not have, you know, entire indigenized semiconductor supply chain. Right. But within 2030. Yeah. By 2030, it's it's possible that they do. But but to date, right. All of China's seven nanometer and 14 nanometer capacity uses ASML DUV tools. Right. And the amount that they can ship and import from ASML is large. But the point being that the vast majority of ASML's revenue, especially on EUV, all of it is outside of China. So the scale advantage is still in the favor of the, let's call it the West plus Taiwan, Japan, et cetera.

---

**Q: Does this also imply, by the way, but there's, at least until recently, people had made this huge point about, oh, what is the depreciation cycle of a GPU?**

A: There's a few strings to pull on there. One is, What happens to depreciation of GPUs, right? And I guess I didn't answer your prior question, which is like anthropic. I think we'll be able to get to like five gigawatts-ish, maybe a little bit more by the end of the year through themselves as well as their product being served through Bedrock or through Vertex or through Foundry. I think they'll be able to get to five or six gigawatts, which is way above their initial plans, right? And anyways, that's sort of like, and OpenAI will be roughly the same, maybe a little higher, actually a little bit higher based on our numbers. Anyways, the depreciation cycle of a GPU, right? Michael Burry was saying it's, you know, three years or less, right? Is like sort of his argument. And there's sort of two ways and lenses to look at this. Like mechanically, in this, you know, there's a TCO model, right?

---

**Q: So if EUV becomes a bottleneck, what if we just went back to 7 nanometer and do what China is doing currently in producing 7 nanometer ships with multi-patterning with DUV machines?**

A: There's a couple like, you know, okay, let's just say, let's redesign, let's make a new chip design on seven nanometers. Sure, we can do that. And then it's optimized for the numerics of the modern day. The performance difference is still going to be much larger than the flops difference you mentioned, right? Often it's easy to boil things down to flops per watt or flops per dollar. But that's actually not a fair comparison. And so this is where you can bring in, hey, let's look at Kimi K1 or DeepSeek. When you look at Kimi K2.5 and DeepSeek, when you look at these two models and you look at their performance on Hopper versus Blackwell on very optimized software, you get vastly different performance. And Most of this is not attributed to flops or numerics, right? Because those models are actually 8-bit. So it's not like Blackwell's and Hopper, they're both optimized for 8-bit and Blackwell's not really taking advantage of its 4-bit there. The performance gulf is actually much larger.

---

**Q: In fact, it goes, even the intermediate layers, We are sort of shocking here. So, Carl Zeiss, which is like the optics supplier that is bottlenecking ASML itself, I checked its market cap this morning. You know what it is? $2.5 billion.**

A: Dude, let's LBO that. Let's LBO it. And I think, so you read this article recently where you were saying over the last three years, TSMC has done $100 billion of CapEx. It's like 30, 30, 40. And if you think about, I mean, a small fraction of that is sort of like being used by Nvidia for the three nanometer that it's going to or, you know, previously for an animator that that's using for his chips. But Nvidia has turned that into what was what are it's like? Your earnings last quarter was like $40 billion, and so $40 billion times four, so $160 billion. So Nvidia alone is turning some small fraction of $100 billion in CapEx that's going to be depreciated over many years, not just this one year, into $160 billion in a single year. And then that gets even more intense when you go down the supply chain to ASML, which is taking a billion dollars worth of machines to produce a gigawatt. And then, of course, those machines last for more than a year, right?

---

**Q: And so if you have all those old wafers and then there's maybe a 50% haircut because the process, you know, the bits per wafer area are like What is it, 50% less or something? Then it's like, it doesn't seem like that bad to just bring on seven nanometer wafers and then, oh, that gives you another 50 or another 100 gigawatts. Yeah, tell me why that's naive.**

A: Yeah, so I think, you know, we potentially do go crazy enough that this happens because we just need incremental compute and the compute is worth the higher cost, power, et cetera, of these chips. But it's also unlikely to some extent, to a large extent, because of, I think, just comparing, you know, some of these are like not fair comparisons, right? For example, you know, from A100, which is 312 teraflops to Blackwell, which is like 1,000-ish of FP16, or maybe it's 2,000 and then Rubin is like 5,000 or so FP16. It's not a fair comparison because these chips have vastly different You know, design targets, right? At A100, that is what Nvidia optimized for was FP16, BF16 numerics. When you look at Hopper, they didn't care as much about that. They cared about FP8. When you look at Rubin, they don't care about FP16 and BF16 as much. They care mostly about FP4 and 6, right? And so numerics are what they've designed their chip for.

---

**Q: So if we end up in this world in 2030, where the West has the most advanced process technology, but it has not ramped it up as much, whereas China, I don't know if you think by 2030, they would have EUV and, I don't know, 2 nanometer or whatever, but they are a semiconductor pill, so they're producing in mass quantity.**

A: To date, China still does not have, you know, entire indigenized semiconductor supply chain. Right. But within 2030. Yeah. By 2030, it's it's possible that they do. But but to date, right. All of China's seven nanometer and 14 nanometer capacity uses ASML DUV tools. Right. And the amount that they can ship and import from ASML is large. But the point being that the vast majority of ASML's revenue, especially on EUV, all of it is outside of China. So the scale advantage is still in the favor of the, let's call it the West plus Taiwan, Japan, et cetera.

---

**Q: So if EUV becomes a bottleneck, what if we just went back to 7 nanometer and do what China is doing currently in producing 7 nanometer ships with multi-patterning with DUV machines?**

A: There's a couple like, you know, okay, let's just say, let's redesign, let's make a new chip design on seven nanometers. Sure, we can do that. And then it's optimized for the numerics of the modern day. The performance difference is still going to be much larger than the flops difference you mentioned, right? Often it's easy to boil things down to flops per watt or flops per dollar. But that's actually not a fair comparison. And so this is where you can bring in, hey, let's look at Kimi K1 or DeepSeek. When you look at Kimi K2.5 and DeepSeek, when you look at these two models and you look at their performance on Hopper versus Blackwell on very optimized software, you get vastly different performance. And Most of this is not attributed to flops or numerics, right? Because those models are actually 8-bit. So it's not like Blackwell's and Hopper, they're both optimized for 8-bit and Blackwell's not really taking advantage of its 4-bit there. The performance gulf is actually much larger.

---

**Q: If we end up in this world in 2030, where the West has the most advanced process technology, but it has not ramped it up as much, whereas China, I don't know if you think by 2030, they would have EUV and, I don't know, 2 nanometer or whatever, but they are a semiconductor pill, so they're producing in mass quantity.**

A: To date, China still does not have, you know, entire indigenized semiconductor supply chain. Right. But within 2030. Yeah. By 2030, it's it's possible that they do. But but to date, right. All of China's seven nanometer and 14 nanometer capacity uses ASML DUV tools. Right. And the amount that they can ship and import from ASML is large. But the point being that the vast majority of ASML's revenue, especially on EUV, all of it is outside of China. So the scale advantage is still in the favor of the, let's call it the West plus Taiwan, Japan, et cetera.

---

**Q: So then there's a question of like, where can you destroy demand to free up enough for AI?**

A: The incremental purchaser who's willing to pay the highest price for tokens also ends up being the one that's like, They're less price sensitive and the compute should be allocated in a capitalistic society towards the goods that have the highest value and the private market determines this by willingness to pay. To some extent, sure, Anthropic could actually release a slow mode. They could release Claude slow mode and have an increase in tokens per dollar by a significant amount. They could probably reduce the price of Opus 4.6 by You know, 4x, 5x and reduce the speed by another by maybe just like 2x like the curve on inference throughput versus speed is there already just on HBM and yet they don't because no one actually wants to use a slow model and furthermore on these agentic tasks.

---

**Q: And so is it possible to go to HBM accelerators and basically have the opposite of Claude Code fast, like have Claude Code slow and do that?**

A: It's great that the model can run at this time horizon of hours. It's kind of like, okay, well, if the model was just running slower, that hours would become a day, right? Or vice versa, right? If the model is running faster, that hours becomes hour. And yet, no one really wants to move to that day-long wait period because the highest value tasks also have some time sensitivity to them, right? And so I struggle to see, you know, yes, you could use DDR, but then there's a couple like things that are challenging with this, right? You could use regular DRAM.

---

**Q: What is the bandwidth difference between HBM and A normal DRM?**

A: So an HBM stack of HBM4, let's just talk about like the stuff that's in Rubin because that's what we've been indexing on, is 2048 bits across connected in an area that's like 13 millimeters wide. So 2048 bits and it transfers memory at around 10 gigatransfers a second. So HBM, a stack of HBM4 is 2048 bits on an area that's 13 millimeters wide, roughly, or 11. And that's the shoreline that you're taking on the chip. And in that shoreline, you have 2048 bits transferring at 10 gigatransfers per second. You multiply those together and you divide by eight bits to bytes. You're at roughly two and a half terabytes a second per HBM stack, right? When you look at DDR, in that same area, it's maybe 64 or 128 bits wide. And that DDR5 is transferring at anywhere from 6.4 gigatransfers a second. To maybe 8,000 gigatransfers a second. So your bandwidth is significantly lower, right?

---

**Q: What does this imply for the next year or two of... Sorry for the run-on question. I think on your newsletter, you said 30% of the CapEx in 2026 of big tech is going towards memory.**

A: Memory crunch will continue to be harder and harder and prices continue to go up. And this affects different parts of the market differently, right? Gets to sort of the like, are people going to hate AI more and more? Yes, because now smartphones and PCs are not going to get incrementally better year on year. And in fact, they're getting incrementally worse.

---

**Q: If you look at the bill of materials of an iPhone, what fraction of it is the memory? Like how much more expensive does an iPhone get if the memory is 2x more expensive or whatever it has to be?**

A: So I believe an iPhone has 12 gigabytes of memory Each gig cost used to cost roughly three or four dollars. So it's 50 bucks but now the price of memory is like Triple, let's call it if it's now, it's $12 per gig for DDR. So now you're talking about $150 versus $50, right? $100 increase in cost on Apple. Also, Apple has some margin, they're not just going to eat the margin. So now that's $100 cost increase. That's just on the DRAM. The NAND also has the same sort of like market. So in fact, you know, it's probably $150 increase on the iPhone. Apple has to either pass it on to the consumer, A, or B, they have to eat it. I don't see Apple reducing their margin too much. Maybe they eat a little bit. But at the end of the day, that means the end consumer is paying $250 more for an iPhone.

---

**Q: What is this? What basically what should we expect over the next year or two as this memory crunch hits?**

A: Memory crunch will continue to be harder and harder and prices continue to go up. And this affects different parts of the market differently, right? Gets to sort of the like, are people going to hate AI more and more? Yes, because now smartphones and PCs are not going to get incrementally better year on year. And in fact, they're getting incrementally worse.

---

**Q: So it sounds like you think power can be arbitrarily scaled.**

A: Not arbitrarily, but yes. And I think, if I'm remembering correctly, your blog post on the power, how AI led to increasing power, you were like, where you were implying that GeoVernova and Mitsubishi and Siemens could produce in gas turbines was like 60 gigawatts a year. And then there's these other sources, but they're like less significant than the turbines. And so And only a fraction of that goes to AI, I assume. So, yeah, if in 2030 we have enough logic and memory to do 200 gigawatts a year, do you just think that these things are on a path to ramp up to more than 200 gigawatts a year or what do you see?

---

**Q: If you're Jensen or Sam Waltman or whoever who stands to gain a lot from scaling up AI compute, there's these stories that they'd go to TSMC and say, hey, why can't we actually Y and Z?**

A: It's a funny dynamic we saw in 2023-2024 and 2025. People who saw the energy bottleneck before others asymmetrically went to Siemens, Mitsubishi, and of course GE Vernova and bought up turbine capacity and now they're able to charge excess amounts for deploying these turbines places because of energy. In the same sense, this could be done for EUV except ASML is not just going to trust any random bozo who wants to buy EUV tools in the sense that these turbines are much cheaper than EUV tools, and there's many more of them produced, especially once you get to industrial gas turbines or like, you know, not just combine cycle, but like the cheaper, smaller, et cetera, less efficient ones. People put down deposits for these. So in a sense, someone could do this, right? Someone should go to the Netherlands and be like, I'll pay you a billion dollars.

# Outlines

## Big Tech's $600 Billion Capex Forecast and AI Labs' Funding: A Compute Timeline
[(00:00)](https://podwise.ai/dashboard/episodes/7508210?locate=0)
The discussion begins with an overview of the combined forecasted capital expenditures (capex) of Amazon, Meta, Google, and Microsoft, totaling $600 billion this year, which equates to approximately 50 gigawatts of compute. The question arises regarding the timeline for this capex to come online. A similar inquiry is made about AI labs like OpenAI and Anthropic, which have recently raised substantial funding ($110 billion and $30 billion, respectively). The question is posed: what are these labs raising all this money for if the yearly price of a one-gigawatt data center is around $13 billion?

---

## Hyperscaler Capex Spending: Turbine Deposits, Data Center Construction, and Power Agreements
[(01:41)](https://podwise.ai/dashboard/episodes/7508210?locate=101)
A portion of the $600 billion capex is for immediate compute, but much is for setup, including turbine deposits for 2028-2029 and data center construction for 2027. Power purchasing agreements and down payments also factor in. Of the 20 gigawatts deployed this year in America, Anthropic and OpenAI account for a significant portion, currently at 2 and 1.5 gigawatts, respectively. Anthropic's revenue growth implies a need to add four gigawatts of inference capacity, potentially requiring them to exceed 5 gigawatts by year's end.

---

## Anthropic's Compute Constraints: Lower Quality Providers and Financial Freakouts
[(03:48)](https://podwise.ai/dashboard/episodes/7508210?locate=228)
Anthropic, being conservative on compute, may miss its target of 5 gigawatts. To acquire compute in a pinch, they may have to go to lower quality providers like CoreWeave and Oracle, unlike OpenAI, which has been more aggressive in securing compute from various sources, including SoftBank Energy. Financial concerns arose last year when companies feared Anthropic couldn't pay for signed deals, but recent funding alleviates those concerns.

---

## Acquiring Compute in a Pinch: Neo Clouds, Shorter-Term Deals, and Higher Prices
[(06:17)](https://podwise.ai/dashboard/episodes/7508210?locate=377)
Acquiring compute in a pinch means potentially using "Neo clouds" and paying higher prices. While some capacity exists at hyperscalers, not all contracts are long-term. OpenAI has secured most of its compute through five-year deals. H100 prices have increased, with some AI labs signing deals as high as $2.40 for two to three years, resulting in higher margins.

---

## Neocloud Capacity and Revenue Sharing: Anthropic's 50% Markup
[(07:38)](https://podwise.ai/dashboard/episodes/7508210?locate=458)
While most capacity at Oracle and Coreweave is signed for long-term deals, anything going online this quarter is already sold. Some neoclouds and hyperscalers may sell capacity initially intended for internal use. Anthropic may pay a 50% markup through revenue sharing or last-minute spot compute due to its conservative approach.

---

## Locking in Compute: The Advantage of Early Commitment and GPU Depreciation Cycles
[(09:32)](https://podwise.ai/dashboard/episodes/7508210?locate=572)
For a period, companies hesitated to sign deals with Anthropic due to financial concerns. Having the best model allows companies to lock in compute in advance and secure better prices. The depreciation cycle of GPUs may be longer than five years, especially if AI takes off, potentially making building clouds more financially lucrative.

---

## GPU Depreciation and Gross Margins: A TCO Model Perspective
[(11:21)](https://podwise.ai/dashboard/episodes/7508210?locate=681)
The discussion shifts to the depreciation cycle of GPUs, with Michael Burry suggesting three years or less. A TCO model considers data center, networking, smart hands, spare parts, chip, and server costs. An H100 costs $1.40 an hour to deploy at volume across five years, yielding a 35% gross margin at a $2/hour deal.

---

## GPU Utility and Value: GPT 5.4 and the Increasing Worth of H100s
[(13:03)](https://podwise.ai/dashboard/episodes/7508210?locate=783)
The utility derived from a chip determines its price. GPT 5.4 is cheaper to run and better than GPT 4, allowing an H100 to serve more tokens of higher quality. The value of an H100 is now based on GPT 5.4's potential, not GPT 4's. An H100 is worth more today than it was three years ago.

---

## The Value of H100s with AGI Models and Dario's Conservative Compute Approach
[(15:51)](https://podwise.ai/dashboard/episodes/7508210?locate=951)
If AGI models are developed, an H100 could repay itself in months. Dario's conservative approach to compute is questioned, given the potential for data centers of geniuses to generate trillions in revenue. The point was to highlight the inconsistency in Dario's statements, not to convince him to "YOLO" on compute.

---

## The Rising Value of GPUs and the Elkin-Allen Effect on Model Margins
[(18:52)](https://podwise.ai/dashboard/episodes/7508210?locate=1132)
As models become more powerful, the value of a GPU increases. Committing to compute now is advantageous. The Elkin-Allen effect suggests that increasing the fixed cost of compute (GPUs) will push people to pay higher margins for better models.

---

## Long-Term Compute Contracts and Margin Accrual in the AI Supply Chain
[(21:18)](https://podwise.ai/dashboard/episodes/7508210?locate=1278)
Companies with long-term compute contracts have a margin advantage. The incremental added compute drives costs. Cloud players, chip vendors, and memory vendors can potentially accrue margin dollars. Model vendors are expected to see margins increase this year due to capacity constraints.

---

## Nvidia's Strategy: Fracturing Complementary Industries and TSMC's Allocations
[(24:28)](https://podwise.ai/dashboard/episodes/7508210?locate=1468)
Nvidia aims to fracture complementary industries to maximize leverage, allocating resources to random NeoClouds. TSMC is giving good allocations to companies doing CPUs, like Amazon's Graviton, viewing the CPU business as more stable.

---

## TSMC's Calculus: Market Signals and Nvidia's AGI-Pilled Approach
[(26:07)](https://podwise.ai/dashboard/episodes/7508210?locate=1567)
TSMC provides good allocations to CPU companies due to their stability. Nvidia is getting the majority of 3nm supply because they signaled demand earlier and checked with the supply chain. Nvidia is more "AGI-pilled" than Google or Amazon, seeing more demand.

---

## Google's TPU Bottleneck and Anthropic's Compute Acquisition
[(29:30)](https://podwise.ai/dashboard/episodes/7508210?locate=1770)
Google has to deploy GPUs because they don't have enough TPUs to fill their data centers. Google sold a million V7s to Anthropic because Anthropic saw the dislocation and negotiated a deal before Google realized its own needs.

---

## Google's Gemini ARR and AGI Awakening: Turbine Deposits and Power Agreements
[(31:23)](https://podwise.ai/dashboard/episodes/7508210?locate=1883)
Anthropic saw the opportunity to acquire TPUs before Google fully realized its potential. Google's Gemini ARR skyrocketed in Q4, indicating a delayed awakening to the AI opportunity. Since then, Google has become aggressively AGI-pilled, buying an energy company and securing long-term power agreements.

---

## Compute as the Biggest Bottleneck: The Semiconductor Supply Chain and Fab Construction
[(34:26)](https://podwise.ai/dashboard/episodes/7508210?locate=2066)
The biggest bottleneck is compute, with the semiconductor supply chain having the longest lead times. The bottlenecks have shifted from COAS and power to chips. Fab construction takes years, while data centers take less than a year.

---

## Shifting Capacity: From Mobile and PC to AI Chips and a Gigawatt Ceiling
[(35:59)](https://podwise.ai/dashboard/episodes/7508210?locate=2159)
Capacity has shifted from mobile and PC to data center chips. Nvidia is now the largest customer at TSMC and SK Hynix. There may be an absolute gigawatt ceiling based on the production of EUV machines.

---

## ASML as the Ultimate Bottleneck: EUV Tools and AI Compute Limits
[(37:03)](https://podwise.ai/dashboard/episodes/7508210?locate=2223)
By 2028-2029, the bottleneck falls to ASML, which makes EUV tools. They can only make about 70 now, growing to a little over 100 by the end of the decade. A gigawatt of Nvidia's Rubin chips requires 55,000 wafers of 3nm, 6,000 wafers of 5nm, and 170,000 wafers of DRAM, requiring 3.5 EUV tools.

---

## Carl Zeiss and TSMC's CapEx: Bottlenecks and Nvidia's Earnings
[(41:07)](https://podwise.ai/dashboard/episodes/7508210?locate=2467)
Carl Zeiss, the optics supplier bottlenecking ASML, has a market cap of $2.5 billion. TSMC has done $100 billion of CapEx over the last three years. Nvidia is turning a small fraction of that into $160 billion in a single year.

---

## Sam Altman's Gigawatt Goal: EUV Tools and AI Chip Allocation
[(42:35)](https://podwise.ai/dashboard/episodes/7508210?locate=2555)
By 2030, there will be about 700 EUV tools, satisfying 200 gigawatts of AI chips. Sam Altman's goal of a gigawatt a week is compatible, requiring 25% market share. The same machines shipped in 2020 will be used in 2030.

---

## ASML's Generosity: EUV Tool Improvements and Pricing
[(44:01)](https://podwise.ai/dashboard/episodes/7508210?locate=2641)
ASML has been shipping EUV tools for a decade, with mass production around 2020. The tools are not the same, with improvements in throughput and overlay. ASML has not raised prices more than the capability increase.

---

## ASML's Supply Chain: Complex Components and AGI-Pilledness
[(46:10)](https://podwise.ai/dashboard/episodes/7508210?locate=2770)
ASML has not decided to expand capacity as fast as possible. The tool has four major components with complex supply chains. Nvidia had to get the entire supply chain to deliver capacity, but Anthropic and OpenAI are still short. The time lag for the AI-pilledness and desire to increase production is long.

---

## Returning to 7nm: Multi-Patterning and Process Improvements
[(55:00)](https://podwise.ai/dashboard/episodes/7508210?locate=3300)
If EUV becomes a bottleneck, could we return to 7nm and multi-patterning with DUV machines? There has been progress from A100 to B100, with a 3X improvement holding numerics constant. It may not be that bad to bring on 7nm wafers, giving another 50-100 gigawatts.

---

## Unfair Comparisons: Numerics and Design Targets in GPU Performance
[(58:12)](https://podwise.ai/dashboard/episodes/7508210?locate=3492)
Comparing A100 to Blackwell is not fair because they have different design targets. Numerics are what they've designed their chip for. The performance difference is still going to be much larger than the flops difference.

---

## Model Performance and Chip Communication: The Impact of Process Node Shrinking
[(1:00:21)](https://podwise.ai/dashboard/episodes/7508210?locate=3621)
Models don't run on a single chip, but hundreds. Every time you cross the barrier of a chip to another chip, there is an efficiency loss. As you shrink the process node, you increase the amount of compute in a single chip.

---

## Hopper vs. Blackwell: Performance Differences and Packaging Limitations
[(1:02:30)](https://podwise.ai/dashboard/episodes/7508210?locate=3750)
Even if Hopper and Blackwell are using a rack worth of chips, Hopper is slower due to performance limitations. Some architectural improvements cannot be ported back to A100. Blackwell has two dies on a single chip, and Rubin Ultra will have four.

---

## China's Semiconductor Ambitions: Scale vs. Process Technology
[(1:05:00)](https://podwise.ai/dashboard/episodes/7508210?locate=3900)
If the West has the most advanced process technology but hasn't ramped it up as much, and China is producing in mass quantity, what is the year where China is ahead in its ability to produce mass flops?

---

## China's Semiconductor Supply Chain: EUV Tools and Production Challenges
[(1:06:40)](https://podwise.ai/dashboard/episodes/7508210?locate=4000)
China does not have an entirely indigenized semiconductor supply chain. Their 7nm and 14nm capacity uses ASML DUV tools. They are trying to make their own DUV and EUV tools. It's possible they will have fully indigenized EUV by 2030.

---

## Chinese Production Capacity: DUV Tools and AGI Timelines
[(1:08:26)](https://podwise.ai/dashboard/episodes/7508210?locate=4106)
It's challenging to look into China's supply chain. They may be able to do 100 DUV tools a year. By when will China be able to have indigenized Chinese production bigger than the rest of the West combined? If we have long timelines on AI, should we expect a world where China is dominating in semiconductors?

---

## China's Model Capabilities and the Compute Race: A Diverging Path
[(1:10:55)](https://podwise.ai/dashboard/episodes/7508210?locate=4255)
It's challenging to make estimates far out. If takeoff timelines are slow enough, China could catch up drastically. Chinese models are competitive, but Opus 4.6 and GPT 5.4 have pulled away. As we move to selling automated white-collar work, the ability to distill American models into Chinese models will be harder.

---

## US Economic Growth and the Return on Invested Capital in Data Centers
[(1:12:21)](https://podwise.ai/dashboard/episodes/7508210?locate=4341)
China is not scaling their AI lab compute as fast. The US economy may grow faster due to capex and revenue from models. Anthropic's revenue implies $50 billion of capex. China has not done this.

---

## Fast vs. Long Timelines: US Wins vs. China Wins in AI
[(1:14:18)](https://podwise.ai/dashboard/episodes/7508210?locate=4458)
If infrastructure investments have middling returns, China may scale past the US. Fast timelines mean the US wins, long timelines mean China wins.

---

## Memory Crunch: HBM vs. Commodity DRAM and Agentic Tasks
[(1:16:10)](https://podwise.ai/dashboard/episodes/7508210?locate=4570)
HBM has three to four times less bits per wafer area than DRAM. Could accelerators use commodity DRAM instead of HBM? If we have agents doing work, we may not need extremely fast latency.

---

## The Highest Value Tasks: Time Sensitivity and the Demand for Speed
[(1:17:35)](https://podwise.ai/dashboard/episodes/7508210?locate=4655)
The incremental purchaser willing to pay the highest price for tokens is less price-sensitive. Anthropic could release a slow mode, but no one wants to use a slow model. The highest value tasks have some time sensitivity.

---

## Chip IO and Bandwidth: The Constraints of DDR vs. HBM
[(1:18:39)](https://podwise.ai/dashboard/episodes/7508210?locate=4719)
If you switch from HBM to DDR, the IO on the edge would have significantly less bandwidth. The metric that matters is bandwidth per wafer, not bits per wafer.

---

## Memory Capacity and System Design: The Four Constraints of GPU Performance
[(1:20:21)](https://podwise.ai/dashboard/episodes/7508210?locate=4821)
GPUs are not always running at full memory capacity. You can be constrained by flops, network bandwidth, memory bandwidth, or memory capacity.

---

## HBM vs. DDR: Bandwidth Differences and Consumer Demand Destruction
[(1:21:21)](https://podwise.ai/dashboard/episodes/7508210?locate=4881)
An HBM4 stack is 2048 bits on an area that's 13 millimeters wide, transferring at 10 gigatransfers per second, yielding 2.5 terabytes a second. DDR is significantly lower. You have to destroy 4X as much consumer demand to free up one byte for AI.

---

## Memory Crunch: Smartphone Volumes and the Impact on Consumers
[(1:23:34)](https://podwise.ai/dashboard/episodes/7508210?locate=5014)
The memory crunch will continue, affecting different parts of the market. Smartphones and PCs are not getting incrementally better. An iPhone gets $150 more expensive due to memory.

---

## Smartphone Volumes and Memory Allocation: The Consumer Impact
[(1:25:13)](https://podwise.ai/dashboard/episodes/7508210?locate=5113)
Smartphone volumes are halving in the low and mid-range. The percentage of the bomb that goes to memory and storage is larger, and the margins are lower.

---

## DRAM vs. NAND: Price Increases and Consumer Sentiment
[(1:26:32)](https://podwise.ai/dashboard/episodes/7508210?locate=5192)
DRAM gets released and goes to AI chips. People are hating AI more because memory prices have doubled.

---

## NAND and EUV: The Constraints on Logic and Memory Scaling
[(1:27:36)](https://podwise.ai/dashboard/episodes/7508210?locate=5256)
NAND is also going up in price. The same constraints preventing logic scaling are preventing more memory wafers. The EUV tool is needed for memory.

---

## Memory Vendor Fabs: Building Delays and Capacity Expansion
[(1:29:14)](https://podwise.ai/dashboard/episodes/7508210?locate=5354)
Memory vendors have not built new fabs because memory prices were low. It took a year for long context to reflect in memory prices. Those fabs take two years to build.

---

## Tooling Bottlenecks: The Complexity of Fab Construction
[(1:30:52)](https://podwise.ai/dashboard/episodes/7508210?locate=5452)
There's nowhere to put the tools. It's not just EUV. The most complex building that people make is fabs, and fabs take two years to build.

---

## Elon's Gigafab: Clean Rooms and Process Technology
[(1:32:02)](https://podwise.ai/dashboard/episodes/7508210?locate=5522)
Elon wants to build a fab that's a million wafers per month. He can recruit people and build a clean room. The complex part is developing a process technology.

---

## Disruptive Technologies: EUV Alternatives and Elon's Approach
[(1:33:45)](https://podwise.ai/dashboard/episodes/7508210?locate=5625)
What probability should we put on something totally out of the left field coming out and none of this is relevant? Something that's very simple and easy to scale has a very low probability.

---

## 3D DRAM: DUV and EUV in Memory Production
[(1:36:26)](https://podwise.ai/dashboard/episodes/7508210?locate=5786)
Could we build 3D DRAM the way we do 3D NAND and then go back to DUV? The hope is that you'll still use EUV.

---

## 3D DRAM Retooling: Fab Shifts and Tool Breakdown
[(1:38:04)](https://podwise.ai/dashboard/episodes/7508210?locate=5884)
3D DRAM would require a huge retooling of fabs. Existing DRAM fabs will require a lot of retooling just to go from one alpha to one beta to one gamma process nodes.

---

## Lithography Costs: EUV and 3D DRAM
[(1:39:22)](https://podwise.ai/dashboard/episodes/7508210?locate=5962)
EUV demand as a percentage of wafer costs has trended up. If we get to 3D DRAM, it tanks again in terms of the total end wafer cost as a percentage of EUV.

---

## Pitching ASML: Demand Signals and Capacity Arbitrage
[(1:40:47)](https://podwise.ai/dashboard/episodes/7508210?locate=6047)
It doesn't really matter what TSMC does. Should Silicon Valley people be pitching ASML to make more tools? Someone could go to the Netherlands and pay a billion dollars for the right to purchase 10 EUV tools two years from now.

---

## Power Scaling: Turbines and Critical IT Capacity
[(1:42:52)](https://podwise.ai/dashboard/episodes/7508210?locate=6172)
Power can be arbitrarily scaled. GeoVernova and Mitsubishi and Siemens could produce 60 gigawatts a year. This is critical IT capacity.

---

## Power Generation: Reciprocating Engines and Utility Scale Batteries
[(1:44:50)](https://podwise.ai/dashboard/episodes/7508210?locate=6290)
There's more we can do than just turbines. There are medium-speed reciprocating engines, ship engines, Bloom Energy fuel cells, solar plus battery, and wind. If you put enough utility-scale batteries, you've unlocked 20% of the US grid for data centers.

---

## Permitting and Power: The Challenges of Data Center Construction
[(1:47:31)](https://podwise.ai/dashboard/episodes/7508210?locate=6451)
Permitting is a challenge, but America is a big place. People are diversifying to Australia, Malaysia, Indonesia, and India.

---

## Power Costs and Model Improvements: The Value of Energy Efficiency
[(1:48:27)](https://podwise.ai/dashboard/episodes/7508210?locate=6507)
It makes less sense to consider the fact that energy is a small fraction of the cost of ownership of a data center. Combined cycle gas turbines have capex of $1,500 per kilowatt.

---

## Gas Generation: Unlocking Gigawatts and Electrician Wages
[(1:49:18)](https://podwise.ai/dashboard/episodes/7508210?locate=6558)
From the different sources of gas generation, how many gigawatts could they unlock by the end of the decade? There are over 16 different manufacturers of power-generating things just from gas alone.

---

## Labor Constraints: Modularization and Factory Production
[(1:51:11)](https://podwise.ai/dashboard/episodes/7508210?locate=6671)
Labor is a humongous constraint. We may start importing the highest skilled labor. The main factor for reducing the number of people is modularizing things and making them in factories in Asia.

---

## Modularization and Cabling: Reducing Labor in Data Centers
[(1:52:31)](https://podwise.ai/dashboard/episodes/7508210?locate=6751)
More and more built-out sections of the data center will be shipped in. You'll ship a fully integrated thing that has a lot of the cooling subsystems already put together.

---

## Space GPUs: Permitting and Land Availability
[(1:54:57)](https://podwise.ai/dashboard/episodes/7508210?locate=6897)
If you're right that power is not a constraint on Earth, the other reason they would make sense is that you can't get the permitting to build hundreds of gigawatts on Earth. America is big, and data centers don't take that much space.

---

## Texas Permitting: Red Tape and Labor Availability
[(1:56:01)](https://podwise.ai/dashboard/episodes/7508210?locate=6961)
Elon had to deal with complex stuff in Memphis. There's a lot more you can get away with in the middle of Texas.

---

## Space Data Centers: Economic Arguments and Power Costs
[(1:57:11)](https://podwise.ai/dashboard/episodes/7508210?locate=7031)
The economic argument makes less sense once you consider that energy is a small fraction of the cost of ownership of a data center.

---

## GPU Unreliability: Testing and Deployment Delays
[(1:58:05)](https://podwise.ai/dashboard/episodes/7508210?locate=7085)
GPUs are horrendously unreliable. 15% of Blackwells have to be RMA'd. If a GPU has a useful life of five years, and it takes six additional months, then that is 10% of your cluster's useful life.

---

## Space Communication: Topology and Bandwidth Limitations
[(1:59:20)](https://podwise.ai/dashboard/episodes/7508210?locate=7160)
Starlink satellites talk to each other at 100 gigabits per second. That ends up being quite close to the InfiniBand bandwidth.

---

## Space Data Centers: Contended Resources and Terrestrial Alternatives
[(2:01:21)](https://podwise.ai/dashboard/episodes/7508210?locate=7281)
Space data centers are limited by the same contended resource. It doesn't matter if it's on land or in space. It is much further out once you have energy constraints actually being a big bottleneck.

---

## Chip Deployment: Speed and Optimization in a Chip-Constrained World
[(2:03:11)](https://podwise.ai/dashboard/episodes/7508210?locate=7391)
In a chip-constrained world, get these chips working on producing tokens ASAP. Elon doesn't win by doing 20% gains. Space data centers will eventually be a 10x gain, potentially, as Earth's resources get more and more contentious.

---

## Power Density: Watts per Millimeter and Cooling Challenges
[(2:04:58)](https://podwise.ai/dashboard/episodes/7508210?locate=7498)
One easy way is to pump that to 2 watts per millimeter squared. It requires more complicated cold plates and very complicated liquid cooling, or maybe it requires things like emergent cooling.

---

## Scale-Up Domains: Nvidia, Google, and Amazon Topologies
[(2:06:27)](https://podwise.ai/dashboard/episodes/7508210?locate=7587)
Scale-up domain is the tight domain where the chips are communicating on the order of terabytes a second. For Nvidia, all 72 GPUs in the rack could connect to each other at terabytes a second speed. Google has a topology that's a torus.

---

## Parameter Scaling: Memory Capacity and Compute Efficiency
[(2:09:15)](https://podwise.ai/dashboard/episodes/7508210?locate=7755)
The reason that parameter scaling has been slow is that Nvidia's scale-ups have not had that much memory capacity. The compute efficiency gains you get from research are so large, you actually want most of your compute to go to research, not to development.

---

## SME Analysis: Leopold's Success and Market Inefficiencies
[(2:14:24)](https://podwise.ai/dashboard/episodes/7508210?locate=8064)
Why is Leopold the only person that is using your spreadsheets to make outrageous money? What is everybody else doing?

---

## The Memory Crunch: Belief in AI and Market Predictions
[(2:17:11)](https://podwise.ai/dashboard/episodes/7508210?locate=8231)
You only buy the memory crunch if you believe AI is going to take off in a huge way. A year ago, if you told someone memory prices were quadruple and smartphone volumes are going to go down 40% over a year or two after that, people were like, you're crazy.

---

## TSMC and Apple: Capacity and Pre-Booking
[(2:18:44)](https://podwise.ai/dashboard/episodes/7508210?locate=8324)
Can TSMC kick out Apple if Nvidia and Amazon and Google say, hey, we're willing to pay a lot of money for N2 capacity? TSMC is not going to kick Apple out entirely.

---

## Apple's Declining Relevance: Process Nodes and Supply Chain Constraints
[(2:20:26)](https://podwise.ai/dashboard/episodes/7508210?locate=8426)
Apple will become a smaller and smaller percentage of TSMC's revenue. They will also just cut their orders because things in the supply chain are kicking them out.

---

## Huawei's Potential: Process Technology and AI Talent
[(2:22:33)](https://podwise.ai/dashboard/episodes/7508210?locate=8553)
Do you think if Huawei had access to three nanometer, they would have a better accelerator than Rubin? Huawei is arguably the only company in the world that has all the legs.

---

## Humanoid Robots: Local Compute and Centralized Intelligence
[(2:24:04)](https://podwise.ai/dashboard/episodes/7508210?locate=8644)
If humanoids take off faster than people expect, what will be required for that? You don't need to have all the intelligence in the robot.

---

## Centralized Intelligence: The Future of Robotics and Elon's Robot Chips
[(2:27:02)](https://podwise.ai/dashboard/episodes/7508210?locate=8822)
The future is one where there's centralized thinking and centralized computation that's driving millions of robots out in the world. Elon recognizes this, which is why he's going to different places for his chips.

---

## Taiwan Risk: Process Engineers and Semiconductor Supply Chains
[(2:28:52)](https://podwise.ai/dashboard/episodes/7508210?locate=8932)
How much of Taiwan's place in the semiconductor supply chain could we de-risk simply by having a plan to airlift every single process engineer at TSMC out when things come to? If you ship out all the process engineers and blow up the fabs, China has a stronger semiconductor supply chain than the rest of the world.

# Keywords

|Keywords|Explanation|
|---|---|
|Semianalysis|Dylan Patel's company, which provides in-depth research and analysis of the semiconductor industry. Semianalysis offers insights into market trends, technological advancements, and competitive landscapes.|
|Capex|Short for capital expenditure, refers to funds used by a company to acquire, upgrade, and maintain physical assets such as property, buildings, or equipment. In the context of the podcast, it refers to the significant investments made by tech giants like Amazon, Meta, Google, and Microsoft in computing infrastructure.|
|Hyperscalers|Companies that operate massive data centers and cloud computing infrastructure, such as Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). These companies invest heavily in hardware and software to support their cloud services and internal operations.|
|EUV (Extreme Ultraviolet) Lithography|An advanced technology used in semiconductor manufacturing to create extremely fine patterns on silicon wafers. EUV tools are essential for producing the most advanced chips, but their limited availability constrains overall chip production capacity.|
|HBM (High Bandwidth Memory)|A type of high-performance memory that is stacked vertically to provide significantly higher bandwidth compared to traditional DRAM. HBM is crucial for AI accelerators, as it enables faster data transfer between the processor and memory.|
|DRAM (Dynamic Random-Access Memory)|A type of volatile memory commonly used in computers and other electronic devices. DRAM stores each bit of data in a separate capacitor within an integrated circuit.|
|NAND Flash Memory|A type of non-volatile storage technology commonly used in SSDs, USB drives, and memory cards. NAND flash stores data in memory cells that retain information even when power is removed.|
|TSMC (Taiwan Semiconductor Manufacturing Company)|The world's largest dedicated independent semiconductor foundry. TSMC manufactures chips for a wide range of customers, including Apple, Nvidia, and AMD.|
|ASML|A Dutch company that is the primary manufacturer of EUV lithography systems. ASML's EUV tools are essential for producing the most advanced chips, making the company a critical player in the semiconductor industry.|
|AGI (Artificial General Intelligence)|A hypothetical level of AI that possesses human-like cognitive abilities and can perform any intellectual task that a human being can. The discussion revolves around how the pursuit of AGI is driving compute demand and infrastructure investments.|
|GPU (Graphics Processing Unit)|A specialized electronic circuit designed to rapidly manipulate and alter memory to accelerate the creation of images in a frame buffer intended for output to a display device. Modern GPUs are used for general-purpose computing, especially in AI and machine learning.|
|Inference|The process of using a trained machine learning model to make predictions or decisions on new data. Inference requires significant computing power, especially for large language models.|
|RL (Reinforcement Learning)|A type of machine learning where an agent learns to make decisions by interacting with an environment and receiving rewards or punishments. RL is used to train AI models for tasks such as robotics and game playing.|
|NVLink|A high-bandwidth, energy-efficient interconnect technology developed by Nvidia for connecting multiple GPUs together. NVLink enables faster communication between GPUs, improving performance in parallel computing applications.|
|OpenAI|A leading artificial intelligence research and deployment company. OpenAI is known for developing cutting-edge AI models such as GPT-4 and DALL-E.|

# Highlights

- [(15:44)](https://podwise.ai/dashboard/episodes/7508210?locate=944) And so you sort of have this dynamic that is quite interesting in that an H100 is worth more today than it was three years ago.
- [(27:35)](https://podwise.ai/dashboard/episodes/7508210?locate=1655) As a company that is conservative and doesn't want to ride cycles of growth too hard, you actually want to allocate to the market that is more stable and lower growth rate first before you allocate all the incremental capacity to the fast growth rate market.
- [(40:56)](https://podwise.ai/dashboard/episodes/7508210?locate=2456) It might be $100 billion worth of AI value into the supply chain is held up by this $1.2 billion worth of tooling that simply just cannot expand its supply chain quickly.
- [(45:50)](https://podwise.ai/dashboard/episodes/7508210?locate=2750) And yet they haven't taken price and margins up like crazy...ASML has never risen the price more than they've increased the capability of the tool. And so in a sense, they've always provided net benefit to their customer.
- [(1:07:51)](https://podwise.ai/dashboard/episodes/7508210?locate=4071) I think they'll have working tools. I don't think that they'll be able to manufacture A bunch yet right you know there's there's sort of having it work and then there's production hell right and ultimately like ASML had EUV working...Now, the tools were not accurate enough. They were not scaled for high production, scaled for high volume manufacturing, reliable enough.
- [(1:17:37)](https://podwise.ai/dashboard/episodes/7508210?locate=4657) the incremental purchaser who's willing to pay the highest price for tokens also ends up being the one that's like, They're less price sensitive and the compute should be allocated in a capitalistic society towards the goods that have the highest value and the private market determines this by willingness to pay.
- [(2:04:37)](https://podwise.ai/dashboard/episodes/7508210?locate=7477) Elon wins when he swings for the fences and does 10x gains...It's not been about chasing the 20%.
- [(2:29:55)](https://podwise.ai/dashboard/episodes/7508210?locate=8995) Just shipping out all the engineers and blowing up the fabs means China has a stronger semiconductor supply chain than the rest of the world.

# Transcript

**Dwarkesh:**
[(00:00)](https://podwise.ai/dashboard/episodes/7508210?locate=0)
Alright, this is the episode of My Roommate Teaches Me Semiconductors.

**Dylan Patel:**
[(00:03)](https://podwise.ai/dashboard/episodes/7508210?locate=3)
It's also the send-off for this current set.

**Dwarkesh:**
[(00:07)](https://podwise.ai/dashboard/episodes/7508210?locate=7)
Yeah, you know, after you use it, I'm like, I can't use this again.

**Unknown Speaker:**
[(00:10)](https://podwise.ai/dashboard/episodes/7508210?locate=10)
I gotta get out of here.

**Dylan Patel:**
[(00:11)](https://podwise.ai/dashboard/episodes/7508210?locate=11)
No sloppy seconds for Dwarkesh.

**Dwarkesh:**
[(00:14)](https://podwise.ai/dashboard/episodes/7508210?locate=14)
Okay, Dylan is the CEO of Semianalysis. Dylan, the burning question I have for you, if you add up the big four,  Amazon, Meta, Google, Microsoft, their combined forecasted capex that you published recently, this year is $600 billion. And given yearly prices of renting that compute, that would be like close to 50 gigawatts. Now, obviously, we're not putting on 50 gigawatts this year. So presumably, that's paying for compute that is going to be coming online over the coming years. So I have a question about how to think about the timeline around when that CapEx comes online. Similar question for the labs where, you know, OpenAI just announced that they raised $110 billion.

[(00:56)](https://podwise.ai/dashboard/episodes/7508210?locate=56)
Anthropic just announced they raised $30 billion. And if you look at the compute that they have coming online this year,  you should tell me how much it is, but like,  is it not another four gigawatts total that they'll have this year? It feels like the cost to rent the compute that OpenAI and Anthropic will have this year to like sustain their compute spend,  At, you know, 10, $13 billion a gigawatt. Those individual raises alone are like enough to cover their compute spend for the year. And then this is not even including the revenue that they're going to earn this year. So help me understand first, when is the timescale at which the big tech CapEx is actually coming online? And two,

[(01:33)](https://podwise.ai/dashboard/episodes/7508210?locate=93)
 what are the labs raising all this money for if like the yearly price of a one gigawatt data center is like $13 billion?

**Dylan Patel:**
[(01:41)](https://podwise.ai/dashboard/episodes/7508210?locate=101)
So, when you talk about the CapEx of these hyperscalers, right, on the order of $600 billion,  and you look at the cross the rest of the supply chain,  gets you to on the order of a trillion dollars. A portion of this is, you know, immediately for compute going online this year, right? The chips and the other parts of CapEx that do get paid this year. But there's a lot of setup CapEx as well, right? So, when we're talking about 20 gigawatts this year in America, roughly- Incremental. Incremental added capacity. A portion of this is not spent this year. A portion of that CapEx was actually spent the prior year. And so when you look at, hey, Google's got $180 billion.

[(02:20)](https://podwise.ai/dashboard/episodes/7508210?locate=140)
Actually, a big chunk of that is spent on turbine deposits for 28 and 29.  A chunk of that is spent on data center construction for 27.  A chunk of that is spent on, you know,  Power purchasing agreements and down payments and all these other things that they're doing for further out into the future so that they can set up this super fast scaling,  right? And this applies to all the hyperscalers and other people in the supply chain. And so, you know, 20 gigawatts roughly deployed this year, a big chunk of that being hyperscalers, a chunk not being. And all of these companies, their biggest customers are Anthropic and OpenAI. Anthropic and OpenAI are in the, you know, two gigawatt and, you know,

[(03:00)](https://podwise.ai/dashboard/episodes/7508210?locate=180)
 two and a half gigawatt and one and a half gigawatts roughly right now. They're trying to scale to much larger, right? If you look at what Anthropic has done over the last few months, you know, $4 billion, $6 billion revenue added. And if we just draw a straight line, hey, yeah, they'll add another $6 billion of revenue a month. People would argue that's bearish and that they should go faster. What that implies is that they're going to add $60 billion of revenue across the next 10 months, right? And $60 billion of revenue at the current gross margins that Anthropic had, at least last reported by media,

[(03:33)](https://podwise.ai/dashboard/episodes/7508210?locate=213)
 would imply that they have roughly $40 billion of compute spend for that inference for that 60 bill of revenue. That 40 billion of compute at roughly 10 billion dollars a gigawatt rental cost means that they need to add four gigawatts of inference capacity just to grow revenue. And that's saying that their research and development training fleet stays flat. Right. So. In a sense, Anthropic needs to get to well above 5 gigawatts by the end of this year,  and it's going to be really tough for them to get there, but it's possible.

**Dwarkesh:**
[(04:02)](https://podwise.ai/dashboard/episodes/7508210?locate=242)
Can I ask a question about that?

**Dylan Patel:**
[(04:03)](https://podwise.ai/dashboard/episodes/7508210?locate=243)
Yeah.

**Dwarkesh:**
[(04:04)](https://podwise.ai/dashboard/episodes/7508210?locate=244)
If Anthropic was not on track to have 5 gigawatts by the end of this year,  but it needs that to serve both the revenue that's gone crazier than expected,  and maybe it's going to be even more than that,  plus the research and training to make sure its models are good enough for next year. How, how, where is that going to come from?

**Dylan Patel:**
[(04:20)](https://podwise.ai/dashboard/episodes/7508210?locate=260)
You know, Dario, when he was on your podcast was very, very like conservative. He's like, you know,  I'm not going to go crazy on compute because if my revenue inflects at a different rate at a different point,  I don't want to go bankrupt. You know, I want to make sure that we're being responsible with this. Scaling, but in reality, he's definitely missed the pooch in terms of going like OpenAI,  which was, let's just sign these crazy fucking deals. And OpenAI has got way more access to compute than Anthropic by the end of the year. And so what does Anthropic have to do to get the compute? Well, they have to go to lower quality providers that they would not have gone to before, right?

[(04:55)](https://podwise.ai/dashboard/episodes/7508210?locate=295)
You know, optimally, you know, Anthropic, at least historically, has had the best quality providers, been like Google and Amazon. Whereas, you know, at least historically minded, you know, the biggest companies in the world,  now Microsoft, and now they're expanding across the supply chain and going to other players that are newer. OpenAI has been, you know, a bit more aggressive on going to many players. Yes, they have tons of capacity from Microsoft, They have Google and Amazon as well,  but they also have tons with CoreWeave and Oracle. They've gone to random companies, or one would think random companies like SoftBank Energy,  who has never built a data center in their life,

[(05:27)](https://podwise.ai/dashboard/episodes/7508210?locate=327)
 but they're building data centers now for OpenAI. They've gone to, and many others like Nscale and others, that they're going and getting capacity from. There's this like, Conundrum for Anthropic, because they were so conservative on compute, because they didn't want to go crazy,  right? In some sense, a lot of the financial freakouts in the second half of last year were like,  okay, I signed all these deals, but they don't have the money to pay for them. Okay, Oracle stock's going to tank. Okay, Core Reef stock's going to tank. Okay, like, you know, all these companies' stocks tanked,  and credit markets went crazy because people were like,  the end buyer can't pay for this.

[(06:02)](https://podwise.ai/dashboard/episodes/7508210?locate=362)
Now it's like, oh, wait, they raised a ton of money. Okay, fine, they can pay for it. But In the sense, Anthropic was a lot more conservative. They were like, we'll sign contracts,  but we'll be principled and we'll purposely undershoot what we think we can possibly do and be conservative because we don't want to potentially go bankrupt.

**Dwarkesh:**
[(06:17)](https://podwise.ai/dashboard/episodes/7508210?locate=377)
The thing I want to understand is, so what does it mean to have to acquire compute in a pinch? Is it that you have to go with like Neo clouds? Is it that they have worse computers? In what way is it worse? And is it that you had to pay gross margins to a cloud provider that you wouldn't have otherwise had to pay to because they're coming in at the last minute? Who built the spare capacity such that it's available for Anthropic and OpenAI to get last minute? And like, basically, what is the concrete advantage that OpenAI has gotten if they end up at similar compute numbers by 2027?  Is it just like they're going to end this year with different gigawatts?

[(06:50)](https://podwise.ai/dashboard/episodes/7508210?locate=410)
If so, how many gigawatts is Anthropic and OpenAI going to have by the end of this year?

**Dylan Patel:**
[(06:54)](https://podwise.ai/dashboard/episodes/7508210?locate=414)
Yeah. To acquire XS Compute, I mean, yes, there is capacity at hyperscalers and not all contracts for compute are long-term,  right? Five years, right? There's compute that in 2023 or 2024, H100, 2025, that were signed at not five-year deals, right? OpenAI, the vast majority of their compute is signed at five-year deals. There were many other customers that had one-year, two-year, three-year deals, six-month deals on demand. As these contracts roll off, who is the participant in the market most willing to pay price? In this sense, we've seen H100 prices inflect a lot and go up,  and people willing to sign long-term deals as above $2 even.

[(07:38)](https://podwise.ai/dashboard/episodes/7508210?locate=458)
I've seen deals where certain AI labs I'm going to be a little bit vague here for a reason,  have signed at as high as $2.40 for two to three years for H100s,  which if you think about the margin,  $1.40 for Hopper when you release it or Hopper to build it across five years and now two years in your signing deals that are two to three years that are at $2.40,  those margins are way higher. Right. And so now you can crowd out all of these other suppliers,  whether it's Amazon had these or Coreweave had these or Together AI or Nebius or whoever it is. Right. You know, these Neo clouds. Are the firms that had a higher percentage of Hopper in general because they were more aggressive on it,

[(08:22)](https://podwise.ai/dashboard/episodes/7508210?locate=502)
 A, and B, they tended to sign shorter-term deals, not Corweave,  but the others tended to sign shorter-term deals. And so, hey, if I want Hopper, there is some capacity out there. And then also,  while most of the capacity at like an Oracle or a Corweave is signed for a long-term deal in terms of Blackwell,  anything that's going online this quarter is already sold. And in some cases, they're not even hitting all the numbers that they promised they would sell because there are some data center delays,  not just those two, but like Nebius and all the other folks, Microsoft, Amazon,  Google.

[(08:53)](https://podwise.ai/dashboard/episodes/7508210?locate=533)
But there is a lot of neoclouds as well as some of the hyperscalers who have capacity they're building that they did not sell yet or capacity that they were going to allocate to some internal use. That is not necessarily super AGI focused that they may now turn around and sell. Or they may, you know, in the case of Anthropic, they don't have to have all the compute directly, right? Amazon can have the compute,  they can serve Bedrock or Google can have the compute and serve Vertex or Microsoft can have the compute and serve Foundry and then do a revenue share with Anthropic or vice versa.

**Dwarkesh:**
[(09:20)](https://podwise.ai/dashboard/episodes/7508210?locate=560)
Basically,  you're saying Anthropic is having to pay either this like 50% markup in the sense of the revenue share or in the sense of Last minute spot compute that they wouldn't have otherwise had to pay had they bought the computer early.

**Dylan Patel:**
[(09:32)](https://podwise.ai/dashboard/episodes/7508210?locate=572)
Right. And, you know, there's a trade off there, but also at the same time,  you know, for a solid like four months, everyone was like, OK,  we're not going to sign deals with you. Like, that sounds crazy. Right. Because you guys don't have the money. Now everyone's like, yeah, OK, we believe you the whole time. We can we can sign any deal because you've raised all this money. But in a sense, Anthropic is constrained in that sense. There are not that many incremental buyers of compute yet because Anthropic hit the capabilities here first where their revenue is mooting.

**Dwarkesh:**
[(10:03)](https://podwise.ai/dashboard/episodes/7508210?locate=603)
Oh, that's interesting. Because otherwise you're like, well, having the best model is an extremely depreciating asset that three months later you don't have the best model. But the reason it's important is that you can sign these deals and then lock in the compute in advance,  get better prices. Doesn't this also imply, by the way, And maybe this is an obvious point,  but there's, at least until recently, people had made this huge point about, oh,  what is the depreciation cycle of a GPU? And the bears, Michael Burry's or whatever, have said, look,  people are saying that four or five years for these GPUs. And in fact, if you, maybe it's because the technology is improving so fast or whatever,

[(10:43)](https://podwise.ai/dashboard/episodes/7508210?locate=643)
 it might make sense to have two-year depreciation cycles for these GPUs. Which increases the sort of like reported amortized CapEx in a given year. And so it makes it maybe financially less lucrative to building all these clouds. But in fact, you're pointing at like Maybe the depreciation cycle is even longer than five years,  because if we're using hoppers, and then especially if AI really takes off and in 2030,  we're like, fuck, we got to like get the seven nanometer fabs up and we got to like,  we got to go back to the A100, like return on the A100s again. Then it's like actually the depreciation cycle is incredibly long.

[(11:16)](https://podwise.ai/dashboard/episodes/7508210?locate=676)
And so I think that's an interesting financial implication of what you're saying.

**Dylan Patel:**
[(11:21)](https://podwise.ai/dashboard/episodes/7508210?locate=681)
There's a few strings to pull on there. One is, What happens to depreciation of GPUs, right? And I guess I didn't answer your prior question, which is like anthropic. I think we'll be able to get to like five gigawatts-ish,  maybe a little bit more by the end of the year through themselves as well as their product being served through Bedrock or through Vertex or through Foundry. I think they'll be able to get to five or six gigawatts, which is way above their initial plans, right? And anyways, that's sort of like, and OpenAI will be roughly the same, maybe a little higher,  actually a little bit higher based on our numbers. Anyways, the depreciation cycle of a GPU, right?

[(12:02)](https://podwise.ai/dashboard/episodes/7508210?locate=722)
Michael Burry was saying it's, you know, three years or less, right? Is like sort of his argument. And there's sort of two ways and lenses to look at this. Like mechanically, in this, you know, there's a TCO model, right? Total cost of ownership of a GPU, where we sort of project pricing out for GPUs and build up the total cost of a cluster. But there's a number of costs, right? There's your data center cost, right? There's your networking costs, there's your smart hands and people in the data center swapping stuff out. There's your spare parts, there's your actual chip costs, there's your server costs.

[(12:32)](https://podwise.ai/dashboard/episodes/7508210?locate=752)
All these various costs get lumped together and there's some depreciation cycles on it, there's certain credit costs on it. And you get to, okay, that's how you build up, hey,  an H100 costs $1.40 an hour to deploy at volume across five years if your depreciation is five years. And then if you sign a deal at $2 an hour for those five years, your gross margin is roughly 35%. It's a little bit above that, but if you sign it for $1.90, it's 35% roughly. And then you assume at that fifth year, the GPU falls off a bus, right? It's dead. And in some cases, you know, sort of the argument people are making is,  well, If you didn't sign a long-term deal because every two years Nvidia's tripling,

[(13:11)](https://podwise.ai/dashboard/episodes/7508210?locate=791)
 quadrupling the performance while only 2x-ing the price or 50% increasing the price, then the price of an H100,  sure, maybe the value in the market was $2 at 35% gross margins in 2024. But in 2026,  when Blackwell is in super high volume and deploying millions a year, you're actually now worth $1 an hour. And when Rubin in 27 is in super high volume, even though it starts shipping this year,  is in super high volume next year, I'm doing millions of chips a year deployed into clouds. You've got another 3x in performance and another 50% or 2x in price. Actually, the hopper is only worth 70 cents an hour. And so the price of a GPU would continue to fall. That's like one lens.

[(13:51)](https://podwise.ai/dashboard/episodes/7508210?locate=831)
The other lens is what is the utility you get out of the chip, right? Because if you could build infinite Rubin or infinite of the newest chip, then yes, that's exactly what would happen. The price of a hopper would fall at a spot or a short-term contract rate As the new chips come out and the price per performance goes up,  but because you are so limited on semiconductors and deployment timelines and all these things,  you end up with actually what prices these chips is not, hey,  what's the comparative thing I can buy today? It's actually what is the value I can derive out of this chip today, right?

[(14:26)](https://podwise.ai/dashboard/episodes/7508210?locate=866)
And in that sense, Let's take GPT 5.4. GPT 5.4 is both way cheaper to run than GPT 4, has fewer active parameters. It's much smaller, right, in that sense of active parameters, plus because, you know,  a sparser MOE versus GPT 4 being a coarser MOE. There's also been so many other advancements in training, RL, model architecture, et cetera, et cetera, data qualities. All these things that have made GPT 5.4 way better than GPT 4 and it's cheaper to serve. And so when you look at an H100,  it can serve more tokens per GPU of 5.4 than if you had ran GPT 4 on it,  right? So at some sense, it's producing more tokens of a model that is of higher quality.

[(15:09)](https://podwise.ai/dashboard/episodes/7508210?locate=909)
And so in some sense, you know, obviously GPT 4, what is the maximum TAM for its tokens? You know, maybe it was a few billion dollars, maybe it was tens of billions of dollars, adoption takes time. For GPT 5.4, that number is probably north of 100 billion,  but there's an adoption lag and there's competition,  so other people are getting it, and there's the constant improvements that everyone else is having. So if improvements stopped here,  the value of an H100 is now predicated on the value that GPT 5.4 can get out of it instead of the value that GPT 4 can get out of it,  and the margins and all that stuff that these labs are doing, and they're in a competitive environment,

[(15:42)](https://podwise.ai/dashboard/episodes/7508210?locate=942)
 so their margins can't go to infinity. So you sort of have this dynamic that is quite interesting in that and H100 is worth more today than it was three years ago.

**Dwarkesh:**
[(15:51)](https://podwise.ai/dashboard/episodes/7508210?locate=951)
That's crazy. And I mean, it's also interesting from the perspective of like, just take that forward. If we had actual AGI models developed, if we had like genuinely human on a server and a human like On a flop basis,  an H100... These are such hand-wavy numbers about how many flops can the brain do. But on a flop basis, an H100 is estimated to... 1E15 is like how much some people estimate the human brain does in flops. Obviously, in terms of memory, the human brain has way more. H100 is like 80 gigabytes and brain might have petabytes.

**Dylan Patel:**
[(16:23)](https://podwise.ai/dashboard/episodes/7508210?locate=983)
Oh, yeah? You've got petabytes? Name a petabyte of ones and zeros, bro. Name me a string.

**Dwarkesh:**
[(16:31)](https://podwise.ai/dashboard/episodes/7508210?locate=991)
Well, this is actually the point where like actually in...

**Dylan Patel:**
[(16:33)](https://podwise.ai/dashboard/episodes/7508210?locate=993)
No, we've just got the best sparse attention techniques ever.

**Dwarkesh:**
[(16:36)](https://podwise.ai/dashboard/episodes/7508210?locate=996)
Genuinely, right? Like in this sort of like amount of information that is compressed, it might be petabytes,  but like the actual, you know, it's like extremely sparse MOE. But anyways, imagine if we had a human knowledge worker can produce six figures a year of value. And so if an age 100 can produce Something close to that,  if we had actual humans on the server,  the value of an H100 is like it can repay itself in the course of like a couple of months. So as I've been going through everything to prep for taxes,  I realized that I worked with over 50 different contractors last year,  from cinematographers to audio technicians to editors, and I owed all of them $10.99. In the past,

[(17:13)](https://podwise.ai/dashboard/episodes/7508210?locate=1033)
 I've just used a spreadsheet and a big folder of invoices to figure out who I need to collect tax forms from. But with so many contractors, this takes a bunch of time, and I've almost missed some people. This year, though, Mercury made my process way more straightforward. Whenever I pay somebody in 2025, I just hit a toggle to have Mercury request a W-9 from them. Because of that, everything that I needed to issue 1099s got sent directly to Mercury. I literally just clicked a button and Mercury generated and sent them all out. This is just one of the many things that I never would have assumed that a banking platform could just handle for me.

[(17:42)](https://podwise.ai/dashboard/episodes/7508210?locate=1062)
Mercury has a bunch of features like this, which are going to collectively save me multiple days this tax season. You can learn more at mercury.com. Mercury is a fintech company, not an FDIC insured bank. Banking services provided through Choice Financial Group and Column NA members FDIC. So when I interviewed Dario,  the point I was trying to make is not that I think the singularity is two years away and therefore Dario desperately needs to buy more compute,  although the revenue is certainly there that he needs to buy more compute. But the point I was trying to make is that given what Dario seems to be saying,  given his statements that we're two years away from a data center of geniuses,

[(18:19)](https://podwise.ai/dashboard/episodes/7508210?locate=1099)
 Certainly not more than five years away. And a data server geniuses should be earning trillions upon trillions of dollars of revenue. It just does not make sense why he keeps making these statements about being more conservative on compute or to your point,  being less aggressive than open AI on compute. And I guess that point got lost because then people were like roasting me about like,  oh, this podcast was like trying to convince this like multi hundred billion dollar company CEO,  like, why don't you YOLO it, bro? But no, I was trying to say that internally his statements are inconsistent. Anyway, so it's good to iron it out.

**Dylan Patel:**
[(18:52)](https://podwise.ai/dashboard/episodes/7508210?locate=1132)
Yeah, I think, you know, going back to like sort of the earlier view that if the models are so powerful,  the value of a GPU goes up over time.

**Dwarkesh:**
[(18:59)](https://podwise.ai/dashboard/episodes/7508210?locate=1139)
Yeah.

**Dylan Patel:**
[(19:00)](https://podwise.ai/dashboard/episodes/7508210?locate=1140)
As we approach closer and closer to, let's say,  a point where right now only OpenAI and Anthropic have that viewpoint. As we approach further and further out, actually everyone is going to, even with open source models,  be able to start to see that value skyrocket per GPU. In that sense, you should commit now to compute. Interestingly, in like an anthropic fashion, right? You know, there's a bit of a meme that they are, they don't,  they have problems with commitment issues and they're like sort of polyamorous. This is a bit of a meme.

**Dwarkesh:**
[(19:39)](https://podwise.ai/dashboard/episodes/7508210?locate=1179)
This explains everything. By the way, so there's this interesting economics effect called Elkin-Allen,  which is the idea that if you increase The fixed cost of different goods,  one of which is higher quality and one which is lower quality. That will make people choose the higher quality good on the margin. So to give a specific example, suppose the better tasting apple costs $2 and then like the shittier apple costs $1.  Okay, now suppose you put an import tariff on them. And so now it's $3 versus $2 for like great apple, medium apple, right?

**Dylan Patel:**
[(20:15)](https://podwise.ai/dashboard/episodes/7508210?locate=1215)
Is that because they both increased by a dollar or should it be like 50% increase?

**Dwarkesh:**
[(20:18)](https://podwise.ai/dashboard/episodes/7508210?locate=1218)
No, no, no, because if they both increased by a dollar,  the whole effect is that if there's a fixed cost that's applied to both,  The price difference between them, the ratio changes. So previously it was like the more expensive one was 2x more expensive. Now it's just 1.5x more expensive. So I wonder if applied to AI, that would mean that, look,  if GPUs are going to get more expensive,  there will be a fixed cost increase in the price of compute. As a result, that will push people to be willing to pay higher margins for slightly better models. Because the calculus is I'm going to be paying all this money for the compute anyways.

[(20:55)](https://podwise.ai/dashboard/episodes/7508210?locate=1255)
I might as well just pay slightly more to making sure it's like the very best model rather than a model that's slightly worse.

**Dylan Patel:**
[(21:01)](https://podwise.ai/dashboard/episodes/7508210?locate=1261)
Right. So the hopper went from two to three dollars. And if a hopper can make a million tokens of Opus and it can make two million tokens of Sonnet,  the price differential between Opus and Sonnet has decreased because the price of the GPU has increased by a dollar from two to three. Interesting. I think that makes a ton of sense. Also, I think we just see all of the volumes are on the best models today,  all the revenues on the best models today. And in a compute limited world, there's sort of two things that happen, right? A, companies that have locked up, you know, and don't have commitment issues, you know,  have these five-year contracts for compute.

[(21:41)](https://podwise.ai/dashboard/episodes/7508210?locate=1301)
They've kind of locked in a humongous margin advantage because they've locked in compute for five years at a price of what it transacted at five years ago or three years ago or two years ago,  whatever it is. Whereas if you're now three years into that five-year contract and someone else's two-year contract or three-year contract rolled off,  and now you're trying to buy that at modern pricing,  when you're priced to the value of models,  the price is going to be up a lot more. And so in a sense, the person who committed Early has better margins in general.

[(22:11)](https://podwise.ai/dashboard/episodes/7508210?locate=1331)
And the percentage of the market that is in long term contracts is much larger than the percentage of the market in short term contracts that can be this sort of flex capacity that you add at the last second. And at the same time, right, so where does the margin go, right? Because models get more valuable. How much can the cloud players flex their pricing? Well, if in fact, like, if you look at Corweave,  their average term duration is like over three years right now. And for like 90% plus of their compute, it's over three years. And so they end up with this like conundrum of like, well, they can't actually flex price.

[(22:45)](https://podwise.ai/dashboard/episodes/7508210?locate=1365)
But Every year they're adding incrementally way more capacity than they had previously, right? This year alone, right,  Meta's adding as much capacity as they had in the entire fleet of compute and data centers for all purposes for serving WhatsApp and Instagram and Facebook in 2022 and doing AI,  right? They're adding that alone this year. So in the same sense, you talk about Meta's doing that, CoreWeave and Google and Amazon,  all these companies are adding insane amounts of compute year on year on year. That new compute gets transacted at the new price. So in a sense, yes, you've locked in, as long as we're in a sort of a takeoff, right?

[(23:21)](https://podwise.ai/dashboard/episodes/7508210?locate=1401)
Oh, OpenAI went from 600 megawatts to 2 gigawatts last year, from 2 gigawatts to You know,  six plus this year and, you know, six to 12 next year, right? The incremental added compute is where all the cost is, not the prior long term contracts. So then who holds the card is the infra providers for charging margin, right? So now the cloud players, the neoclouds or the hyperscalers can charge the margin. Oh, they can't because or they can to some extent. But then as you go upstream to, oh, well, who has access to all the memory and logic capacity? Well, it's Nvidia for the most part. They've signed a lot of long-term contracts.

[(23:53)](https://podwise.ai/dashboard/episodes/7508210?locate=1433)
They've got like $90 billion of long-term contracts today and they're negotiating three-year deals with the memory vendors today. You've got obviously Amazon and Google through Broadcom and Amazon directly and all these companies, AMD. These companies hold all the cards because they've secured the capacity. And TSMC is not raising prices, but memory vendors are just like sort of,  to some extent, raising a lot of price, right? So they're going to double or triple price again. But then they're also signing these long term deals. So who is able to accrual the margin dollars is actually, you know, potentially the cloud,  potentially the chip vendors, and the memory vendors.

[(24:28)](https://podwise.ai/dashboard/episodes/7508210?locate=1468)
Until TSMC or ASML like break out and they like, no, actually, we're going to charge a lot more. But at the same time, do the model vendors get to charge crazy margins? I think at least this year, we're going to see margins for the model vendors go up a lot, right? Because they're so capacity constrained, they have to destroy demand, right? There's no way they can continue, Anthropic can continue at the current pace without destroying demand.

**Dwarkesh:**
[(24:51)](https://podwise.ai/dashboard/episodes/7508210?locate=1491)
Yeah, let's get into logic and memory. How specifically Nvidia has been able to lock up so much of both. So if you, I think, according to your numbers, by 27,  Nvidia is going to have like 70 plus percent of N3 wafer capacity or something like that,  or around that area. And then I forget what the numbers were for memory at SK Hynix and Samsung and so forth. But if you look at, so think about how the NeoCloud business works and how Nvidia works with that,  or how the RL environment business works and how Anthropic works with that. In both those cases, Nvidia is purposely trying to fracture the complementary industry to make sure that they have as much leverage possible.

[(25:34)](https://podwise.ai/dashboard/episodes/7508210?locate=1534)
So they're giving, you know, allocation to random NeoClouds to make sure that there's not one person that has all the compute. Similarly, Anthropic or OpenAI, when they're working with the data providers, they say, no,  we're going to just cede a huge industry of these things so that we're not locked into any one supplier for data environments. And I wonder why on the three nanometer process, that's going to be Tranium-3,  that's going to be TPU-V7, other accelerators potentially,  and why is TSMC just giving it all up to Nvidia rather than,  you know, trying to fracture the market?

**Dylan Patel:**
[(26:07)](https://podwise.ai/dashboard/episodes/7508210?locate=1567)
Yeah, so I think There's a couple points here, right? On 3 nanometer, if we go back to last year, the vast majority of 3 nanometer was Apple. Apple is being moved to 2 nanometer. Memory prices are going up, so Apple's volumes may go down because as memory prices go up,  either they cut margin or they move on. There's some time lag because they have long-term contracts, but basically,  Apple likely reduces demand slash moves to two nanometer faster where two nanometers only capable of a sort of mobile chips today. And in the future, AI chips will move there. So sort of Apple has that.

[(26:42)](https://podwise.ai/dashboard/episodes/7508210?locate=1602)
And then Apple is also talking to third party vendors because they're getting squeezed out of TSMC a little bit because TSMC's margins on high performance computing,  HPC, AI chips, et cetera, is higher than it is for mobile because they have a bigger advantage in HPC than they do in mobile. But anyways, when you look at what's TSMC running calculus here, actually,  they're providing really good allocations to companies that are doing CPUs,  right? So when you think about, hey, Amazon has Tranium and Amazon has Graviton, both of those are on three nanometer,  Graviton being their CPU, Tranium being their AI chip. They're actually,

[(27:20)](https://podwise.ai/dashboard/episodes/7508210?locate=1640)
 TSMC is much more excited to give allocation to Graviton than they are to Tranium because they view CPU business as more stable,  long term growth, right? And As a company that is conservative and doesn't want to ride cycles of growth too hard,  you actually want to allocate to the market that is more stable and lower growth rate first before you allocate all the incremental capacity to the fast growth rate market. That is the case generally. And so when you look at like, hey, same for AMD, right? The allocations they get on their CPUs is like,  TSMC is much more excited about those than they are for GPUs. Likewise for Amazon. And Nvidia is a bit unique because yes, they have CPUs.

[(28:04)](https://podwise.ai/dashboard/episodes/7508210?locate=1684)
Yes, they make switches. Yes, they make networking. They make NVLink. They make all these different, InfiniBand, Ethernet, all these different products, NICs. By and large,  most of these things will be on three nanometer by the end of this year with the Rubin launch and all the chips that are in that family,  the GPU being the most important one, and yet Nvidia is getting the majority of supply,  right? Part of this is because you look at the market and you like sort of like,  you know, TSMC and others like they, there are many ways that they forecast market demand. But also it's market signal, right? The market signaled, hey, we need this much capacity next year. We need this much. We need this much.

[(28:41)](https://podwise.ai/dashboard/episodes/7508210?locate=1721)
We'll sign non-cancelable, non-returnable. We may even pay deposits, right? Things like this. Nvidia just did it way earlier than Google or Amazon. And in some cases, Google and Amazon had stumbling blocks. One of the chips got delayed slightly by a couple quarters, Tranium and all these sorts of things happened. And so in that case, there was a huge sort of like, okay, well,  these guys are delaying, but Nvidia is wanting more, more, more, more, more. And we are checking with the rest of the supply chain, is there enough capacity, right? So they're going to all the PCV vendors and they're saying, hey, is there enough Victory Giant. Is there enough PCB?

[(29:16)](https://podwise.ai/dashboard/episodes/7508210?locate=1756)
This is like one of the largest suppliers of PCBs to Nvidia, and they're a Chinese company. All the PCBs come from China, sort of from them, or many of them. And anyways, they're like, do you have enough PCB capacity? Great. Oh, hey, memory vendors, who has all the memory capacity? Okay, Nvidia does. Great. So when you look at sort of in the same way, you know,  who is AGI-pilled enough to buy compute and long timelines at levels that seem ridiculous to people who aren't AGI-pilled,  but nonetheless, they're willing to pay a pretty good margin and sign it now because they view In the future,  that ratio is screwed up. The same thing happens with the supply chain for semiconductors, right?

[(29:53)](https://podwise.ai/dashboard/episodes/7508210?locate=1793)
Nvidia was, well, I don't think Nvidia is quite AGI-pilled, right? Jensen doesn't believe software is going to be automated fully and all these things, right?

**Dwarkesh:**
[(30:00)](https://podwise.ai/dashboard/episodes/7508210?locate=1800)
Accelerated computing, not AI chips, right?

**Dylan Patel:**
[(30:02)](https://podwise.ai/dashboard/episodes/7508210?locate=1802)
It's AI chips, right?

**Dwarkesh:**
[(30:03)](https://podwise.ai/dashboard/episodes/7508210?locate=1803)
But that's what he calls it, right?

**Dylan Patel:**
[(30:05)](https://podwise.ai/dashboard/episodes/7508210?locate=1805)
Yeah, because I mean, I think there's a broader term, right? AI is within that, but like,  Physics modeling and simulations and like already just like he's not embracing the sort of like main use case and I think he's embracing it. But like, I just don't think he's like AGI pilled like Dario, right? Or Sam, but he's still way, way more AGI pilled. Then, Google was at Q3 of last year,  or Amazon was at Q3 of last year,  and he saw way more demand, right? And the reason is pretty simple. You can see all the data center construction. He's like, okay, I want to have this market share. We have all the data centers tracked, and you can see There's a lot of data centers that you could say,

[(30:42)](https://podwise.ai/dashboard/episodes/7508210?locate=1842)
 well, they could be one or the other, right? And so to some extent, Google and Amazon, Google especially,  even though their TPU is just better for them to deploy,  they have to deploy a crap load of GPUs because they don't have enough TPUs to fill up their data centers. They can't get them fabbed.

**Dwarkesh:**
[(30:55)](https://podwise.ai/dashboard/episodes/7508210?locate=1855)
I have a question about that. Google sold, I think a million, was it the V7s, the Ironwoods to Entropiq. And you're saying in general, there's this big bottleneck right now, this year, next year,  I mean, I guess going forward forever now, is going to be the logic memory,  the stuff that it takes to build these chips. And Google has DeepMind. This is the other third prominent AI lab. And if this is the big bottleneck, why would they sell it rather than just giving it to DeepMind?

**Dylan Patel:**
[(31:23)](https://podwise.ai/dashboard/episodes/7508210?locate=1883)
Right. So this is, again, like a problem of like, DeepMind people were like, this is insane. Why did we do this? Then Google Cloud people and Google executives saw a different thought process. Basically, you and I know the compute team. Both of them actually came from Google. The main people on the compute team at Tropic, they saw this dislocation. They negotiated a deal and they were able to get access to this compute. Before Google realized and so the actually the chain of events at least from our data that we found was in in early Q3,  we saw over the course of two over the course of like six weeks,  we we saw capacity on anthropic or sorry on TPUs go up by a significant amount.

[(32:09)](https://podwise.ai/dashboard/episodes/7508210?locate=1929)
Over the course of those six weeks, and it went up like multiple times in those six weeks, right? There were multiple requests. Google even had to go to TSMC and explain to them why they needed this increase in capacity because it was so sudden. But a lot of that capacity increase was for selling to Anthropic because Anthropic saw it before Google. And then Google had Nano, Banana and Gemini 3,  which caused their user metrics to skyrocket and leadership at Google was like,  oh, and then they started making the statement of we have to double compute every,  is it six months? Or I don't remember the exact number that they said,  but they really Woke up a lot more and then they're like,

[(32:42)](https://podwise.ai/dashboard/episodes/7508210?locate=1962)
 oh, hey, TSMC, we want more. We want more. And it's like, well, sorry, guys, like we're sold out for next year. We can work on next year. We can maybe get like five, 10% more for 26. But really, we're going to work on 27. Right. It's sort of like, you know, there's this like information asymmetry of the labs in my mind. Right. I don't know if this is exactly the narrative I've spun myself from seeing all the data in the supply chain on like wafer orders and like What's going on with the data centers that,  you know, Anthropic signed and FluidStack signed and all this, like sort of,  it's pretty clear to me that Google screwed up. And you can see this from Google's Gemini ARRs, right?

[(33:15)](https://podwise.ai/dashboard/episodes/7508210?locate=1995)
They had next to nothing in Q1 to Q3, Q3 a little bit, right? Once they started inflecting, but Q4, they were at like 5 billion ARR, right? Exiting or something like this. So it's like, or 5 billion revenue for Q4 on an ARR basis. And so it's clearly like Google didn't see revenue skyrocket. And in a sense, right, Anthropic was not willing, you know,  it's kind of had like a little bit of commitment issues before their ARR exploded,  even though they have far more information asymmetry and see what's coming down the pipe. Google is going to be more conservative than Anthropic is, A. And B, Google had had even less ARR. So they sort of were like, I think, just not willing to like sort of do it.

[(33:56)](https://podwise.ai/dashboard/episodes/7508210?locate=2036)
And then they realized they should do it. And so now since then, Google has gotten absurdly AGI-pilled, right, in terms of what they're doing. They bought an energy company. They're putting deposits down for turbines. They're buying a ridiculous percentage of the powered land. They're going to utilities and negotiating long-term agreements. They're doing this on the data center and power side very, very aggressively, right? So, you know, I think Google woke up towards the end of last year, but it took them some time.

**Dwarkesh:**
[(34:26)](https://podwise.ai/dashboard/episodes/7508210?locate=2066)
And how many gigawatts do you think Google will have by the end of next year?

**Dylan Patel:**
[(34:28)](https://podwise.ai/dashboard/episodes/7508210?locate=2068)
Buy my data.

**Dwarkesh:**
[(34:31)](https://podwise.ai/dashboard/episodes/7508210?locate=2071)
You charge for that kind of information.

**Unknown Speaker:**
[(34:32)](https://podwise.ai/dashboard/episodes/7508210?locate=2072)
Yes, yes.

**Dwarkesh:**
[(34:33)](https://podwise.ai/dashboard/episodes/7508210?locate=2073)
I feel like every year, the bottleneck for what is preventing us from scaling AI compute keeps changing. A couple of years ago, it was CoOS. Last year, it was Power. This year, you'll tell me what the bottleneck is this year. But I want to understand five years out,  what will be the thing that is constraining us from Deploying the singularity.

**Dylan Patel:**
[(34:51)](https://podwise.ai/dashboard/episodes/7508210?locate=2091)
Yeah,  I think the biggest bottleneck is compute and for that the longest lead time supply chains are not power or data centers. They're actually The semiconductor supply chain themselves, right,  switches back from being power and data center as a major bottleneck to chips. And in the chip supply chain, there's a number of different bottlenecks, right? There's memory, there's logic wafers from TSMC, there's fabs themselves. Construction of the fabs takes a couple years, two to three years,  versus a data center takes Less than a year,  right? We've seen Amazon build data centers in as fast as eight months, right? So there's a big difference in lead times because of the complexity of the building,

[(35:31)](https://podwise.ai/dashboard/episodes/7508210?locate=2131)
 the fab that actually makes the chips, and then the tools, right? Those also have really long lead times. And so the bottlenecks, as we've scaled, have shifted from, hey, what is the supply chain currently not,  what is it currently not able to do,  which was COAS and Power and data centers,  but those were all shorter lead time items, right? Co-auth is a much more simple process of packaging chips together. Power and data centers are ultimately way more simple than the actual manufacturing of the chips. And so there's been some sliding of capacity across mobile or PC to data center chips,

[(36:08)](https://podwise.ai/dashboard/episodes/7508210?locate=2168)
 but that's been somewhat fungible, whereas Whereas COAS and power and data centers have sort of had to start anew as supply chains,  but now there's sort of no more capacity for the mobile and PC industries,  which used to be the majority of the semiconductor industry, to shift over to AI,  right? Nvidia is now the largest customer at TSMC,  and Nvidia is the largest customer at SK Hynix,  the largest memory manufacturer, right? So it's sort of It's impossible for the scaling or the sliding of resources away from the common person,  PCs and smartphones to shift anymore towards the AI chips. And so now, how do we scale the AI chip production?

[(36:47)](https://podwise.ai/dashboard/episodes/7508210?locate=2207)
And that's the biggest bottleneck As we go to 2030 is those.

**Dwarkesh:**
[(36:52)](https://podwise.ai/dashboard/episodes/7508210?locate=2212)
It'd be very interesting if there is an absolute gigawatt ceiling that you can project out to 2030 based just on,  hey, we can't produce more than this many EUV machines.

**Dylan Patel:**
[(37:03)](https://podwise.ai/dashboard/episodes/7508210?locate=2223)
Right. So to scale compute further, right, there's some different bottlenecks this year, next year,  but ultimately by 28, 29, the bottleneck falls to the lowest rung on the supply chain,  which is ASML. ASML makes the world's most complicated machine, i.e. an EUV tool, and the selling price for those is $300, $400 million. Currently, they can make about 70. Next year, they'll get to 80. Even under very aggressive supply chain expansion,  they only get to a little bit over 100 by the end of the decade. What does that mean? Okay, they can make 100 of these tools by the end of the decade and 70 right now. How does that actually translate to AI compute, right?

[(37:43)](https://podwise.ai/dashboard/episodes/7508210?locate=2263)
We see all these numbers from Sam Altman and many others across the supply chain, gigawatts, gigawatts, gigawatts, right? How many gigawatts are we adding? And we see Elon saying, hey, 100 gigawatts in space.

**Dwarkesh:**
[(37:55)](https://podwise.ai/dashboard/episodes/7508210?locate=2275)
A year.

**Dylan Patel:**
[(37:56)](https://podwise.ai/dashboard/episodes/7508210?locate=2276)
A year, right. The problem with any of these numbers or the challenge to these numbers is actually not the power,  not the data center. We can dive into that, but it's manufacturing the chips, right? So a gigawatt of Nvidia's Rubin Chips, right? So Rubin is announced at GTC. I believe the week this podcast goes live and to make a gigawatt worth of data center capacity of Nvidia's latest chip that they're releasing at the end of this year,  towards the end of this year, you need, you know, a few different wafer technologies,  right? You need About 55,000 wafers of three nanometer, you need about 6,000 wafers of five nanometer,  and then you need about 170,000 wafers of DRAM, right, memory.

[(38:40)](https://podwise.ai/dashboard/episodes/7508210?locate=2320)
And so across these three different buckets. Each of these requires different amounts of EUV, right? So when you manufacture a wafer, there's thousands and thousands of process steps where you're depositing material, removing them. But the sort of key critical step, which at least in advanced logic is like 30% of the cost of the chip,  is Something that doesn't actually put anything on the wafer, right? You take the wafer, you deposit photoresist, which is like a chemical that basically chemically changes when you expose it to light. And then you stick it into the EV tool, which shines light at it in a certain way. It patterns it, right?

[(39:12)](https://podwise.ai/dashboard/episodes/7508210?locate=2352)
Because there's what's called a mask, which is a stencil effectively for the design. And so when you look at a wafer, you know, leading edge three nanometer wafer has 70 or so masks, right? 70 or so layers of lithography, but 20 of them are the most advanced EUV, right? And that specifically If you think about, okay, well, if I need 55,000 wafers, For a gigawatt,  if I do 20 EUV passes per wafer, you then can do the math that's like,  okay, that's 1.1 million passes of EUV for a single gigawatt. So actually like it's pretty simple. And then once you add the rest of the stuff,  it ends up being 2 million right across five nanometer and all the memory.

[(39:49)](https://podwise.ai/dashboard/episodes/7508210?locate=2389)
You're at roughly 2 million EUV passes for a single gigawatt. These tools are very complicated. So when you think about what it's doing across a wafer,  it's taking the wafer and it's scanning And it's stepping across or it's getting stepping across and it does this. Hundreds of times across the entire, or dozens of times across the whole wafer. And so when you're talking about, hey, how many EUV passes,  that's the entire wafer is being exposed at a certain rate. A wafer, a EUV tool can do roughly 75 wafers per hour. And the tool is up roughly 90% of the time, right? So in the end, you end up with, actually,

[(40:24)](https://podwise.ai/dashboard/episodes/7508210?locate=2424)
 I need about three and a half EUV tools to do the 2 million EUV wafer passes for the gigawatt. So three and a half EUV tools satisfies a gigawatt. So it's funny to think about the numbers, right? Because we're talking about, oh, what's the gigawatt cost? It costs like $50 billion roughly, right? Whereas what does three and a half EUV tools cost? That's like 1.2, right? It's actually like quite a lower number. Which is interesting to think about like, oh, 50 gigawatts of economic, you know, sort of CapEx in the data center. And what gets built on top of that in terms of tokens is even larger, right?

[(40:56)](https://podwise.ai/dashboard/episodes/7508210?locate=2456)
It might be $100 billion worth of AI value into the supply chain is held up by this $1.2 billion worth of tooling that simply just cannot expand its supply chain quickly.

**Dwarkesh:**
[(41:07)](https://podwise.ai/dashboard/episodes/7508210?locate=2467)
In fact, it goes, even the intermediate layers, We are sort of shocking here. So, Carl Zeiss, which is like the optics supplier that is bottlenecking ASML itself,  I checked its market cap this morning. You know what it is? $2.5 billion.

**Dylan Patel:**
[(41:22)](https://podwise.ai/dashboard/episodes/7508210?locate=2482)
Dude, let's LBO that. Let's LBO it.

**Dwarkesh:**
[(41:25)](https://podwise.ai/dashboard/episodes/7508210?locate=2485)
And I think, so you read this article recently where you were saying over the last three years,  TSMC has done $100 billion of CapEx. It's like 30, 30, 40. And if you think about, I mean,  a small fraction of that is sort of like being used by Nvidia for the three nanometer that it's going to or,  you know, previously for an animator that that's using for his chips. But Nvidia has turned that into what was what are it's like? Your earnings last quarter was like $40 billion, and so $40 billion times four, so $160 billion. So Nvidia alone is turning some small fraction of $100 billion in CapEx that's going to be depreciated over many years,  not just this one year, into $160 billion in a single year.

[(42:07)](https://podwise.ai/dashboard/episodes/7508210?locate=2527)
And then that gets even more intense when you go down the supply chain to ASML,  which is taking a billion dollars worth of machines to produce a gigawatt. And then, of course, those machines last for more than a year, right? So it's doing more than that. Okay, so now I want to understand, okay, well,  how many such machines will there be by 2030,  if you include not just the ones that are sold that year,  but have been compiling over the previous years? And what does that imply about the... Sam Altman says he wants to do a gigawatt a week in 2030. When you add up those numbers, is that compatible with that?

**Dylan Patel:**
[(42:35)](https://podwise.ai/dashboard/episodes/7508210?locate=2555)
Right. That's completely compatible, right? Because if you think about TSMC and the entire ecosystem has something 250 to 300 EUV tools already,  and then you stack on 70 this year, 80 next year, growing to 100 by 2030,  you're at like 700 EUV tools by the end of the decade. 700 EUV tools, three and a half tools per gigawatt, Assuming it's all allocated to AI,  which it's not,  but three and a half tools per gigawatt gets you to 200 gigawatts worth of AI chips for the data centers to deploy,  right? So 200 gigawatts, Sam wants 50 gigawatts or 52 gigawatts a year. He's only taking 25% share then, right? Obviously, there's some share given to mobile and PC, assuming that You know, for some reason,

[(43:18)](https://podwise.ai/dashboard/episodes/7508210?locate=2598)
 we're allowed to even have consumer goods still, you know,  and we don't get priced out of them. But, you know, roughly like he's saying, 25 percent, 50 percent, you know, 25 percent market share of the total chips fab. That's that's kind of like very reasonable, given, you know, this year alone,  I think he's going to have access to 25 percent of the Blackwell GPUs that are deployed. Right. So it's not that crazy.

**Dwarkesh:**
[(43:39)](https://podwise.ai/dashboard/episodes/7508210?locate=2619)
I find it surprising that, you know, when was the first, uh, when did ASML start shipping UV tools? When the seven nanometer started. So I don't know when that was exactly, but you're saying in 2030,  they're going to be using machines that initially were shipped in 2020. So 10 years you're using the same most important machine in this most technologically advanced industry in the world. I find that surprising.

**Dylan Patel:**
[(44:01)](https://podwise.ai/dashboard/episodes/7508210?locate=2641)
So ASML has been shipping UV tools now for roughly a decade, but it only entered mass volume production around 2020. The tool's not the same. Back then, the tools were even lower throughput. There's various specifications around them called overlay. I was mentioning you're stacking layers on top of each other. You'll do some EUV. You'll do a bunch of different process steps, depositing stuff, etching stuff, cleaning the wafer,  dozens of those steps before you do another EUV layer. There's a spec called overlay, which is, okay, you did all this work. You drew these lines on the wafer. Now I want to draw these dots, right?

[(44:36)](https://podwise.ai/dashboard/episodes/7508210?locate=2676)
Let's just say I want to draw these dots to connect this, these lines of metal to and then,  you know, holes. And then the next layer up is another set of lines that goes perpendicular. So now you're connecting wires going. Perpendicular to each other, you have to be able to land them on top of each other. So it's called overlay. And overlay is a spec that's been improved rapidly by ASML. Wafer throughput has been improved rapidly by ASML. And also the price of the tool has gone up, but not as much as the capabilities of the tool. Initially, the EUV tools were like $150 million. And over time, they're now like $400 million. You know, as I as I look out to 2028,

[(45:09)](https://podwise.ai/dashboard/episodes/7508210?locate=2709)
 but the capabilities of the tools have more than doubled as well,  right, especially on throughput and overlay accuracy, which is the ability to stack, you know,  accurately align the the subsequent passes on top of each other,  even though you do tons of steps between. And so this is this is. ASML is improving super rapidly. I think it's also something noteworthy to say ASML is maybe one of the most generous companies in the world. They have this linchpin thing. No one has anything competitive. Maybe China will have some EUV by the end of the decade,  but no one else has anything even close to EUV and yet they haven't taken price and margins up like crazy.

[(45:50)](https://podwise.ai/dashboard/episodes/7508210?locate=2750)
You go ask You know, some other folks, you know, that we talk to all the time,  like, you know, for example, Leopold, they're like, well, you know, let's let's, you know,  let's let's have the price go up, right? Because they can. The margin is there. You can you can take the margin like Nvidia takes the margin. Memory players are taking the margin. But ASML has never risen the price more than they've increased the capability of the tool. And so in a sense, they've always provided net benefit to their customer. It's not that the tool is stagnant. It's just that like, you know, these tools are old. Yes, you can upgrade them some and the new tools are coming.

[(46:20)](https://podwise.ai/dashboard/episodes/7508210?locate=2780)
And for simplicity's sake, we're kind of ignoring, you know, the advances for this podcast,  the advances in overlay or throughput per tool.

**Dwarkesh:**
[(46:26)](https://podwise.ai/dashboard/episodes/7508210?locate=2786)
So you say we're producing 60 of these machines this year and then 70, 80 over subsequent years. What would happen if ASML just decided to double its CapEx or triple its CapEx? What is preventing them from producing more than 100 in 2030?  Why so confident that even five years out you can be relatively sure what their production will be?

**Dylan Patel:**
[(46:48)](https://podwise.ai/dashboard/episodes/7508210?locate=2808)
So I think a couple of factors here, right? ASML has not decided to just go YOLO, let's expand capacity as fast as possible, right? In general, the semiconductor supply chain has not, right? It's lived through the booms and busts and we can talk a bit more about it,  but basically no one you know, some players as of very recently have like woken up,  but in general no one really sees demand for 200 gigawatts a year of AI chips or,  you know, trillions of dollars of spend a year in the semiconductor supply chain. They're just like, they're not AI-pilled, right? They're not AGI-pilled.

**Dwarkesh:**
[(47:21)](https://podwise.ai/dashboard/episodes/7508210?locate=2841)
We're going to get to a trillion dollars this year.

**Dylan Patel:**
[(47:24)](https://podwise.ai/dashboard/episodes/7508210?locate=2844)
Yeah, I feel you, but I'm saying like no one really understands this in the supply chain. Constantly we're told our numbers are way too high and then when they're right,  they're like, oh yeah, but your next year's numbers are still too high. And it's like, but anyways, like ASML, Their tool has four major components. It has the source, which is made by CYMER in San Diego. It has the reticle stage, which is made in Wilmington, Connecticut. It has the wafer stage. And the optics, right, the lenses and such, and those two are made in Europe, right? And so when you look at each of these four, they're tremendously complex supply chains that A,

[(48:05)](https://podwise.ai/dashboard/episodes/7508210?locate=2885)
 they have not tried to expand massively, and B, when they try to expand them,  the time lag is quite long, right? And so again, this is the most complicated machine that humans make, period, right,  at a volume, At any sort of volume, but let's talk about the source specifically,  right? What does the source do? It drops these tin droplets. It hits it three subsequent times with a laser perfectly. So the first one hits this tin droplet, expands out, it hits it again,  so it expands out to this perfect shape. And then it blasted at super high power. And the tin droplets get excited enough that they release EUV light, 13.5 nanometer.

[(48:43)](https://podwise.ai/dashboard/episodes/7508210?locate=2923)
And then it's in this thing that is like basically collecting all the light and directing it into the lens stack,  right? Then you have the Lendstack, which is Carl Zeiss, right, as you mentioned, and some other folks,  but Zeiss being the most important part of it. They also have not tried to expand production capacity because they don't see any,  you know, they're like, Oh, yeah, like, we're growing a lot because of AI. We're going from 60 to 100. Right? It's like, no, no, no, no, no, we need to go to like, a couple hundred, but it's fine, whatever. Each of these tools has, you know, I think 18 of these lenses, effectively, mirrors,

[(49:14)](https://podwise.ai/dashboard/episodes/7508210?locate=2954)
 they are, they're multi layer mirrors, which are perfect layers of molybdenum, And Ruthenium,  if I recall correctly, stacked on top of each other in many layers and then the light bounces off of it perfectly. But it's not just like, you know, like when we think about a lens,  you know, it's like in a shape and it focuses the light. This is like a mirror that's also a lens. And so it's pretty complicated. Any defect in this perfect layer of stat in these like super thinly deposited stacks will mess it up. Any curvature issues, like there is a lot of challenges with scaling the production. It's quite artisanal, right, in the sense, right,  because you're not making tens of thousands of these a year,

[(49:51)](https://podwise.ai/dashboard/episodes/7508210?locate=2991)
 you're making hundreds, you're making thousands, right, you know, talk about 60 tools a year,  18 of these per tool, you end up with, you know, you're still in the,  you know, hundreds of tools, or thousand, you're at the thousand number roughly for these,  these lenses, And projection optics. So then you step forward to the reticle stage, which is also something really crazy. This thing moves at, I want to say, 9Gs. Like it will shift 9Gs because as you step across a wafer, the tool will go. And the wafer stage is complementary. It's the wafer part. So you line these two things up. You're taking all the light through the lenses that's focused.

[(50:31)](https://podwise.ai/dashboard/episodes/7508210?locate=3031)
And here's the reticle, here's the wafer, and you're passing, the reticle's moving one direction,  the wafer's moving the other direction, as it scans a 26 by 33 millimeter section of the wafer,  and then it stops. It shifts over to another part of the wafer and does it again. And it does that in just seconds, right? And each of them are moving at 9Gs in opposite directions. So each of these things is like a wonder and marvel of like chemistry,  fabrication, you know, sort of like mechanical engineering, optical engineering,  because you have to align all these things and make sure they're perfect.

[(51:08)](https://podwise.ai/dashboard/episodes/7508210?locate=3068)
All these things have crazy amounts of metrology because you have to perfectly test everything because if anything is messed up,  The yield goes to zero, right? Because this is such a finely tuned system. And by the way, it's so large that you're building it in all these,  you're building in the factory in Hindhoven, Netherlands,  and they're deconstructing it and shipping it on many planes to the customer site. And then you're reassembling it there and testing it again. And that process takes many, many months. So like, it's just, there's so many steps in the supply chain, right?

[(51:36)](https://podwise.ai/dashboard/episodes/7508210?locate=3096)
Whether it's Zeiss making their lenses and projection optics, Or CYMR, which is an ASML-owned company, making the EUV source. And each of these has its own complex supply chain, right? ASML's commented their supply chain has over 10,000 people in it, right?

**Dwarkesh:**
[(51:50)](https://podwise.ai/dashboard/episodes/7508210?locate=3110)
Like individual suppliers.

**Dylan Patel:**
[(51:51)](https://podwise.ai/dashboard/episodes/7508210?locate=3111)
Yes. And it might not be directly, it might be through like, hey, you know,  ZEISS has so many suppliers and, you know, XYZ company has so many suppliers,  but, you know, these, you know, If you think about like, okay,  you're talking about two physically moving objects that are like this large and this large,  you know, the size of a wafer, right? And it has to be accurate to the level of You know, single digit nanometers or even smaller,  because the entire system, the overlay, right? Layer to layer variation has to be on the order of three nanometers, right? And so if the overlay is three nanometers, that means each individual part,

[(52:26)](https://podwise.ai/dashboard/episodes/7508210?locate=3146)
 the accuracy of its physical movement has to be even less than that,  right? Has to be sub one nanometer in most cases, because the error of these things stacks up, right? And so there's no way to like, You know, just like snap your fingers and increase production, right? You know, things simple as power, right? The US going from 0% power growth to 2% power growth, even though China's already at 30,  was like so hard for America to do, right? And that's a really simple supply chain with very few people in the supply chain, right, who make difficult things. And there's You know, probably what, 100,000 electricians slash people who work in the supply chain of electricity or more in the US.

[(53:08)](https://podwise.ai/dashboard/episodes/7508210?locate=3188)
And, you know, when you look at, oh, ASML employs like so few people. Carl Zeiss probably employs like less than a thousand people working on this. And all of those people are like super, super specialized. So, you know, you can't just train random people up for this, like in the snap of a finger. You can't just get your entire supply chain to get galvanized right. Nvidia's had to do a lot To get the entire supply chain to even deliver the capacity they're going to make this year,  even though when you go talk to Anthropic, they're like, well, we're short of TPUs,  we're short of Tranium, we're short of GPUs. When you go talk to OpenAI, they're like, we're short of these things, right?

[(53:41)](https://podwise.ai/dashboard/episodes/7508210?locate=3221)
So OpenAI and Anthropic, they know they need X. Nvidia is not quite as AGI-pilled and they're building, you know, X minus one. And you go down the supply chain, everyone's doing minus one. And in some cases, they're doing like divided by two, right? Because they just don't, they're not AGI-pilled, right? I think. And so you end up with The time lag for this whip to react,  the AI-pilledness and desire to increase production is so long. Then once they finally understand, hey, we need to increase production rapidly, and they think they understand,  oh, AI means we have to go from 60 to 100. In addition to the tools all just getting better and faster,

[(54:21)](https://podwise.ai/dashboard/episodes/7508210?locate=3261)
 the source getting higher power from 500 watts to 1,000 and all these other aspects of the supply chain,  advancing technically plus increase in production, they think they're actually increasing production a lot. But if you float through the numbers of, hey, what does Elon want? He wants 100 gigawatts a year in space by 2028, is it? Or 2029. And, you know, Sam Altman wants 50 gigawatt, 52 gigawatts a year by the end of the decade. And you look at, you know, probably Anthropic needs the same. And then, you know, Google needs that. You know, you go across the supply chain.

[(54:52)](https://podwise.ai/dashboard/episodes/7508210?locate=3292)
It's like, wait, no, the supply chain can't possibly build enough capacity for everyone to get what they want on the side of compute.

**Dwarkesh:**
[(55:00)](https://podwise.ai/dashboard/episodes/7508210?locate=3300)
Real conversations are full of fits and starts and pauses and interruptions. I mean, just listen to this episode. At least superficially, voice models have gotten pretty good at handling these kinds of things. But at a deeper level, interruptions can throw off a model's understanding and degrade the quality of its responses. And it's not always clear why. LimoBox realized that this was a huge bottleneck for their customers. So they built an evaluation pipeline called EchoChain to help you diagnose and fix your voice model's specific failure modes. EchoChain starts by feeding conversations into your voice model.

[(55:28)](https://podwise.ai/dashboard/episodes/7508210?locate=3328)
It then injects interruptions at specific intervals and classifies any failures into one of three different modes. One, did it acknowledge a correction to keep the old plan? Two, did it adapt briefly but then slide back to old assumptions? Or three, did it abandon the old task entirely? This is extremely useful information because LabelBox can get your model the exact data it needs to fix whatever issue is preventing it from being a viable and competent voice model. So, if you want to ensure that your voice model states performance in real conversations,  you should reach out to Labelbox. Go to labelbox.com slash Dwarkesh. So, I feel like in the data center supply chain for the last few years,

[(56:09)](https://podwise.ai/dashboard/episodes/7508210?locate=3369)
 people have been making arguments of, This specific thing we are bottlenecked by. Therefore, AI compute can't scale more than X. But then as you've written about, oh, no, if, you know, say the grid is a bottleneck,  then we just do behind the meter on the site. We do gas turbines, etc. If that doesn't work, there's like all these other alternatives that people fall back on. And I want to ask you a question about whether we can imagine a similar thing happening We're in the semiconductor supply chain. So if EUV becomes a bottleneck,  what if we just went back to 7 nanometer and do what China is doing currently in producing 7 nanometer ships with multi-patterning with DUV machines?

[(56:49)](https://podwise.ai/dashboard/episodes/7508210?locate=3409)
And if you look at a 7 nanometer ship like the A100, there's been a lot of progress,  obviously, from the A100 to the B100 or B200. How much of that progress is just numerics? And then if you just hold constant, say, FP16 from A100 to B100,  the B100 is a little over one petaflop,  and then A100 is 300 teraflops. And so you have like basically 3X holding numerics constant. You have like a 3X improvement from A100 to B100. And then some of that is the process improvement. Some of that is just the accelerator design improving, which we could replicate again in the future.

[(57:32)](https://podwise.ai/dashboard/episodes/7508210?locate=3452)
And so then it just seems like actually it's like very small effect from the process improving from seven nanometer to four nanometer. So I don't know, say we have a I don't know the numbers offhand,  but let's say there's like 150k wafers per month of 3nm and then eventually similar amounts for 2nm. But then there's a similar amount for 7nm, right? So if you have all those old wafers and then there's maybe a 50% haircut because the process,  you know, the bits per wafer area are like What is it, 50% less or something? Then it's like, it doesn't seem like that bad to just bring on seven nanometer wafers and then,  oh, that gives you another 50 or another 100 gigawatts.

[(58:12)](https://podwise.ai/dashboard/episodes/7508210?locate=3492)
Yeah, tell me why that's naive.

**Dylan Patel:**
[(58:13)](https://podwise.ai/dashboard/episodes/7508210?locate=3493)
Yeah, so I think, you know,  we potentially do go crazy enough that this happens because we just need incremental compute and the compute is worth the higher cost,  power, et cetera, of these chips. But it's also unlikely to some extent, to a large extent, because of, I think,  just comparing, you know, some of these are like not fair comparisons, right? For example, you know, from A100, which is 312 teraflops to Blackwell, which is like 1,000-ish of FP16,  or maybe it's 2,000 and then Rubin is like 5,000 or so FP16.  It's not a fair comparison because these chips have vastly different You know,  design targets, right? At A100, that is what Nvidia optimized for was FP16, BF16 numerics.

[(59:04)](https://podwise.ai/dashboard/episodes/7508210?locate=3544)
When you look at Hopper, they didn't care as much about that. They cared about FP8. When you look at Rubin, they don't care about FP16 and BF16 as much. They care mostly about FP4 and 6, right? And so numerics are what they've designed their chip for. And so there's a couple like, you know, okay, let's just say, let's redesign,  let's make a new chip design on seven nanometers. Sure, we can do that. And then it's optimized for the numerics of the modern day. The performance difference is still going to be much larger than the flops difference you mentioned, right? Often it's easy to boil things down to flops per watt or flops per dollar. But that's actually not a fair comparison.

[(59:47)](https://podwise.ai/dashboard/episodes/7508210?locate=3587)
And so this is where you can bring in, hey, let's look at Kimi K1 or DeepSeek. When you look at Kimi K2.5 and DeepSeek,  when you look at these two models and you look at their performance on Hopper versus Blackwell on very optimized software,  you get vastly different performance. And Most of this is not attributed to flops or numerics, right? Because those models are actually 8-bit. So it's not like Blackwell's and Hopper, they're both optimized for 8-bit and Blackwell's not really taking advantage of its 4-bit there. The performance gulf is actually much larger. And the way you can sort of compare them and think about them is,

[(1:00:28)](https://podwise.ai/dashboard/episodes/7508210?locate=3628)
 sure, it's one thing to shrink process technology and make the transistor smaller and each chip has X number of flops. But you forget the big gating factors. These models don't run on a single chip. They run on hundreds of chips at a time, right? If you look at DeepSeek's production deployment, which is well over a year old now,  they were running on 160 GPUs, right? And that's what they serve production traffic on. And so they split the model across 160 GPUs. Every time you cross the barrier of a chip to another chip,  there is an efficiency loss because you now have to transmit over,  you know, high speed electrical sturdies, and there is a latency cost, there's a power cost,

[(1:01:03)](https://podwise.ai/dashboard/episodes/7508210?locate=3663)
 there's all these dynamics that hurt. As you shrink and shrink and shrink the process node, you've Increase the amount of compute in a single chip. Now, in chip, movement of data is at least tens of terabytes a second,  if not hundreds of terabytes a second. Whereas between chips, you're on the order of a terabytes of second. This movement of data between chips that are super close to each other physically,  and then you can only put so many chips close to each other physically,  so you have to put chips in different racks. The order of data between that is on the order of hundreds of gigabits a second, right? 400 gig or 800 gig a second. So 100 gigabytes a second, roughly.

[(1:01:46)](https://podwise.ai/dashboard/episodes/7508210?locate=3706)
And so you've got this like huge ladder of like, oh, on chip, I can communicate at super fast speeds. Within the rack, I can communicate at order of magnitude speeds. Outside the rack I can communicate at an even order of magnitude lower than that. And as you break the bounds of chips, you end up with this performance loss. So anyways, the reason I explain this is because when you look at Hopper versus Blackwell,  even if both of them are using a rack worth of chips,  the Hopper is significantly slower because the amount of performance that you have Leverage to the task within that,

[(1:02:16)](https://podwise.ai/dashboard/episodes/7508210?locate=3736)
 you know, within each domain of, hey, tens of terabytes of seconds of communication between these transistors or these processing elements. And, you know, terabytes a second between these processing elements is much, much higher,  and therefore the performance is much higher. So when you look at inference at, let's say, 100 tokens a second for DeepSeek and KimiK 2.5,  Hopper versus Blackwell, the performance difference is on the order of 20x.

**Dwarkesh:**
[(1:02:40)](https://podwise.ai/dashboard/episodes/7508210?locate=3760)
Interesting.

**Dylan Patel:**
[(1:02:40)](https://podwise.ai/dashboard/episodes/7508210?locate=3760)
Not two or three x like the flops Performance difference indicates,  even though those are on the same process node,  there's just differences in networking technologies and what they've worked on. And so you can translate some of these back. But when you look at like Rubin, what they're doing on three nanometers,  some of these things are just not possible to do all the way back on A100,  even if you make a new chip for seven nanometer. There's just like certain architectural improvements you can port. There's certain ones you cannot. And so the performance difference is not just going to be the difference in flops. It's in some senses, cumulative between the difference in, you know, flops per chip,

[(1:03:14)](https://podwise.ai/dashboard/episodes/7508210?locate=3794)
 networking speed between chips, how many flops are on a chip versus a system,  memory bandwidth on a single chip and on an entire system. All of these things compound.

**Dwarkesh:**
[(1:03:22)](https://podwise.ai/dashboard/episodes/7508210?locate=3802)
Can I ask you a very naive question? So this year, last year, the B200 has now two dies on a single chip. So you can get that bandwidth on a single chip without having to go through ME-Link or InfiniBand. And then next year, Rubin Ultra will have four dies on one chip. What is preventing us from just doing that with How many dyes could you have a single chip and still get these tens of terabytes a second?

**Dylan Patel:**
[(1:03:46)](https://podwise.ai/dashboard/episodes/7508210?locate=3826)
Yeah, so even within Blackwell, there are differences in performance when you're communicating on the chip versus across the chips. Those bounds are obviously much smaller than when you're going out of the entire chip,  but each die versus within the package. And so anyways, when you scale the number of chips up, there is some performance loss. It's not just perfect, but it is way better than different entire packages. Now, how large can advanced packaging scale? The way Nvidia is doing it is co-auth the way Google and with Broadcom and MediaTek and Amazon,  Tranium, all these chips are doing is called co-auth. But actually you can go and look back at what Tesla did with Dojo.

[(1:04:31)](https://podwise.ai/dashboard/episodes/7508210?locate=3871)
Dojo, which they canceled and restarted. Anyways, Dojo was a chip that was the size of an entire wafer. They had 25 chips on it. And there were some trade-offs, right? They couldn't put HBM on it. But the positive side of it was that they had 25 chips on it. And so to date, it is still probably the best chip for running convolutional neural networks. It's just not great at transformers because the, you know,  the sort of the shape of the chip,  the memory, the arithmetic, all these various specifications of it are just not well suited for transformers. They're well suited for CNNs. And anyway, so, you know, dojo chips were optimized around that.

[(1:05:10)](https://podwise.ai/dashboard/episodes/7508210?locate=3910)
They made a bigger package, but at the same time, you know,  as you make packages bigger and bigger and bigger,  you have other constraints, right? Networking speed, memory bandwidth, cooling capabilities, all of these things start to rear their heads. It's not simple, but yes, you will see a trend line of more chips on the package. And yes, you're going to be able to do that on 7nm. In fact, that's what Huawei did with their Ascend 910C or D. They put They were initially just one and then they did two. And they're focusing on scaling the packaging up because that is an area where they can advance faster than sort of process technology where they can't shrink.

[(1:05:47)](https://podwise.ai/dashboard/episodes/7508210?locate=3947)
But at the end of the day, that's still, you know,  that's something that you can do on the leading edge chips too,  right? Anything you do on seven nanometer, you can also probably do on three nanometer in terms of packaging.

**Dwarkesh:**
[(1:05:55)](https://podwise.ai/dashboard/episodes/7508210?locate=3955)
So if we end up in this world in 2030,  where the West has the most advanced process technology,  but it has not ramped it up as much, whereas China, I don't know if you think by 2030,  they would have EUV and, I don't know, 2 nanometer or whatever, but they are a semiconductor pill,  so they're producing in mass quantity. Basically, I'm wondering what the year is where there's a crossover,  where our advantage in process technology has faded enough and their advantage in scale has increased enough. And also their advantage in having one country that has the entire supply chain indigenized rather than having random suppliers in Germany and Netherlands and whatever,

[(1:06:34)](https://podwise.ai/dashboard/episodes/7508210?locate=3994)
 would mean that China would be ahead in its ability to... Produce mass flops.

**Dylan Patel:**
[(1:06:40)](https://podwise.ai/dashboard/episodes/7508210?locate=4000)
Yeah. So to date, China still does not have, you know, entire indigenized semiconductor supply chain. Right.

**Dwarkesh:**
[(1:06:47)](https://podwise.ai/dashboard/episodes/7508210?locate=4007)
But within 2030. Yeah.

**Dylan Patel:**
[(1:06:48)](https://podwise.ai/dashboard/episodes/7508210?locate=4008)
By 2030, it's it's possible that they do. But but to date, right. All of China's seven nanometer and 14 nanometer capacity uses ASML DUV tools. Right. And the amount that they can ship and import from ASML is large. But the point being that the vast majority of ASML's revenue, especially on EUV,  all of it is outside of China. So the scale advantage is still in the favor of the, let's call it the West plus Taiwan,  Japan, et cetera.

**Dwarkesh:**
[(1:07:18)](https://podwise.ai/dashboard/episodes/7508210?locate=4038)
They're trying to make their own DUV and EUV tools, right?

**Dylan Patel:**
[(1:07:20)](https://podwise.ai/dashboard/episodes/7508210?locate=4040)
They're trying to do all these things. The question is how fast can they advance and scale up production as well as quality. And to date, we haven't seen that. Now, I'm quite bullish that they're going to be able to do these things over the next five to 10 years,  right? Really scale up production, really kick it into high gear. They have more engineers working on it. They have more desire to throw capital at the problem.

**Dwarkesh:**
[(1:07:43)](https://podwise.ai/dashboard/episodes/7508210?locate=4063)
So by 2030, do they have fully indigenized EUV?

**Dylan Patel:**
[(1:07:46)](https://podwise.ai/dashboard/episodes/7508210?locate=4066)
I think for sure, for sure. EUV, yes.

**Dwarkesh:**
[(1:07:47)](https://podwise.ai/dashboard/episodes/7508210?locate=4067)
And fully indigenized EUV by 2030? I think they'll have working tools.

**Dylan Patel:**
[(1:07:51)](https://podwise.ai/dashboard/episodes/7508210?locate=4071)
I don't think that they'll be able to manufacture A bunch yet right you know there's there's sort of having it work and then there's production hell right and ultimately like ASML had EUV working. In the early 2010s at some capacity. Right. Now, the tools were not accurate enough. They were not scaled for high production, scaled for high volume manufacturing, reliable enough. And then they had to ramp production. And that all took time. Production hell takes time. Right. Which is why it took another five to seven years to get EUV into mass production at a fab rather than just working in the lab.

**Dwarkesh:**
[(1:08:26)](https://podwise.ai/dashboard/episodes/7508210?locate=4106)
So how many EUV tools do you think anybody will manufacture in 2030?

**Dylan Patel:**
[(1:08:30)](https://podwise.ai/dashboard/episodes/7508210?locate=4110)
ASML?

**Dwarkesh:**
[(1:08:31)](https://podwise.ai/dashboard/episodes/7508210?locate=4111)
No, China.

**Dylan Patel:**
[(1:08:32)](https://podwise.ai/dashboard/episodes/7508210?locate=4112)
Oh, that's a great question. It's a bit of a challenge to look into this supply chain, especially we try really hard. But, you know, in some instances, they're like buying stuff from Japanese vendors. And if they want a fully indigenized supply chain,  they need to not buy these lenses or buy these projection optics or stages from Japanese vendors. They need to build it internally. So it's really tough to say where they'll be able to get to. Like, I honestly think it's like a shot in the dark,  but it's probably not unlikely that they'll be able to do,  you know, on the order of 100 DUV tools a year,  whereas ASML is doing hundreds of DUV tools a year currently.

[(1:09:13)](https://podwise.ai/dashboard/episodes/7508210?locate=4153)
You know, no one's made No company has a process node where they make a million wafers a month, right? Elon says he wants to do it, and China's obviously going to do it, right? And I don't think the, you know, TSMC is trying to do that. The memory makers may get there as well, right, to the million wafers a month,  but not in a single fab. It's sort of mind-boggling to think of that scale and challenging to see the supply chain galvanize for that. So I'm not sure, you know, I don't want to doubt, you know, China's capability to scale.

**Dwarkesh:**
[(1:09:48)](https://podwise.ai/dashboard/episodes/7508210?locate=4188)
Right. I guess this is an interesting question that I think it might, you know,  at some point, semi-analysis will do the deep dive on this. But I think this question of, like, by when would China be able, like,  indigenized Chinese production could be bigger than the rest of the West combined, if you just add up,  like, And put in the input of your model when they'll have DUV machines at scale,  when they'll have DUV machines at scale. Because I think there's this question around if you have long timelines on AI,  by long meaning 2035, which is not that long in the grand scheme of things. Should you expect a world where China is dominating in semiconductors?

[(1:10:25)](https://podwise.ai/dashboard/episodes/7508210?locate=4225)
Which I think, I don't know, it doesn't get asked enough. In San Francisco, we're just thinking on timescale of weeks. And then if you're outside of San Francisco, you're not thinking about AGI at all. And so this question of like, OK, what if we have AGI? What if you have this transformational thing that is commanding tens of trillions of dollars or hundreds of trillions of dollars of economic growth and,  you know, token output and so forth? But then it happens in 2035. And what does that imply for the West versus China? I think it's just like, I don't know, the semi analysis has got to ride the definitive model on this.

**Dylan Patel:**
[(1:10:55)](https://podwise.ai/dashboard/episodes/7508210?locate=4255)
Yeah. It's really challenging when you move timescales out that far. What we tend to focus on is we're tracking every data center, we're tracking every fab,  we're tracking all the tools, and we're tracking where they're going,  but the time lags for these things are relatively short. We can only make reasonably accurate estimates for data center capacity based on land purchasing and permits and turbine purchasing and all these things. And we know where all these things are going and that's what the data we sell is. But as you go out to 2035, things are just so radically different and your error bars get so large,  it's kind of hard to make an estimate. But at the end of the day, you know,

[(1:11:37)](https://podwise.ai/dashboard/episodes/7508210?locate=4297)
 there is if takeoff or timelines are slow enough,  right, then certainly China, I don't see why they wouldn't be able to catch up drastically,  right. You know, in some sense, we've got like this valley right of where Call it three to six months ago,  Chinese models were, or maybe even now, Chinese models are competitive as they've ever been. I think Opus 4.6 and GPT 5.4 have really pulled away and made the gap a little bit bigger,  but I'm sure some new Chinese models will come out. But as we move from, hey, these companies are selling tokens where they provide the entire reasoning chain and all that to selling automated White-collar work,  right?

[(1:12:15)](https://podwise.ai/dashboard/episodes/7508210?locate=4335)
Automated software engineer, send them the request, they give you the result back,  and there's a bunch of thinking on the back end that they don't show you. The ability to distill out of American models into Chinese models will be harder, A. B, as the scale of the compute that the labs have, right? OpenAI exited the year with roughly 2 gigawatts last year. Anthropic will get to 2 plus gigawatts this year. And by the end of next year, they'll both be at like 10 gigawatts of capacity. China is not scaling their AI lab compute nearly as fast. And so at some point, when you can't distill the learnings from these labs into the Chinese models,

[(1:12:49)](https://podwise.ai/dashboard/episodes/7508210?locate=4369)
 plus this compute race that OpenAnthropic, Google, et cetera, Meta are all racing on,  at some point, they end up getting to a point where You know,  the model performance should start to diverge more. And then all of this CapEx that's being spent on, you know, data centers and all that, right? Amazon, you know, 200 billion, Google 180, you know, so on and so forth. All these companies are spending hundreds of billions of dollars of CapEx. You know, there's nearly a trillion dollars of CapEx being invested in data centers in America this year, roughly, right? You end up with, okay, well, what's the return on invested capital here?

[(1:13:27)](https://podwise.ai/dashboard/episodes/7508210?locate=4407)
You and I would think that the return on invested capital for data center CapEx is very high. And at least if we look at Anthropx revenues in January, they added like $4 billion. In February, which is a shorter month, they added like $6. We'll see what they can do in March and April, given compute constraints are what's bottlenecking their growth, right? The reliability of Claude code is actually quite low because they're so compute constrained. But if this continues, then the ROIC on these data centers is super high. And at some point, the US economy starts growing faster and faster over the next,

[(1:13:59)](https://podwise.ai/dashboard/episodes/7508210?locate=4439)
 you know, this year and next year, because of all this capex and all this revenue that these models are generating and downstream supply chain. Versus China doesn't have that yet, right? They have not built the scale of infrastructure to then invest in models to get to the capabilities to then deploy these models at such scale,  right? Because when you look at like Anthropx, hey, they're at, call it 20 billion ARR. Of that, the margins are sub 50% at least last reported by the information. So then you're at, okay, that's like $13, $14 billion of compute that it's running on rental cost wise,

[(1:14:33)](https://podwise.ai/dashboard/episodes/7508210?locate=4473)
 which is actually like $50 billion worth of capex that someone laid out for Anthropic to generate their current revenue. And China has just not done this. If and when Anthropic 10X has revenue again,  and I think our answer would be when,  not if, then China doesn't have the compute to deploy at that scale. And so there is some sense of like, oh, we're in fast takeoff-ish, right? It's not like we're talking about Dyson sphere by X date. It's more like the revenue is compounding at such a rate that it does affect the economic growth. And the resources these labs are gathering are going so fast that China hasn't done that yet. So in that case, the US and the West is actually diverging.

[(1:15:15)](https://podwise.ai/dashboard/episodes/7508210?locate=4515)
The flip side is actually these infrastructure investments Have middling returns. Maybe they're not as good as hoped. Maybe Google is wrong for wanting to take free cash flow to zero and spend $300 billion on CapEx next year. Maybe they're just wrong. And people on Wall Street who are bearish and people who don't understand AI are correct. And in which case, then the US is building all this capacity. It doesn't get really great returns. And China is able to build the fully vertical indigenized supply chain,  not US Japan korea taiwan southeast asia you know you're up all these all these countries together building this like less vertical supply chain.

[(1:15:57)](https://podwise.ai/dashboard/episodes/7508210?locate=4557)
And in a sense, at some point, China is able to scale past us. If AI takes longer to get to certain capability levels,  then I would say the vast majority of your guests on this podcast believe.

**Dwarkesh:**
[(1:16:07)](https://podwise.ai/dashboard/episodes/7508210?locate=4567)
It's like fast timelines, US wins, long timelines, China wins.

**Dylan Patel:**
[(1:16:10)](https://podwise.ai/dashboard/episodes/7508210?locate=4570)
Right. But I don't know what fast timelines means. I don't think you have to believe in AGI to have the timelines where the US wins.

**Dwarkesh:**
[(1:16:19)](https://podwise.ai/dashboard/episodes/7508210?locate=4579)
Okay,  let's go back to memory because I think this is maybe people on Wall Street and people in the industry are understanding how big this is,  but maybe generally people don't understand how big a deal this is. So we've got this memory crunch, as you're talking about, and earlier I was asking about,  oh, could we solve for the EUV tool shortage by going back to seven nanometers? So let me ask a similar question about memory. HBM is made of DRAM, but has three to four X less bits per wafer area than the DRAM is made out of. Is it possible that accelerators in the future could just use commodity DRAM and not HBM? And so just we can make much more capacity out of the DRM we get.

[(1:16:58)](https://podwise.ai/dashboard/episodes/7508210?locate=4618)
And the reason I think this might be possible is, look,  If we're going to have agents that are just going off and doing work and it's not a synchronous chatbot application,  then you don't necessarily need extremely high fast latency kinds of things anymore. And so maybe you can have the low bandwidth because the reason you stack DRAM into stacks and make HBM is for higher bandwidth. And so is it possible to go to HBM accelerators and basically have the opposite of Claude Code fast,  like have Claude Code slow and do that?

**Dylan Patel:**
[(1:17:35)](https://podwise.ai/dashboard/episodes/7508210?locate=4655)
I think at the end of the day,  the incremental purchaser who's willing to pay the highest price for tokens also ends up being the one that's like, They're less price sensitive and the compute should be allocated in a capitalistic society towards the goods that have the highest value and the private market determines this by willingness to pay. To some extent, sure, Anthropic could actually release a slow mode. They could release Claude slow mode and have an increase in tokens per dollar by a significant amount. They could probably reduce the price of Opus 4.6 by You know, 4x,

[(1:18:10)](https://podwise.ai/dashboard/episodes/7508210?locate=4690)
 5x and reduce the speed by another by maybe just like 2x like the curve on inference throughput versus speed is there already just on HBM and yet they don't because no one actually wants to use a slow model and furthermore on these agentic tasks. It's great that the model can run at this time horizon of hours. It's kind of like, okay, well, if the model was just running slower, that hours would become a day, right? Or vice versa, right? If the model is running faster, that hours becomes hour. And yet,  no one really wants to move to that day-long wait period because the highest value tasks also have some time sensitivity to them,  right? And so I struggle to see, you know, yes, you could use DDR,

[(1:18:54)](https://podwise.ai/dashboard/episodes/7508210?locate=4734)
 but then there's a couple like things that are challenging with this,  right? You could use regular DRAM. One is you're still limited, you know, one of the like core constraints of chips,  even though they're, you know, sort of like, you know,  there's a chip is like a certain size,  all of the IO escapes on the edges of the chip, right? So oftentimes, you know, what you see is the left and the right of the chip are HBM,  the IO from the chip to the HBM is on the sides and then the top and bottom are IO to other chips,  right? And so if you were to change from HBM to DDR,  then all of a sudden this IO on this edge would have significantly less bandwidth,

[(1:19:36)](https://podwise.ai/dashboard/episodes/7508210?locate=4776)
 but it had significantly more capacity per chip. And so, yes, you're making less You know,  the metric that you actually care about is bandwidth per wafer,  not bits per wafer.

**Dwarkesh:**
[(1:19:50)](https://podwise.ai/dashboard/episodes/7508210?locate=4790)
Because the thing that is constraining the flops is just getting in and out the next matrix and for that you just need more bandwidth.

**Dylan Patel:**
[(1:19:58)](https://podwise.ai/dashboard/episodes/7508210?locate=4798)
Yeah, getting out the weights and getting in and out the KV cache.

**Dwarkesh:**
[(1:20:01)](https://podwise.ai/dashboard/episodes/7508210?locate=4801)
Right.

**Dylan Patel:**
[(1:20:02)](https://podwise.ai/dashboard/episodes/7508210?locate=4802)
In many cases, these GPUs are not running at full memory capacity. Yes, it's obviously like a system design thing, you know, model hardware, software co-design of,  hey, what do I, what do I, how much KVCache do I do? How much do I keep on the chip? How much do I offload to other chips and call when I need it for tool calling or whatever? How much do I, how many chips do I paralyze this on? Obviously these are like, the search space of this is like very broad,  which is why we have like inference X,  like this is like an open source model,  like searches all the optimal points on inference for a variety of eight different chips. Um, and models.

[(1:20:33)](https://podwise.ai/dashboard/episodes/7508210?locate=4833)
Um, anyways, like the point is you don't necessarily, you're not always necessarily constrained by memory capacity. Uh, you can be constrained by flops. You can be constrained by network bandwidth. You can be constrained by memory bandwidth, uh, or you can be constrained by memory capacity. There's sort of like four, if you're really to simplify it down,  there's like four constraints and each of these can break out into more. But in this case, if you switch to DDR, yes, you produce 4x the bits. Per DRAM wafer, but all of a sudden the constraints shift a lot and your system design shifts a lot. You go slower. Yes. Is the market smaller?

[(1:21:06)](https://podwise.ai/dashboard/episodes/7508210?locate=4866)
Okay, maybe possibly, but also now all of a sudden all these flops are wasted because they're just sitting there waiting for memory. It's like, great. I don't need all that capacity because I can't really increase batch size because then the KB cache is going to take even longer to read. And so you never, you can, yeah.

**Dwarkesh:**
[(1:21:21)](https://podwise.ai/dashboard/episodes/7508210?locate=4881)
Interesting. What is the bandwidth difference between HBM and A normal DRM?

**Dylan Patel:**
[(1:21:26)](https://podwise.ai/dashboard/episodes/7508210?locate=4886)
Yeah. So an HBM stack of HBM4, let's just talk about like the stuff that's in Rubin because that's what we've been indexing on,  is 2048 bits across connected in an area that's like 13 millimeters wide. So 2048 bits and it transfers memory at around 10 gigatransfers a second. So HBM, a stack of HBM4 is 2048 bits on an area that's 13 millimeters wide,  roughly, or 11. And that's the shoreline that you're taking on the chip. And in that shoreline, you have 2048 bits transferring at 10 gigatransfers per second. You multiply those together and you divide by eight bits to bytes. You're at roughly two and a half terabytes a second per HBM stack, right?

[(1:22:05)](https://podwise.ai/dashboard/episodes/7508210?locate=4925)
When you look at DDR, in that same area, it's maybe 64 or 128 bits wide. And that DDR5 is transferring at anywhere from 6.4 gigatransfers a second. To maybe 8,000 gigatransfers a second. So your bandwidth is significantly lower, right? It's 64 times 8,000 divided by 8. You're at 64 gigabytes a second. And even if you take a generous interpretation of 128 times 8 gigatransfers,  you're at 128 gigabytes a second for the same shoreline versus two and a half terabytes a second. There's an order of magnitude difference in bandwidth per edge area. And if your chip is a square or it's 26 by 33, right, is the maximum size for a chip,  individual die, you only have so much edge area.

[(1:22:50)](https://podwise.ai/dashboard/episodes/7508210?locate=4970)
And then on the inside of that chip, you put all your compute. There's things you can do to try and change, right? More SRAM, more caching, blah, blah, blah. But at the end of the day, you're very constrained by bandwidth.

**Dwarkesh:**
[(1:22:59)](https://podwise.ai/dashboard/episodes/7508210?locate=4979)
Interesting. So then there's a question of like, where can you destroy demand to free up enough for AI? And I guess the picture is especially bad because as you're saying,  if it takes 4X more wafer area to get the same byte for HBM,  you had to destroy 4X as much consumer demand for laptops and phones and whatever in order to free up one byte for AI. Yeah, what does this imply for the next year or two of... Sorry for the run-on question. I think on your newsletter, you said 30% of the CapEx in 2026 of big tech is going towards memory.

**Dylan Patel:**
[(1:23:34)](https://podwise.ai/dashboard/episodes/7508210?locate=5014)
Yes.

**Dwarkesh:**
[(1:23:35)](https://podwise.ai/dashboard/episodes/7508210?locate=5015)
That's insane, right?

**Dylan Patel:**
[(1:23:36)](https://podwise.ai/dashboard/episodes/7508210?locate=5016)
Yeah.

**Dwarkesh:**
[(1:23:36)](https://podwise.ai/dashboard/episodes/7508210?locate=5016)
Like of the 600 billion or whatever, you're saying 30% is going just to just to.

**Dylan Patel:**
[(1:23:42)](https://podwise.ai/dashboard/episodes/7508210?locate=5022)
And, you know, obviously there's some level of like margin stacking that Nvidia does. And so if you separate out, you know, and you apply their margin to the memory and the logic. But at the end of the day, yeah, like a third of their capex is going to memory.

**Dwarkesh:**
[(1:23:52)](https://podwise.ai/dashboard/episodes/7508210?locate=5032)
That's that's that's crazy. OK, so what is the question I'm trying to ask is something like, yeah, what is this? What basically what should we expect over the next year or two as this memory crunch hits?

**Dylan Patel:**
[(1:24:00)](https://podwise.ai/dashboard/episodes/7508210?locate=5040)
Yeah, so memory crunch will continue to be harder and harder and prices continue to go up. And this affects different parts of the market differently, right? Gets to sort of the like, are people going to hate AI more and more? Yes, because now smartphones and PCs are not going to get incrementally better year on year. And in fact, they're getting incrementally worse.

**Dwarkesh:**
[(1:24:19)](https://podwise.ai/dashboard/episodes/7508210?locate=5059)
If you look at the bill of materials of an iPhone, what fraction of it is the memory? Like how much more expensive does an iPhone get if the memory is 2x more expensive or whatever it has to be?

**Dylan Patel:**
[(1:24:27)](https://podwise.ai/dashboard/episodes/7508210?locate=5067)
So I believe an iPhone has 12 gigabytes of memory Each gig cost used to cost roughly three or four dollars. So it's 50 bucks but now the price of memory is like Triple, let's call it if it's now,  it's $12 per gig for DDR. So now you're talking about $150 versus $50, right? $100 increase in cost on Apple. Also, Apple has some margin, they're not just going to eat the margin. So now that's $100 cost increase. That's just on the DRAM. The NAND also has the same sort of like market. So in fact, you know, it's probably $150 increase on the iPhone. Apple has to either pass it on to the consumer, A, or B, they have to eat it. I don't see Apple reducing their margin too much. Maybe they eat a little bit.

[(1:25:08)](https://podwise.ai/dashboard/episodes/7508210?locate=5108)
But at the end of the day, that means the end consumer is paying $250 more for an iPhone. And now that's on like, hey, what is last year's memory pricing versus today's? Now, there is some lag for Apple to have to feel the heat because they have tended to have,  you know, three, six or a year long contracts for a lot of memory. But at the end of the day, Apple gets hit pretty hard by this. But they won't really adjust until the next iPhone release. But that's the high end of the market. Actually, that's only a few hundred million phones a year, right? Apple sells, what, two, three hundred million phones a year.

[(1:25:40)](https://podwise.ai/dashboard/episodes/7508210?locate=5140)
The bulk of the market This mid-range low-end, right, used to be 1.4 million smartphones were sold a year. Now we're at like 1.1. But our projections are we maybe get down to like 800 million this year and next year like 600 or 500 million. And we look at like, you know,  there's some data points out of China from some of our analysts in Asia and Singapore and Hong Kong and Taiwan. They've been tracking this and they see Xiaomi and Oppo are cutting low-end and mid-range smartphone volumes by half. Because, yes, it's only a $150 price increase on a $1,000 smartphone or $150 bomb increase on a $1,000 iPhone where Apple has some larger margin. But if we look at the smaller phones,

[(1:26:22)](https://podwise.ai/dashboard/episodes/7508210?locate=5182)
 the percentage of the bomb that goes to memory and storage is much larger,  and the margins are lower. So there's less capacity to even eat the margins. And they have generally tended not to do as long-term agreements on memory. Why this is like a big deal is if smartphone volumes, let's say half,  The halving will frankly happen in the low and mid range, not in the high end. So it's not like the bits released are halving, right? You know, currently consumers more than half of memory demand,  even if you half the smartphone volumes because of the shape of the halving,  right? It's like low end gets cut by more than half,  high end gets cut by less than half,  because you and I will buy, you know,

[(1:27:03)](https://podwise.ai/dashboard/episodes/7508210?locate=5223)
 the high end phones that cost north of $1,000,  we'll buy them, even if they get a little bit more expensive. And Apple's volumes will not go down as much as like a low end smartphone provider. And the same applies to PCs And what this does to the market is quite drastic, right? DRAM gets released, goes to AI chips who are willing to do longer term contracts,  willing to pay higher margins, etc., etc., because at the end of the day,  the margin that they extract is much larger from the end user or whatever. And so this probably leads to like People are hating AI even more, right?

[(1:27:36)](https://podwise.ai/dashboard/episodes/7508210?locate=5256)
Because they're going to start being like, today you already see all the memes like on PC subreddits and PC like Twitter,  gaming PC Twitter is like, you know, cat dancing videos. And it's like, this is why memory prices is doubled and you can't get a new gaming GPU, right? Or you can't get a new desktop. And it's going to be even worse when memory prices double again, especially DRAM. Another dynamic that's quite interesting is it's not just DRAM, it's also NAND. NAND is also going up in price. Both of these markets have expanded capacity very slowly over the last few years,  NAND almost zero,

[(1:28:08)](https://podwise.ai/dashboard/episodes/7508210?locate=5288)
 but smartphones The percentage of NAND that goes to phones and PCs is larger than the percentage of DRAM that goes to phone and PC. So as you destroy demand, you unlock, you know, mostly for the DRAM purposes,  you unlock more NAND that gets allocated and can sort of go to other markets. And so the price increases of DRAM will be larger than those of NAND because you've released more from the consumer. And in fact, you've produced more memory for AI.

**Dwarkesh:**
[(1:28:35)](https://podwise.ai/dashboard/episodes/7508210?locate=5315)
Sorry, but the NAND is, maybe you just explained it and I missed it. Is it because SSDs are being used in large quantities for data centers or?

**Dylan Patel:**
[(1:28:42)](https://podwise.ai/dashboard/episodes/7508210?locate=5322)
They are, but not as large quantities as DRAM.

**Dwarkesh:**
[(1:28:46)](https://podwise.ai/dashboard/episodes/7508210?locate=5326)
Okay, but you're saying they will also increase because they're using some quantity,  but like there's not as much need as there is for HBM. Makes sense. One thing I didn't appreciate until I was reading some of your newsletters is that basically the same constraints that are preventing logic scaling over the next few years,  it's quite similar to what's preventing us from producing more memory wafers. In fact, like literally the same exact machine. This EUV tool is needed for memory. So I guess, yeah, maybe there's a question that somebody could be asking right now,  like, well, why can't we just make more memory?

**Dylan Patel:**
[(1:29:19)](https://podwise.ai/dashboard/episodes/7508210?locate=5359)
Is that somebody?

**Dwarkesh:**
[(1:29:20)](https://podwise.ai/dashboard/episodes/7508210?locate=5360)
Yeah, who knows?

**Dylan Patel:**
[(1:29:23)](https://podwise.ai/dashboard/episodes/7508210?locate=5363)
So I think the constraints, as I was mentioning earlier, are not necessarily EUV tools today or next year. They become that as we get to the latter part of the decade. But currently, right, the constraints are more so they physically just haven't built fabs. Right. So over the last Three to four years, these vendors have just not built new fabs. That's because memory prices were really low. Their margins were low. And in fact, they were losing money in 2023 on memory. So they're like, oh, we're not building new fabs. And then like the market slowly recovered over time, but never really got amazing until last year.

[(1:29:59)](https://podwise.ai/dashboard/episodes/7508210?locate=5399)
In 2024, we were banging on the drums that reasoning means long context, which means large KV cache,  which means you need a lot of memory demand. We've been talking about that for a year and a half, two years. People who understand AI Like went really long memory then, right? You know, and so you've seen that sort of like dynamic, but now it finally played out in pricing. It took so long for what was obvious, right? Hey, long context, KV cash gets bigger, you need more memory and accelerators, half their cost is memory. So of course, they're just going to start, you know, they're going to start like going crazy on it. It took a year for that to actually reflect in memory prices.

[(1:30:35)](https://podwise.ai/dashboard/episodes/7508210?locate=5435)
Once memory price is reflected, then it took another six months,  three months for the memory vendors to start building fabs. And those fabs take two years to build. And so we don't have really meaningful fabs that you can even put these tools in until late 27 or 28, right? And so instead what you've seen is like some really crazy stuff to get capacity. Micron bought a fab from a company in Taiwan that makes lagging edge chips. Hynix and Samsung are doing some pretty crazy things to try and expand capacity at their existing fabs that also have very large knock-on effects in the economy. And so, hey, why can't we build more capacity? There's nowhere to put the tools. And it's not just EUV.

[(1:31:22)](https://podwise.ai/dashboard/episodes/7508210?locate=5482)
There's other tools involved in DRAM and logic. Logic, you know, N3, 30% or so of the cost, you know,  28% of the cost is EUV of the wafer,  of the final wafer. When you look at like DRAM, it's in the teens. And it's going up, but it's in the teens. So it's a much smaller percentage of the cost is DRAM or is EUV. These other tools are also bottlenecks, although their supply chains are not as complex as ASMLs. And so you see Applied Materials and Lam Research and all these other companies also expanding capacity a lot. And anyways,  you don't have anywhere to put the tool because the most complex building that people make is fabs and fabs take two years to build.

**Dwarkesh:**
[(1:32:02)](https://podwise.ai/dashboard/episodes/7508210?locate=5522)
You can think of Jane Street as a research lab with a trading desk attached. Their infrastructure team has built some of the biggest research clusters in the world with tens of thousands of high-end GPUs and hundreds of thousands of CPU cores and exabytes of storage. This compute is part of how Jane Street surfaces all the hidden patterns that are embedded in incredibly noisy market data. Even beyond the noise, the nature of the signal changes constantly in reaction to things like pandemics and elections and new regulations,  and even changes in sentiment. There's this unremitting game of trying to figure out whether your old models still reflect the real world,  and if not, what to do about it.

[(1:32:34)](https://podwise.ai/dashboard/episodes/7508210?locate=5554)
If you're interested in working on this sort of thing, Jane Street is hiring ML researchers and engineers. They're also accepting applications for their summer ML internship program with spots in London, New York and Hong Kong. And if you happen to find yourself at GTC,  which is happening the week after this episode drops,  Jane Street's GPU performance team is giving a talk. Go to janestreet.com slash Dwarkesh to learn more. I interviewed Elon recently and his whole plan is that I guess they're going to build this Gigafab,  TerraFab, some power of 10, and they're going to build the clean rooms. I don't even ask you about the dirty rooms thing, but let's say they build the clean rooms.

[(1:33:15)](https://podwise.ai/dashboard/episodes/7508210?locate=5595)
Okay, I have a couple of questions. One,  Do you think this is the kind of thing that ElonCo could build much faster than people are conventionally building it? This is not about building the end tools. This is just about building the facility itself. How complicated is it to just build a clean room and do it extremely fast? Is this something that like Elon with his move fast thing could do much faster if that's what we're bottlenecked on this year or next year? And two, does that even matter if in two years,  your view is that we're not bottlenecked on clean room space,  but we're bottlenecked on the tooling?

**Dylan Patel:**
[(1:33:45)](https://podwise.ai/dashboard/episodes/7508210?locate=5625)
So I think, you know, as with any complex supply chain, it takes time and constraints shift over time. And even if something isn't any longer a constraint, that doesn't mean that market no longer has margin, right? So, for example, energy will not be a big bottleneck as we get to,  you know, a couple of years from now. But that doesn't mean energy is not growing super fast and there's no margin there. It's just like it's not the key bottleneck. And in the space of fabs, right, clean rooms are the biggest bottleneck this year and next year. And as we get over time, 29, you know, 28, 29, 30, there will be still constraints there.

[(1:34:16)](https://podwise.ai/dashboard/episodes/7508210?locate=5656)
The thing about Elon is, I think he's had a tremendous capability to garner physical resources and really smart people to build things. And the way he's able to recruit really amazing people is just try and build the craziest stuff, right? In the case of AI, that's not really worked because everyone's trying to build AGI. Everyone's very ambitious. But in the case of like, we're going to make We're going to go to Mars and we're going to make rockets that land themselves,  or we're going to make fully autonomous cars that are electric, or we're going to make human-aid robots.

[(1:34:44)](https://podwise.ai/dashboard/episodes/7508210?locate=5684)
These are methods of recruiting the people who think that's the most important problem in the world to work on that problem because he's the only one trying really hard. In the case of semiconductors, I want to make a fab that's a million wafers per month. No one has a fab that big. That's what he stated, right? He wants to make a million wafers a month. It's possible that he's able to recruit a lot of really awesome people and get them on this crazy task of trying to build a fab that does a million wafers per month. Step one is to build the clean room. And I think that he probably can do, right? I think, you know, there's some mindset, you know, his mindset around like delete things.

[(1:35:14)](https://podwise.ai/dashboard/episodes/7508210?locate=5714)
It can be dirty. It's fine. Probably not right. Or actually, I think 100% it's not right. You like need the fab to be very clean. I think the entire air, the entire, all of the air in the fab gets replaced like every three seconds. It's like that fast, and there's so few particles per, but I think he can build a clean room. It'll take a year or two, maybe. Initially, it won't be super fast, but then over time, he'll get faster and faster at it. Then the really complex part is actually developing a process technology and building wafers,  and I don't think he can develop that quickly. I think that has a lot of built-up knowledge. It's, again,

[(1:35:48)](https://podwise.ai/dashboard/episodes/7508210?locate=5748)
 like the most complicated integration of And the only very expensive tools and supply chain that's done is a TSMC or an Intel or a Samsung. And those, some of these, these two other two companies aren't even that great. And they're like tremendously complex.

**Dwarkesh:**
[(1:36:02)](https://podwise.ai/dashboard/episodes/7508210?locate=5762)
How surprised would you be if in 2030 people like there just happened to be some total disruption where we're not using UV,  we're using something that has like much better factors, much simpler to produce. We can produce in much bigger quantities. I'm sure as an industry insider, that sounds like a totally naive question, but do you see what I'm asking? What probability should we put on, oh, something totally out of the left field comes out and none of this is relevant?

**Dylan Patel:**
[(1:36:26)](https://podwise.ai/dashboard/episodes/7508210?locate=5786)
Something that's very simple and easy to scale, I have very, very low probability for. There are a number of companies working on effectively like Particle accelerators or synchrotrons that generate light that's either 13.5 nanometer like EUV or even x-ray like even narrower wavelength like 7 nanometer or whatever wavelengths of light to then use in lithography tools. But those things are like massive particle accelerators that are then generating this light. It's a very complicated thing to build. So there's a couple companies and I think that that could be a big disruption to the industry beyond what EUV is.

[(1:36:58)](https://podwise.ai/dashboard/episodes/7508210?locate=5818)
I don't necessarily think that like We're going to just magically build something new that is like direct write and super simple and can be manufactured at huge volumes,  although there are some attempts to do things like this.

**Dwarkesh:**
[(1:37:09)](https://podwise.ai/dashboard/episodes/7508210?locate=5829)
Yeah. Because I ask because if you think about Elon Co's in the past,  rocketry was this thing that was thought to be,  I mean, it is incredibly complicated.

**Dylan Patel:**
[(1:37:17)](https://podwise.ai/dashboard/episodes/7508210?locate=5837)
Look, I'm just a naive yapper compared to Elon, right? What have I built? So maybe it's possible, right?

**Dwarkesh:**
[(1:37:24)](https://podwise.ai/dashboard/episodes/7508210?locate=5844)
In order to be able to build more memory in the future,  could we build 3D DRAM the way we do 3D NAND and then go back to DUV?

**Dylan Patel:**
[(1:37:33)](https://podwise.ai/dashboard/episodes/7508210?locate=5853)
This is the hope currently. Everyone's roadmap for 3D DRAM is that you'll still use EUV because you want to have that tighter overlay because now when you're doing these subsequent processing steps,  You want it to be, you know, everything's vertically stacked. You have more layers on top of each other. And you want the pitches to be tighter and all these things. So generally, people are still trying to do an EUV,  but what 3D would do is it would take the,  you know, hey, a single EUV pass, how many bits can it make, right? If you do this sort of like calculation, and that number would go up drastically if you go to 3DDRAM.

[(1:38:04)](https://podwise.ai/dashboard/episodes/7508210?locate=5884)
That is the hope, but right now everyone's roadmap is sort of like you go from current,  it's called a 6F cell to a 4F cell,  and then finally 3DDRAM by the end of the decade or early next decade. So there's still a lot of R&D and manufacturing and integration to be done. I wouldn't call that out of the cards. I think it's very much likely going to happen. It also is going to require a huge retooling of fabs, right? The breakdown of tools in a fab are very different. Actually, the lithography tool is the only thing that isn't that different,

[(1:38:35)](https://podwise.ai/dashboard/episodes/7508210?locate=5915)
 but the number of them relative to different types of chemical vapor deposition or atomic layer deposition or dry etch or different kinds of etch chambers with different chemistries,  all of these things You have all these different kinds of tools for different process nodes. You can't just convert a logic fab to a DRAM fab or vice versa,  back and forth, or a NAND fab to a DRAM fab in a short amount of time. In the same way,  existing DRAM fabs We require a lot of retooling just to go from one alpha to one beta to one gamma process nodes,  because now they have to add to EUV and change the chemistry stacks for when you're using EUV in terms of deposition and etch,

[(1:39:10)](https://podwise.ai/dashboard/episodes/7508210?locate=5950)
 and the EUV tool has to be there. And furthermore, when you change to 3D DRAM, there's going to be an even larger shift. And so there's a lot of retooling of these fabs that needs to happen in terms of the tools. And so that would be a big disruption. That would make EUV demand generally lower. But as we've seen across time, EUV demand as a percentage of wafer costs has trended up initially,  or lithography, right? Lithography initially, I want to say in like 2014-ish era, was like 16% of the wafer cost,  17%, and it's gone to 30 over the last 15 years. And for DRAM, it was in the mid-teens as well, or low-teens, and now it's trended towards the high-teens.

[(1:39:48)](https://podwise.ai/dashboard/episodes/7508210?locate=5988)
And before we get to 3D DRAM, it'll likely cross into the 20s percentage range. But then if we get to 3D DRAM,  it tanks again in terms of the total end wafer cost as a percentage of EUV.

**Dwarkesh:**
[(1:39:58)](https://podwise.ai/dashboard/episodes/7508210?locate=5998)
Yeah. I guess you care less about the percent of cost and more about how much it bottlenecks.

**Dylan Patel:**
[(1:40:02)](https://podwise.ai/dashboard/episodes/7508210?locate=6002)
Right, but the percentage of cost is sort of...

**Dwarkesh:**
[(1:40:05)](https://podwise.ai/dashboard/episodes/7508210?locate=6005)
A proxy, yeah, yeah.

**Dylan Patel:**
[(1:40:05)](https://podwise.ai/dashboard/episodes/7508210?locate=6005)
Yeah.

**Dwarkesh:**
[(1:40:06)](https://podwise.ai/dashboard/episodes/7508210?locate=6006)
So if you're Jensen or Sam Waltman or whoever who stands to gain a lot from scaling up AI compute,  there's these stories that they'd go to TSMC and say, hey, why can't we actually Y and Z? But I think the point you're making here is It doesn't really matter in some sense what TSMC does. And in fact, even if you have Intel and Samsung building more foundries, in the long run,  you're going to be bottlenecked by ASML and other toolmakers and other material makers. So first, is that correct interpretation? And second, then why should basically Silicon Valley people be going to the Netherlands to try to pitch ASML?

[(1:40:43)](https://podwise.ai/dashboard/episodes/7508210?locate=6043)
Like right now, should they be trying to pitch ASML to make more tools so that like in 2030,  they can have more AI compute?

**Dylan Patel:**
[(1:40:48)](https://podwise.ai/dashboard/episodes/7508210?locate=6048)
It's a funny dynamic we saw in 2023-2024 and 2025.  People who saw the energy bottleneck before others asymmetrically went to Siemens,  Mitsubishi,  and of course GE Vernova and bought up turbine capacity and now they're able to charge excess amounts for deploying these turbines places because of energy. In the same sense,  this could be done for EUV except ASML is not just going to trust any random bozo who wants to buy EUV tools in the sense that these turbines are much cheaper than EUV tools,  and there's many more of them produced, especially once you get to industrial gas turbines or like,  you know, not just combine cycle, but like the cheaper, smaller, et cetera, less efficient ones.

[(1:41:31)](https://podwise.ai/dashboard/episodes/7508210?locate=6091)
People put down deposits for these. So in a sense, someone could do this, right? Someone should go to the Netherlands and be like, I'll pay you a billion dollars. You give me the right to purchase 10 EUV tools two years from now. And I'm first in line two years from now. And then over those two years, you then go around and wait for everyone to realize,  oh crap, I don't have enough EUV tools. And then you try and sell your option at some premium. But all you're effectively doing is you're saying, ASML, you're dumb. You weren't making enough margin on these. I'm gonna make a margin. And the question is like, will ASML even agree to this? And I'm like, I don't think so, right?

**Dwarkesh:**
[(1:42:08)](https://podwise.ai/dashboard/episodes/7508210?locate=6128)
There's a world where they at least get the demand signal from that to increase production.

**Dylan Patel:**
[(1:42:12)](https://podwise.ai/dashboard/episodes/7508210?locate=6132)
Potentially, potentially, I agree.

**Dwarkesh:**
[(1:42:14)](https://podwise.ai/dashboard/episodes/7508210?locate=6134)
But it sounds like you're saying, oh, they couldn't even increase production if they wanted to, given the supply chain.

**Dylan Patel:**
[(1:42:18)](https://podwise.ai/dashboard/episodes/7508210?locate=6138)
Right, but that's exactly the market in which if they can't increase production,  just like TSMC cannot increase production that fast,  And yet demand is mooning,  then the obvious solution is to arbitrage this because you and I know demand is way higher than they're projecting and their capability to build. So then you arbitrage this by locking up the capacity and then sort of doing like a forward contract and then trying to sell it at a later date once other people realize,  actually, shit, everything is fucked and we don't have enough capacity. And then you'll have like this insane margin that ASML and TSMC should have been charging.

[(1:42:49)](https://podwise.ai/dashboard/episodes/7508210?locate=6169)
But the thing is, I don't know if ASML and TSMC will ever agree to this.

**Dwarkesh:**
[(1:42:52)](https://podwise.ai/dashboard/episodes/7508210?locate=6172)
Okay, let me ask about power now. So it sounds like you think power can be arbitrarily scaled.

**Dylan Patel:**
[(1:42:58)](https://podwise.ai/dashboard/episodes/7508210?locate=6178)
Not arbitrarily, but yes.

**Dwarkesh:**
[(1:43:00)](https://podwise.ai/dashboard/episodes/7508210?locate=6180)
But beyond these numbers. And I think, if I'm remembering correctly, your blog post on the power, how AI led to increasing power,  you were like, where you were implying that GeoVernova and Mitsubishi and Siemens could produce in gas turbines was like 60 gigawatts a year. And then there's these other sources, but they're like less significant than the turbines. And so And only a fraction of that goes to AI, I assume. So, yeah, if in 2030 we have enough logic and memory to do 200 gigawatts a year,  do you just think that these things are on a path to ramp up to more than 200 gigawatts a year or what do you see?

**Dylan Patel:**
[(1:43:38)](https://podwise.ai/dashboard/episodes/7508210?locate=6218)
Yeah. So, I mean, right now we're at 30, right? Or 20, 20, 20. So, this is critical IT capacity, by the way, right? This is an important thing to mention. When I'm talking about these gigawatts, I'm talking about critical IT capacity, server plugged in,  that's how much power it pulls. But there's losses along the chain, right? There is a loss on the transmission. There's losses on the conversion. There's losses on cooling, et cetera. And so you should gross this factor up from 20 gigawatts for this year or 200 gigawatts by the end of the decade to some number 20,  30% higher. And then you have capacity factors, right? Turbines don't run at 100%.

[(1:44:12)](https://podwise.ai/dashboard/episodes/7508210?locate=6252)
In fact, if you look at PGM, which is the largest grid, I think,  in America, sort of the Midwest or Northeast kind of area-ish. Not the full Northeast, but anyways, PJM, they rate in their models for like,  hey, turbines, how much capacity we want to have excess, you know, roughly 20% capacity. In addition, in that 20% excess capacity, we're running all the turbines at 90% because they are derated some for reliability,  all things go down, maintenance, et cetera, et cetera, et cetera. So then in reality,  the nameplate capacity for energy is always way higher than the actual end critical IT capacity because of all of these factors. But it's not just turbines, right?

[(1:44:50)](https://podwise.ai/dashboard/episodes/7508210?locate=6290)
If you're just making power from turbines, like that's simple, boring, easy, right? Humans and capitalism is far more effective. And so the whole point of that blog was, yes,  there's only three people making combined cycle gas turbines,  but there's so much more we can do, right? We can do aeroderivatives, right? We can take airplane engines and turn them into turbines as well. And there's even new entrants in the market, like Boom Supersonics trying to do that, right? And they're working with Crusoe. And also there's all the other ones that already exist in the market. There's There's medium speed reciprocating engines, right? Engines that spin in circles, right?

[(1:45:24)](https://podwise.ai/dashboard/episodes/7508210?locate=6324)
So sort of like any diesel engine, right? There's like 10 people who make engines that way, right? So Cummins, you know, you know, at least I'm from Georgia and we, you know,  people used to be like, oh man, you got a Cummins engine in there. You know, like, you know, regarding Ram trucks, but it's like, well, actually auto, Automobiles, manufacturing is going down. These companies all have capacity and could scale and convert that for data center power, right? Stick all these reciprocating engines. Yes, it's not as clean as combined cycle. Maybe you can convert them from diesel to gas if you want. But at the end of the day, these spinning engines, oh, what about ship engines, right?

[(1:45:55)](https://podwise.ai/dashboard/episodes/7508210?locate=6355)
All of these engines for these massive cargo ships. Those are great. Nebius is doing that for a data center for Microsoft in New Jersey, right? They're running these ship engines to generate power. Oh, there's, you know, Bloom Energy is doing fuel cells. We've been like very positive on them for like a year and a half now because they have like such a capability to increase their production and their payback period for production increase is like very fast,  even if the cost is a little bit higher than combined cycle,  which is like the best cost and efficiency. And then there's solar plus battery, which as these cost curves continue to come down, those can come online. There's wind.

[(1:46:30)](https://podwise.ai/dashboard/episodes/7508210?locate=6390)
And of course, the derating of those, hey, when you put on a wind turbine,  you might say, oh, I'm only going to expect 15% of the maximum power because things just oscillate. But yeah, batteries, there's all these things. And then the other thing is that the grid is scaled for, hey,  we're not going to cut off power at peak usage,  which is like the hottest day in the summer. But in reality, that's a load spike that is 10, 15, 20 percent higher than the average. Well, if you just put enough utility scale batteries,  or you put peaker plants that only run a small portion of the year,  then all of a sudden, you know, and those could be gas, they could be industrial gas turbines,

[(1:47:06)](https://podwise.ai/dashboard/episodes/7508210?locate=6426)
 they could be combine cycle, they could be any of the other sources of power I mentioned,  they could be batteries, then all of a sudden,  you've unlocked 20% of the US grid for data centers,  because most of the times that capacity is sitting idle,  and it's really only there for that peak,  right, which is a day or two. And it's a few hours of like maybe a few days of the full year is that peak. And so you just have enough capacity to absorb that peak load. And all of a sudden you've transferred all. And today, data centers are only three, 4% of the power of the US grid. And by 28, there'll be 10%. But if you can just unlock 20% of the US grid like this, it's not that crazy.

[(1:47:42)](https://podwise.ai/dashboard/episodes/7508210?locate=6462)
And the US grid is terawatt level, not hundreds of gigawatts level. So we can add a lot more energy. It's not easy. I'm not saying it's easy. These things are going to be hard. There's a lot of hard engineering. There's a lot of risks that people have to take. There's a lot of new technologies people have to use. But Elon was the first to do this behind the meter gas. And since then, we've seen an explosion of different things that people are doing to get power. And they're not easy, but people are going to be able to do them. And the supply chains are just way more simple than chips.

**Dwarkesh:**
[(1:48:15)](https://podwise.ai/dashboard/episodes/7508210?locate=6495)
Interesting. So I guess he made the point during the interview that the specific blade for the specific turbine he was looking at,  the lead times for that go out beyond 2030. And your point is that.

**Dylan Patel:**
[(1:48:25)](https://podwise.ai/dashboard/episodes/7508210?locate=6505)
That's great. There's so many other ways to make energy. OK, so just be inefficient like it's fine.

**Dwarkesh:**
[(1:48:29)](https://podwise.ai/dashboard/episodes/7508210?locate=6509)
Right. So you're like right now, I guess, combined cycle gas turbines have cap backs of $1,500 per kilowatt. And you're saying you could just it would make sense to have either technologies that are much more expensive than that or other things are getting cheap enough to that to make it competitive.

**Dylan Patel:**
[(1:48:43)](https://podwise.ai/dashboard/episodes/7508210?locate=6523)
Exactly, exactly. You know, it can be as high as $3,500 per kilowatt even. Right. So it could be twice as much as the cost of combined cycle. And the total cost of the GPU on a TCO basis has gone up a few cents per hour. Again, because we've been talking about hopper pricing, $1.40 now becomes, oh, the power price doubles? Okay, the hopper that was $1.40 is now $1.50 in cost. Oh,  I don't care because the models are improving so fast that the marginal utility of them is worth way more than that 10% increase in energy.

**Dwarkesh:**
[(1:49:18)](https://podwise.ai/dashboard/episodes/7508210?locate=6558)
Okay. And then so you're saying 20% of the grids, one terawatt about,  20% of that can just come online from utility scale batteries increasing what you'd be comfortable putting on the grid.

**Dylan Patel:**
[(1:49:30)](https://podwise.ai/dashboard/episodes/7508210?locate=6570)
The regulatory mechanism there is like not easy, by the way.

**Dwarkesh:**
[(1:49:32)](https://podwise.ai/dashboard/episodes/7508210?locate=6572)
But like that's 200 gigawatts, like if that hypothetically happens. But you're saying on just from the different sources of gas generation you mentioned,  the different kinds of engines and turbines, combined,  how many gigawatts could they unlock by the end of the decade?

**Dylan Patel:**
[(1:49:46)](https://podwise.ai/dashboard/episodes/7508210?locate=6586)
Yeah. So we're tracking in some of our data where there's over 16 different manufacturers of power generating things just from gas alone. So, yes, there's only three turbine manufacturers for a combined cycle,  but we're tracking 16 different vendors and we have all of their orders and things like that. And it turns out there is just hundreds of gigawatts of orders to various data centers. As we get to the end of the decade,  we think like something like half of the capacity that's being added will be behind the meter. And when we look at like a lot of this is actually behind the meter is almost always more expensive than grid connected,

[(1:50:21)](https://podwise.ai/dashboard/episodes/7508210?locate=6621)
 but there's just a lot of problems with getting grid connected and permits and interconnection queues and all this sort of stuff. So it ends up being even though it's more expensive, people are doing behind the meter. And then what they're doing behind the meter with ranges widely, right? It could be reciprocating engines. It could be ship engines. It could be aero derivatives. It could be combined cycle, although combined cycle is not that great for behind the meter. It could be bloom energy fuel cells. It could be solar plus battery, right? Like it could be any of these things.

**Dwarkesh:**
[(1:50:47)](https://podwise.ai/dashboard/episodes/7508210?locate=6647)
You're saying any of these individually could do like tens of gigawatts?

**Dylan Patel:**
[(1:50:51)](https://podwise.ai/dashboard/episodes/7508210?locate=6651)
Any of these individually will do tens of gigawatts and in a whole they will do hundreds of gigawatts. Okay, so that that alone should more than I mean, it's going to take I mean,  like electrician wages probably double or triple again, right? And like, there's gonna be a lot of new people entering that field. And there's gonna be a ton of people who make money. But it is something that I don't, like, I don't see that as the main bottleneck, right?

**Dwarkesh:**
[(1:51:11)](https://podwise.ai/dashboard/episodes/7508210?locate=6671)
So right now in Abilene, the 1.2 gigawatt data center that Chris is building for OpenAI,  I think they have like 5,000 people working there or at peak they did. And if you turn that into A hundred gigawatts,  and I'm sure things will get more efficient over time,  but that would be like 400K people it would take to build a hundred gigawatts. And if you think about the US labor force of how many electricians there are,  how many construction workers there are, yeah, I guess there's like 800K electricians. I don't know if they're all substitutable in this way. There's millions of construction workers, but if we're in a world where we're adding 200 gigawatts a year,

[(1:51:51)](https://podwise.ai/dashboard/episodes/7508210?locate=6711)
 Are we going to be crunched on labor eventually,  or do you think that is actually not a real constraint?

**Dylan Patel:**
[(1:51:56)](https://podwise.ai/dashboard/episodes/7508210?locate=6716)
So labor is a humongous constraint in this. People have to be trained. Likewise, we probably start importing the highest skilled at labor in this in this way, right? Because now it makes sense that, you know, hey,  a really high skilled electrician in Europe who I was working on destroying power plants,  now comes to America and is building data center, you know, high voltage electricity,  you know, power, moving across data center, right? Something like this, right? Humanoid robots maybe start to, or robotics at least start to,  but the main factor is going to be for reducing the number of people is modularizing things and making them in factories in Asia.

[(1:52:31)](https://podwise.ai/dashboard/episodes/7508210?locate=6751)
Unfortunately, but you know, at least for America, but You know, Korea, Southeast Asia,  and in many ways, China as well. But, you know, these areas are going to do,  are going to ship more and more built out,  built out sections of the data center. And those will be shipped in, right? Maybe today you, you know, you currently ship servers in or a rack in and then you plug that into you know,  different pieces that you're shipping from different places,  but now you'll ship it to a factory and integrate the entire,  you know, hey, maybe this is a two megawatt block. And this block goes from, you know, high voltage power to, uh, the, you know,  the voltage power that you, the voltage and, uh,

[(1:53:14)](https://podwise.ai/dashboard/episodes/7508210?locate=6794)
 and maybe DC that you deliver to the rack,  um, instead of being AC and high voltage, right. Or something like this, right. Or cooling, you take You ship a fully integrated thing that has a lot of the cooling subsystems already put together,  or because plumbers are also a big constraint here, or furthermore,  you take instead of just a single rack,  and now you have people wiring up all these racks of power and electricity and blah,  blah, blah, blah, blah, you take a skid and you put an entire row of servers,  and that is shipped from the factories. And today, a single rack may be 120, 140 kilowatts, but as we get to next generation,  Nvidia Kyber and things like that, it's almost a megawatt.

[(1:53:53)](https://podwise.ai/dashboard/episodes/7508210?locate=6833)
And then in addition, if you do an entire row, it'll have the rack,  it'll have the networking and it'll have the cooling and the power racks all integrated together. So now when you come in, actually you have much less stuff to cable,  whether it be networking with a fiber, whether it be The power, right? There's fewer power things to connect. And then there's fewer plumbing things to connect, right? And so this drastically can reduce the amount of people working in data centers. And therefore, the capability to build these will be much larger. And along the way, there will be, you know, new things mean, you know,  some people move faster to new things, some people move slower, right?

[(1:54:28)](https://podwise.ai/dashboard/episodes/7508210?locate=6868)
Crusoe and Google have been talking a lot about this modularization,  as has people like Meta and many others have been talking a lot about this modularization. Others are going to be slower to doing it, but at the end of the day,  And people who move faster to new things may have more delays or people who are slower have labor problems. So there will always be dislocations in the market because this is a very complex supply chain. At the end of the day,  it's still simple enough that we will be able to solve it through capitalism and human ingenuity on the time scales that are required.

**Dwarkesh:**
[(1:54:57)](https://podwise.ai/dashboard/episodes/7508210?locate=6897)
Yeah. Okay. So speaking of big problems to solve, Elon Musk is very bullish on space GPUs. If you're right, that power is not a constraint on Earth. I guess the other reason they would make sense is that even you can,  there is enough, there'll be enough gas turbines or whatever to build it on Earth. I think Elon's next argument then is like, you can't get the permitting to build hundreds of gigawatts on Earth. Do you buy that argument?

**Dylan Patel:**
[(1:55:21)](https://podwise.ai/dashboard/episodes/7508210?locate=6921)
Land-wise, America's big. Data centers don't take that much space. You can solve that. Permitting-wise, air pollution permits are a challenge, but the Trump administration's made it much easier. You go to Texas and you can skip a lot of this red tape. Elon had to deal with a lot of this complex stuff in Memphis and then building a power plant across the border and all these things for Colossus 1 and 2. But at the end of the day, there's a lot more you can get away with in the middle of Texas,  right?

**Dwarkesh:**
[(1:55:50)](https://podwise.ai/dashboard/episodes/7508210?locate=6950)
Well, given that Elon lives in Texas, why didn't he just go to Texas?

**Dylan Patel:**
[(1:55:53)](https://podwise.ai/dashboard/episodes/7508210?locate=6953)
I think it was partially like they over-indexed on grid power for a temporary period of time, right? Because that's just what they thought they needed more of.

**Dwarkesh:**
[(1:56:01)](https://podwise.ai/dashboard/episodes/7508210?locate=6961)
You said an aluminum refinery connected to the grid there.

**Dylan Patel:**
[(1:56:03)](https://podwise.ai/dashboard/episodes/7508210?locate=6963)
It was an appliance factory that was idled. But I think they may have indexed more to what was grid power. They may have indexed more to water access and gas access. Actually, I think they bought that knowing that the gas line was right there and they were going to tap it. Same with water. It was a whole host of different constraints. It was probably an area where electricians and things like that were easier to find. But at the end of the day, I'm not exactly sure why they chose that site. I bet Elon would have chosen somewhere in Texas if he could have gone back. But because of the regulatory challenges he's faced, It's ultimately like permitting is a challenge,

[(1:56:42)](https://podwise.ai/dashboard/episodes/7508210?locate=7002)
 but America is a big place and there are 50 states and things will get done. And there are a lot of small jurisdictions where you can just transport in all the workers that you need for a temporary period of six months to a year,  depending on the type of contractor. It can be even three months for depending on the type of contractor that's coming in and put them in temporary housing,  pay out the butt because labor is very cheap relative to the GPUs and the power or not the power,  but the GPUs and the like. The networking and so on and so forth and the end value of the tokens it's going to produce. So all of these things have plenty of room to be paid for. And so I think it's fine, right?

[(1:57:18)](https://podwise.ai/dashboard/episodes/7508210?locate=7038)
And also people are diversifying now, right? Australia, Malaysia, Indonesia, India, these are all places where data centers are going up at a much faster pace,  but currently still 70% plus of the AI data centers are in America and that continues to be the trend. And so I think people are figuring out how to build these things and permitting like I just like ultimately like permitting and red tape in middle of nowhere,  Texas or middle of nowhere,  Wyoming or middle of nowhere like New Mexico is probably a hell of a lot easier than sending stuff into space.

**Dwarkesh:**
[(1:57:49)](https://podwise.ai/dashboard/episodes/7508210?locate=7069)
Right. Well,  other than the fact that the economic argument makes less sense once you consider the fact that energy is a small fraction of the cost of ownership of a data center. What are the other reasons you're skeptical?

**Dylan Patel:**
[(1:57:59)](https://podwise.ai/dashboard/episodes/7508210?locate=7079)
Yeah. So obviously power's free in space, basically.

**Dwarkesh:**
[(1:58:03)](https://podwise.ai/dashboard/episodes/7508210?locate=7083)
That's the reason to do it.

**Dylan Patel:**
[(1:58:04)](https://podwise.ai/dashboard/episodes/7508210?locate=7084)
Yeah. That's the reason to do it. But then there's all the other counter arguments, right? Because even if power costs double, you're still at a fraction of the total cost of the GPU. The main challenges is, and what we've seen that disperses, right? We have ClusterMax, which rates all the Neo clouds and we test them. We test over 40 cloud companies, including the hyperscalers and Neo clouds. What differentiates some of these clouds the most outside of software is their ability to deploy and manage failure, right? GPUs are horrendously unreliable. Even today, 15% of black wells or so that get deployed have to be RMA'd. You have to take them out.

[(1:58:40)](https://podwise.ai/dashboard/episodes/7508210?locate=7120)
You have to, you know, maybe just plug them and plug them back in,  but sometimes you have to take them out and ship them to Nvidia or rather their partners who do these RMAs and such.

**Dwarkesh:**
[(1:58:47)](https://podwise.ai/dashboard/episodes/7508210?locate=7127)
What do you make of Jelenskiy's argument that once you have the initial After an initial phase,  they actually don't fail that much.

**Dylan Patel:**
[(1:58:53)](https://podwise.ai/dashboard/episodes/7508210?locate=7133)
Sure. But now you've done this, you've tested them all, you deconstructed them, put them on a spaceship,  fucking put them into space, and then put them online again. That's months, right? And if your argument is that, you know, hey, GPUs have a useful life of X years, right? If a GPU has a useful life of five years, and it takes three additional months,  probably six, let's say six additional months, then that is 10% of your cluster's useful life. And because we're so capacity constrained, that compute is most valuable Theoretically, in the first six months,  you have it because we're more constrained now than in the future,

[(1:59:30)](https://podwise.ai/dashboard/episodes/7508210?locate=7170)
 because that compute now can contribute to a better model in the future or contribute to revenue now,  which you can use to raise more money to get back, you know, all these sorts of things. Now is always the most important moment. And so you've delayed your compute deployment by six months, potentially. And the thing that separates these clouds is we see clouds that take six months to deploy GPUs today on Earth,  right? We see clouds that take a lot less than six months, right? And so the question is, where does space get in there? I don't see how you would test them all on Earth, deconstruct them and ship them into space,

[(1:59:59)](https://podwise.ai/dashboard/episodes/7508210?locate=7199)
 and it not take longer than just putting them in the spot that you're testing them.

**Dwarkesh:**
[(2:00:03)](https://podwise.ai/dashboard/episodes/7508210?locate=7203)
Yeah. So the question I wanted to ask is the topology of space communication. Right now, Starlink satellites talk to each other at 100 gigabits per second. And you could imagine that being much higher with optical inner satellite laser links that are optimized for this. And that actually ends up being quite close to the InfiniBand bandwidth, which is like 400 gigabytes a second, right?

**Dylan Patel:**
[(2:00:28)](https://podwise.ai/dashboard/episodes/7508210?locate=7228)
That's per GPU, not per rack.

**Dwarkesh:**
[(2:00:30)](https://podwise.ai/dashboard/episodes/7508210?locate=7230)
I see. Okay.

**Dylan Patel:**
[(2:00:31)](https://podwise.ai/dashboard/episodes/7508210?locate=7231)
So multiply that by 72. Also, that was Hopper when you go to Blackwell and Rubin, that 2Xs and 2Xs again.

**Dwarkesh:**
[(2:00:38)](https://podwise.ai/dashboard/episodes/7508210?locate=7238)
All right. But how much compute is happening per, like during inference,  are the different scale ups still working together or is it just happening,  it's a batch within a single scale up?

**Dylan Patel:**
[(2:00:49)](https://podwise.ai/dashboard/episodes/7508210?locate=7249)
A lot of models fit within one scale up domain,  but many times you split them across multiple scale up domains. I think that You really have to, as models become more and more sparse,  at least this is like the general trend,  then you want to ping just a couple experts per GPU. And if leading models today have hundreds, if not thousand experts,  then you'd want to run this across hundreds of chips or thousands of chips,  even as we continue to advance into the future. And so then you end up with this problem of Well,  now you need to connect all these satellites together comms wise as well.

**Dwarkesh:**
[(2:01:27)](https://podwise.ai/dashboard/episodes/7508210?locate=7287)
Okay, so that would be tough. Because I was imagining if there's a world where you could like do a batch,  inference for a batch on a single scale up, then maybe it's more plausible. But if not, then it's...

**Dylan Patel:**
[(2:01:40)](https://podwise.ai/dashboard/episodes/7508210?locate=7300)
Yeah, I mean, networking these chips together is a problem. And you can't just make this satellite infinitely large, right? Like there are a lot of challenges with physics to making a satellite really big, right? So then that's why you need these interconnects between the satellites, those interconnects are more expensive than the,  you know, a cluster like 20% of the cost or 15% of the cost is networking. All of a sudden now you're making it like space lasers instead of like pretty simple,  like lasers that are manufactured in millions of volumes with, you know, pluggable transceivers. And those things are very unreliable as well. More unreliable than the GPUs, by the way.

[(2:02:13)](https://podwise.ai/dashboard/episodes/7508210?locate=7333)
Across the life of a cluster, you have to unplug, clean it all the time, right? Unplug, replug it just for random reasons. These things are just not as reliable. So you've got that also, that problem as well. Like you've got a more expensive, complicated space laser to communicate instead of this pluggable optical transceiver that's been in super high volume.

**Dwarkesh:**
[(2:02:29)](https://podwise.ai/dashboard/episodes/7508210?locate=7349)
Okay. So all in all, what does that imply for space data centers?

**Dylan Patel:**
[(2:02:32)](https://podwise.ai/dashboard/episodes/7508210?locate=7352)
So space data centers effectively are not limited by, you know, hey, we have this energy advantage. It's actually just limited by the same contended resource. We can only make 200 gigawatts of chips a year by the end of the decade. So what are we going to do to get that capacity? It doesn't matter if it's on land or in space. It doesn't really matter because you can build that power. I think human capabilities and capacity could get to the period where we're adding a terawatt a year globally of various types of power. At some point, we do cross the chasm where space data centers make sense, but it's not this decade.

[(2:03:11)](https://podwise.ai/dashboard/episodes/7508210?locate=7391)
It is much further out once you have Energy constraints actually being a big bottleneck once you have space,  land permitting be a much bigger bottleneck as it subsumes more and more of the economy. And chips are no longer the bottleneck because chips are the biggest bottleneck. And so you want them deployed working on AI the moment they're done being manufactured. And so there's a lot of things people are doing to increase that speed faster and faster,  whether it be modulizing data centers or even modulizing racks where you actually put the chip in At the data center,  but only the chip and everything else is already wired up and ready to go at the data center.

[(2:03:47)](https://podwise.ai/dashboard/episodes/7508210?locate=7427)
So there's things like this that people are doing to decrease that time that you cannot do in space. And at the end of the day, all that matters in a chip-constrained world is get these chips working on producing tokens ASAP in a world,  you know, maybe 2035, once the semiconductor industry and ASML and ZEISS and all these other suppliers,  land research applied materials, fab manufacturers, like pendulum swings, and are able to make enough chips. And really, we're optimizing every dial. And like, it makes sense to optimize the 10% of energy costs, or 15% of energy costs,  or as we move to a six, potentially, and Nvidia's margins aren't 70 plus percent,

[(2:04:25)](https://podwise.ai/dashboard/episodes/7508210?locate=7465)
 maybe that energy cost is 30% of the cluster, and fab construction, all this,  like these are the things are data center,  these are the things to optimize. But that's not a, you know, Elon doesn't win by doing You know, 20% gains. Elon never wins that way. Elon wins when he swings for the fences and does 10x gains, right? That's what SpaceX is about. That's what Tesla was about. That's what all of his success has been about, right? It's not been about chasing the 20%. So I think space data centers will eventually be a 10x gain, potentially,  as Earth's resources get more and more contentious. But that's not this decade.

**Dwarkesh:**
[(2:04:58)](https://podwise.ai/dashboard/episodes/7508210?locate=7498)
Yeah. I mean, I think just to drive some intuition about how much land there is on Earth,  Obviously, the chips themselves, especially if we move to a world where you have racks that have megawatts,  like literally, it's not even a variety factor.

**Dylan Patel:**
[(2:05:11)](https://podwise.ai/dashboard/episodes/7508210?locate=7511)
That's the other thing, right? The power dense, you know, if chips and manufacturing is the constraint, right now,  roughly, it's one watt per millimeter squared for AI chips and such. One easy way is to pump that to 2 watts per millimeter squared. Now, you may not get 2x the performance. You may only get 20% more performance, and that requires much more exotic cooling, right? It requires more complicated cold plates and very complicated liquid cooling, or maybe it requires things like emergent cooling. But in space, higher watts per millimeter is very difficult, whereas on Earth, these are solved problems. And one of these things enables you to get a lot more tokens, maybe it's 20% more tokens,

[(2:05:47)](https://podwise.ai/dashboard/episodes/7508210?locate=7547)
 per wafer that's manufactured. And that's a humongous way.

**Dwarkesh:**
[(2:05:50)](https://podwise.ai/dashboard/episodes/7508210?locate=7550)
So millimeter you mean of die area?

**Dylan Patel:**
[(2:05:52)](https://podwise.ai/dashboard/episodes/7508210?locate=7552)
Yeah, of die area, square millimeters of a die area.

**Dwarkesh:**
[(2:05:55)](https://podwise.ai/dashboard/episodes/7508210?locate=7555)
I mean,  it would be better for space because if you can run more watts per millimeter would be the chip runs hotter and the hotter the chip. I guess this is a question of the computer chip engineering,  but it like it cools to the power of four by Stefan Boltzmann's law. So if you can run a very hot chip because it allows a lot of...

**Dylan Patel:**
[(2:06:10)](https://podwise.ai/dashboard/episodes/7508210?locate=7570)
You can't run it hotter, you can only run it denser. And the problem is getting the heat out of that dense area means you have to move away from standard air cooling and liquid cooling to more exotic forms of liquid cooling or even immersion to get to higher power densities. And that's more difficult in space than it is on Earth.

**Dwarkesh:**
[(2:06:27)](https://podwise.ai/dashboard/episodes/7508210?locate=7587)
And maybe it's at this point worth explaining what exactly a scale-up is and what it looks like for Nvidia versus Tranium versus TPUs.

**Dylan Patel:**
[(2:06:38)](https://podwise.ai/dashboard/episodes/7508210?locate=7598)
Yeah. So earlier I was mentioning how communication within a chip is super fast. Communication within chips that are in the same rack is fast, but it's not as fast. And then, you know, it's on the order of terabytes. And then communication very far away is on the order of gigabytes, hundreds of gigabytes, right? So this, this order of magnitude, as you get further distance, compute, and maybe across the country,  it's on the order of gigabytes a second, right? Scale up domain is this like tight domain where the chips are communicating on the order of terabytes a second. And so for Nvidia, previously,

[(2:07:11)](https://podwise.ai/dashboard/episodes/7508210?locate=7631)
 this meant an H100 server had eight GPUs and those eight GPUs could talk to each other at terabytes a second. With Blackwell and VL72, they implemented rack scale up. And that meant all 72 GPUs in the rack could connect to each other at terabytes a second speed. And the speed doubled gen on gen, but also the most important innovation they did was going from eight to 72 in the domain. When we look at Google, their scale-up domain is completely different, right? It has always been on the order of thousands, right? With TPU v4, they had pods the size of 4,000 chips. With v8, they have pods, or v7, they have pods in the 7,000, or sorry, 8,000, 9,000 range.

[(2:07:49)](https://podwise.ai/dashboard/episodes/7508210?locate=7669)
And what's relevant here is that it's not the same as Nvidia. It's not like for like. Google has a topology that's a torus, right? So every chip connects to six neighbors. Rather than Nvidia, the 72 GPUs connect all to all, right? So they can send terabytes a second to each other,  to any arbitrary other chip in that pod of scale up. Whereas Google, you have to bounce through chips, right? So this means if TPU 1 needs to talk to TPU 76, then it has to bounce through various chips. And there is always some blocking of resources when you do that. So because that one TPU is only connected to six other TPUs.

[(2:08:23)](https://podwise.ai/dashboard/episodes/7508210?locate=7703)
And so there's a difference in topology and bandwidth, and there are trade-offs and advantages of both, right? Google gets to have a massive scale-up domain. But then they have the trade-off of you have to bounce across chips to get from one chip to another. You can only talk to six direct neighbors. And so there is this trade-off. And Amazon has mutated their scale-up domain. They're somewhere in between Nvidia and Google, effectively, where they're trying to make larger scale-up domains. They try and do all-to-all to some extent with switches, which is what Nvidia does. But also, to some extent, they use tourist topologies like Google does. And as we as we advance forward to next generations,

[(2:08:59)](https://podwise.ai/dashboard/episodes/7508210?locate=7739)
 all three of them are moving more and more towards a dragonfly topology,  which means there's sort of like there is some fully connected elements and there's some elements that are not fully connected. So you can get the scale up to be hundreds or thousands of chips,  but also have it not contend for resources when you're bouncing through chips.

**Dwarkesh:**
[(2:09:15)](https://podwise.ai/dashboard/episodes/7508210?locate=7755)
Related question. I heard somebody make the claim that the reason that parameter scaling has been slow and only now are we getting bigger and bigger models from OpenAI and Anthropic is that So original GPT-4 is over a trillion parameters and only now are models starting to approach that again. And I heard a theory. The reason is that Nvidia's scale ups have just not had that much memory capacity. And so What was the claim exactly? Let's say you have a 5T model running at FP8. So that's 5 trillion gigabytes. And then you have the KV cache. Let's say it's the same size for one batch. So you need 10 gigabytes, sorry, 10 terabytes to be able to run a single forward pass.

**Dylan Patel:**
[(2:10:14)](https://podwise.ai/dashboard/episodes/7508210?locate=7814)
Yeah.

**Dwarkesh:**
[(2:10:14)](https://podwise.ai/dashboard/episodes/7508210?locate=7814)
And then only with the GB200 and VL72 do you have an Nvidia scale up that has 20 terabytes. And before that, they were much smaller. Whereas Google, on the other hand, has had these huge TPU pods that are not all to all,  but still have, I think, hundreds of terabytes of capacity in a single scale up. So does that explain why parameter scaling has been slow?

**Dylan Patel:**
[(2:10:35)](https://podwise.ai/dashboard/episodes/7508210?locate=7835)
I think it's partially the capacity and bandwidth,  but also As you build a larger model,  the ability to deploy it is slower, right? Like in terms of like, hey, what is the inference speed for the end user? That's kind of irrelevant. What's really relevant is RL. And what we've seen with these models and allocation of compute at a lab is sort of there's a few main ways you can allocate compute. You can allocate it to inference, i.e. revenue. You can allocate it to development, i.e. making the next model, and you can allocate it to research. And in development specifically, you split it between pre-training and RL, right? And so when you think about, hey, what exactly is happening?

[(2:11:14)](https://podwise.ai/dashboard/episodes/7508210?locate=7874)
Well, the model, the compute efficiency gains you get from research are so large,  you actually want most of your compute to go to research, not to development,  because, you know, all these researchers are generating new ideas, trying them out, testing them. And continuing to march along this and push the Pareto optimal curve of scaling laws further and further and further. And at least what we've seen empirically is like model cost gets 10x cheaper every year or even more than that,  which at the same scale gets 10x cheaper or to reach new frontiers, it costs the same amount or more,  right? So you don't want to allocate too many resources to pre-training and RL.

[(2:11:52)](https://podwise.ai/dashboard/episodes/7508210?locate=7912)
You actually want to allocate most of your resources to research. And then in the middle is this development period. If you pre-train a 5 trillion parameter model, Now you have to spend all this time. How many rollouts do you have to do in these RLs? And these rollouts for a trillion parameter model versus a five trillion parameter model are five times larger,  which then means it takes, if you wanted to do as many rollouts,  maybe the larger model is more sample efficient. Let's say it's two X more sample efficient. Okay, great. Now you need two and a half X much time of RL to get the model smarter.

[(2:12:24)](https://podwise.ai/dashboard/episodes/7508210?locate=7944)
Or you could RL the smaller model for 2X the time and you'd still have a 25% difference in the big model,  which is 2X more sample efficient and doing X number of rollouts versus the small model,  which is a trillion parameters, although it's less sample efficient, is doing twice as many rollouts. It's still done faster. And so you get the model faster, sooner, and you've done more RL,  and then you can take that model to help you build the next models,  help your engineers train and do all these research ideas. And so this feedback loop is actually weighed towards smaller models in every case, no matter what your hardware is.

[(2:12:59)](https://podwise.ai/dashboard/episodes/7508210?locate=7979)
And then as you look to Google, Google does deploy the largest production model of any of the major labs,  right, with Gemini Pro. It is a larger model than GPT-54. It's a larger model than Opus. And so you end up with, yes, Google does this because they have a unipolar set of compute,  almost all TPU. Whereas Anthropic is dealing with H100s, H200s, Blackwell, Traniums, TPUs of various generations, right? And OpenAI is dealing with mostly Nvidia right now, but going towards having AMD and Tranium as well. The fleets of compute like Google can just optimize around a larger model and they can leverage a thousand chips in a scale-up domain to get the RL speed much faster.

[(2:13:49)](https://podwise.ai/dashboard/episodes/7508210?locate=8029)
So that you can actually have this feedback loop be fast. But at the end of the day, in isolation,  you almost always want to go with a smaller model that gets RL'd faster and gets deployed into research and development. So you can build the next thing and get more compute efficiency wins. And then this compounding effect of, oh, I made a smaller model that I RL'd more that I then deployed into research and development earlier. And I spent less compute on the training itself because I was able to allocate more compute to the research. This, like, compounding effect of being able to do the research faster and faster and faster is potentially a faster takeoff.

[(2:14:21)](https://podwise.ai/dashboard/episodes/7508210?locate=8061)
And that's all these companies want, is fastest takeoff possible.

**Dwarkesh:**
[(2:14:24)](https://podwise.ai/dashboard/episodes/7508210?locate=8064)
Okay. Spicy question. You know, you're explaining, you make the, SME Analysis sells these spreadsheets and you're always like,  ah, six months ago or a year ago, you told people the memory crunch,  or now you're telling people the cleanroom crunch, and then in the future, the tool crunch. Why is Leopold the only person that is using your spreadsheets to make outrageous money? What is everybody else doing?

**Dylan Patel:**
[(2:14:48)](https://podwise.ai/dashboard/episodes/7508210?locate=8088)
I think there are a lot of people making money In many ways, I think obviously Leopold,  Leopold jokes that, you know, he's the only client of mine that tells me our numbers are too low. Everyone else tells me our numbers are too high, almost ad nauseum. You know, whether it's a hyperscaler saying, hey, that other hyperscaler, their numbers are too high,  you know, and we're like, nah, that's it. And they're like, no, no, no, no, it's impossible, blah, blah, blah. And then you're like,  finally have to convince them through all these facts and data when we're working with hyperscalers or AI labs that in fact,  no, that number isn't too high. That's correct.

[(2:15:18)](https://podwise.ai/dashboard/episodes/7508210?locate=8118)
But eventually, sometimes it's like six months later, it takes them to realize or a year later. I think other clients on the trading side also use our data, right? We sell data to a lot of, I think roughly 60% of my business is industry. So AI labs, data center companies, hyperscalers, Semiconductor companies, the whole supply chain across AI infrastructure. 40% of our revenue is hedge funds. I'm not going to comment on who our customers are, but I think a lot of people use the data. It's just how do you interpret it and then what do you view as beyond it? I will say Leopold is pretty much the only person who tells me my numbers are too low always. And sometimes he's too high. Sometimes I'm too low.

[(2:16:02)](https://podwise.ai/dashboard/episodes/7508210?locate=8162)
Right. But in general, I think other people are, you know, doing that. And you can check certain you can you can look across the space at hedge funds and look at the 13 apps and see actually they own. Maybe not exactly what Leopold does, because it's always like a question of like, what is the most constrained thing? What's the thing that's going to be that's most outside of expectations? And that's what you're really trying to exploit is inefficiencies in the market. And in a sense, what our data shows is, is,  is like making the market more efficient by making the base data of what's happening more accurate versus like,

[(2:16:34)](https://podwise.ai/dashboard/episodes/7508210?locate=8194)
 but in a sense, I think many, many funds do trade on information that is out there. And it's not, I don't think, I don't think Leopold's the only person. I think he has the most conviction on the entire, in the entire, like about the AGI takeoff though, right?

**Dwarkesh:**
[(2:16:51)](https://podwise.ai/dashboard/episodes/7508210?locate=8211)
Right. I mean, but the bets are not about like what happens in 2035.  The bets that you're making that are at least exemplified by public returns,  we can see for different funds, including Leopold's about what has happened in the last year. And the last year stuff could be predicted using your spreadsheets, right? So it's less about buying the next year's spreadsheets.

**Dylan Patel:**
[(2:17:11)](https://podwise.ai/dashboard/episodes/7508210?locate=8231)
They're not just spreadsheets. There's reports. There's API access to the data. There's a lot of data. But anyways, you know, I think...

**Dwarkesh:**
[(2:17:16)](https://podwise.ai/dashboard/episodes/7508210?locate=8236)
Do you see what I mean? It's not about some crazy singularity thing. It's about like, oh, do you buy the memory crunch?

**Dylan Patel:**
[(2:17:21)](https://podwise.ai/dashboard/episodes/7508210?locate=8241)
A simple one, though,  is like you only buy the memory crunch if you believe AI is going to take off in a huge way. And The memory crunch, a lot of it was predicated on like, you know,  at least for like people in the Bay Area who think about infrastructure, it's like obvious. KV cash explodes as context lenses go longer, so you need more memory. And then you do the math and you also have to have a lot of supply chain understanding of like what fabs are being built and what data centers are being built and how many chips and all these things. And so we track all these different data sets like very tightly, but at the end of the day,

[(2:17:51)](https://podwise.ai/dashboard/episodes/7508210?locate=8271)
 it takes, you know, Someone to fully believe that this is going to happen. I think a year ago,  if you told someone memory prices were quadruple and smartphone volumes are going to go down 40% over a year or two after that,  people were like, you're crazy. That never happened. Except a few people do believe that and those people did trade memory. And people did. I don't think like Leopoldo is the only person buying memory companies. I think there are a lot of people buying memory companies. He, of course, sized and positioned and did things in better ways than some. Maybe most, right? I don't want to comment on whose returns are what. But he certainly did well.

[(2:18:31)](https://podwise.ai/dashboard/episodes/7508210?locate=8311)
But other people also did really well, right? Wow, you've made me diplomatic for the first time ever. No, no, you're fine. I think it's hilarious, right? I'm being a diplomat, whereas usually I'm like spicy.

**Dwarkesh:**
[(2:18:44)](https://podwise.ai/dashboard/episodes/7508210?locate=8324)
Okay, maybe some rapid fire to close out. Can TSMC, if you're saying, look, the memory logic, et cetera,  the N3 is mostly going to be AI accelerators,  but then there's N2, which is mostly Apple now. And then in the future, I guess AI would also want to go on N2. Can they kick out Apple if Nvidia and Amazon and Google say, hey,  we're willing to pay a lot of money for N2 capacity?

**Dylan Patel:**
[(2:19:17)](https://podwise.ai/dashboard/episodes/7508210?locate=8357)
So I think the challenge of this is chip design timelines take a long while. And so that's more than a year. And the designs that are on two nanometer are more than a year out. And so what would really happen is Apple or sorry,  Nvidia and all these others will be like,  hey, we're going to prepay for the capacity and you're going to expand it for us. And then Apple would be, and maybe TSMC takes a little bit of margin, but not a ton. They're not going to kick Apple out entirely, right? What they're going to do is when Apple orders X, they may say, hey,  we project you only need Y or X minus one. And so that's what we're going to give you is X minus one.

[(2:19:49)](https://podwise.ai/dashboard/episodes/7508210?locate=8389)
And then that flex capacity Apple's kind of screwed on. Whereas traditionally Apple's always over-ordered by like 10% and cut back by 10% over the course of the year. And some years they hit the entire 10%, just, you know, volumes vary, right? Based on the season and macro, blah, blah, blah, blah, blah. And so I don't think TSMC would kick out Apple. I think Apple will become a smaller and smaller and smaller percentage of TSMC's revenue and therefore be less relevant for TSMC to cater to their demands. And TSMC could eventually start saying, hey,

[(2:20:18)](https://podwise.ai/dashboard/episodes/7508210?locate=8418)
 you've got to pre-book your capacity for next year for two years out and you have to pre-pay for the CapEx because that's what Nvidia and Amazon and Google are doing.

**Dwarkesh:**
[(2:20:26)](https://podwise.ai/dashboard/episodes/7508210?locate=8426)
Yeah, I wonder if it's worth going to specific numbers on like,  I don't have any of them on hand of like,  how many N2 wafers or what percentage of N2 does Apple have its hands on versus over the coming years versus AI?

**Dylan Patel:**
[(2:20:40)](https://podwise.ai/dashboard/episodes/7508210?locate=8440)
Yeah, I mean, this year, Apple has the majority of N2 that's going to get fabricated. There's a little bit from AMD. They are trying to make some AI chips and CPU chips early. There's a little bit, but for the most part, it's Apple. And as we go forward to the year after that,  Apple still gets closer to like half of it as other people start ramping. But then it falls drastically, right? Just like for N3, they were half. And when I say N2, that includes A16, which is a variant of N2. Over time, those nodes will be the majority. And what's also interesting is traditionally Apple has been the first to a process node. 2nm is actually the first time they're not. Well, besides Huawei, right?

[(2:21:23)](https://podwise.ai/dashboard/episodes/7508210?locate=8483)
Huawei back in 2020 and before was the first with Apple, but they were both making smartphones. Now with 2nm,  you've got AMD trying to make a CPU and a GPU chiplet that they used advanced packaging to package together in the same timeframe as Apple. And this is a big risk for AMD that causes potential delays, potentially, because it's a brand new process technology. It's hard. But at the end of the day, this is a bet that they want to do to scale faster than Nvidia and try and beat them. As we move forward, actually, when we move to the A16 node, the first customer there is not even Apple. It's AI. And as we move forward, that will become more and more prevalent.

[(2:22:02)](https://podwise.ai/dashboard/episodes/7508210?locate=8522)
Not only will Apple not be the first to a node,  they will also not be the majority of the volume to the new node. And then they'll just be like any old customer. And because the scale of TSMC's CapEx keeps ballooning,  but Apple's business is kind of not growing at the same pace,  they become a less and less relevant customer. And They also will just cut their orders because things in the supply chain are kicking them out,  whether it be packaging or materials or DRAM or NAND. These things are increasing in cost. They can't pass on all the cost to customers likely because the consumer is not that strong. And you end up with like this conundrum where they are just not Apple,

[(2:22:37)](https://podwise.ai/dashboard/episodes/7508210?locate=8557)
 TSMC's best bud like they have been historically.

**Dwarkesh:**
[(2:22:39)](https://podwise.ai/dashboard/episodes/7508210?locate=8559)
Do you think if Huawei had access to three nanometer, they would have a better accelerator than Rubin?

**Dylan Patel:**
[(2:22:44)](https://podwise.ai/dashboard/episodes/7508210?locate=8564)
Potentially, yeah. I think Huawei, they were the first with a 7nm AI chip as well. They were the first with a 5nm mobile chip, but they were the first with a 7nm AI chip. The Huawei Ascend was like two months before the TPU and like four months before Nvidia's,  I want to say, was it V100 or A100? A100, I think. And so, you know, I mean, that's just moving to a process. No, that doesn't imply software. It doesn't imply hardware design, all these other things. But Huawei is arguably the only company in the world that has all the legs, right? Huawei has cracked software engineers. Huawei has cracked networking technologies. That's in fact, their biggest business historically, right?

[(2:23:27)](https://podwise.ai/dashboard/episodes/7508210?locate=8607)
And they have cracked AI talent. But furthermore, beyond Nvidia, they actually have better AI researchers. And furthermore, beyond Nvidia, they have their own fabs. And furthermore, beyond Nvidia, they have their own end market of selling tokens and things like that. And Huawei They're able to get the top, top, top talent, Nvidia is as well, but not as much concentration. Huawei has a bigger pool in China. It's very arguable that Huawei, if they had TSMC, would be better than Nvidia. There are areas where China has advantages outside of In areas that Nvidia can't access as easily,  right, around not just scale, but also like some things around, you know, certain optical technologies,

[(2:24:10)](https://podwise.ai/dashboard/episodes/7508210?locate=8650)
 China's actually really good at. So there's certain, I think it's very reasonable that if in 2019 that issue that was not,  that Huawei was not banned from using TSMC,  Huawei had already eclipsed Apple as the biggest TSMC customer and Huawei has huge share in networking and compute and CPUs and all these things. They would have kept gaining share and they'd likely be TSMC's biggest customer.

**Dwarkesh:**
[(2:24:33)](https://podwise.ai/dashboard/episodes/7508210?locate=8673)
Wow, that's crazy. I've got kind of a random final question for you. So the other part of the Elon interview was robots. And so if humanoids take off faster than people expect, if by 2030, there's millions of humanoids running around,  which each need local compute, Any thoughts on what that implies? What will be required for that?

**Dylan Patel:**
[(2:24:55)](https://podwise.ai/dashboard/episodes/7508210?locate=8695)
There's a lot of difficulties with the VLMs and all these things that people,  VLAs that people are deploying on robots. But to some extent, you don't need to have all the intelligence in the robot. And it would be much more efficient to not do that, right? Because in the server, in cloud, you can batch process and all these things. So what you may want to do is, hey,  a lot of the planning and longer horizon tasks are determined by a much more capable model in the cloud that runs at very high batch sizes. And then it pushes those directions to the robots who then interpolate between each subsequent action or is given like,  hey, pick up that cup and then the model on the robot can pick up the cup.

[(2:25:35)](https://podwise.ai/dashboard/episodes/7508210?locate=8735)
And it's like, as it's picking up, it's like, oh, you know, in fact,  this, you know, you know, things like weight and all these things might have to be and like force may have to be like,  determined by the model on the robot, but not everything needs to be like,  you know, hey, pick up the robot, you know, this, right? Or like, hey, that's a headphone. Actually, I'm the supermodel in the cloud. I know that this headphones are, you know, Sony. XM6 is, which is not a Dwarkesh ad spot, but you know.

**Dwarkesh:**
[(2:26:00)](https://podwise.ai/dashboard/episodes/7508210?locate=8760)
I'm like, why is this guy plugging this thing so hard? It's like on the table. It's like on his neck when we're interviewing Satya together. Is he getting paid by Sony?

**Dylan Patel:**
[(2:26:09)](https://podwise.ai/dashboard/episodes/7508210?locate=8769)
Unfortunately not. Unfortunately not. But anyways, like, you know, it might say, hey,  the headband is soft and this is the weight of it and all these things. And then the model on the robot can be less intelligent and take these inputs and do the actions. And it may get told by the model in the cloud every second, every 10 times a second,  maybe, you know, it depends on the hertz of the action,  but a lot of that can be offloaded to the cloud. Because otherwise, if you do all of the processing on the device,  I believe it would be more expensive because you can't batch. Two, you couldn't have as much intelligence as you do in the cloud,  because the models will just be bigger in the cloud.

[(2:26:41)](https://podwise.ai/dashboard/episodes/7508210?locate=8801)
And three, we're in a semiconductor shortage world. And Any robot you deploy needs leading edge chips because the power is really bad for robots, right? You need it to be low power and efficient. And all of a sudden you're taking power and chips that would have been for AI data centers and you're putting them in robots. So now that 200 gigawatts gets lower if you're deploying millions of humanoids.

**Dwarkesh:**
[(2:27:02)](https://podwise.ai/dashboard/episodes/7508210?locate=8822)
I think this is very interesting because something people might not appreciate about the future is how centralized in a physical sense intelligence will be. Where right now with humans, There's 8 billion humans and their compute is on their heads, on their person. And in the future, even with robots that are out physically in the world,  I mean,  obviously knowledge work will be done in a centralized way from data centers with hundreds of thousands of instances or maybe millions of instances. But even for robotics,  the future you're suggesting is one where there's centralized thinking and centralized computation that's driving millions of robots out in the world.

[(2:27:42)](https://podwise.ai/dashboard/episodes/7508210?locate=8862)
And so I think that just like, yeah,  that's an interesting fact about the future that I think people might not appreciate.

**Dylan Patel:**
[(2:27:47)](https://podwise.ai/dashboard/episodes/7508210?locate=8867)
I think Elon recognizes this, which is why he's like, Going to different places for his chips, right? He signed this massive deal with Samsung to make his robot chips in Texas because he thinks,  you know, like I personally think he thinks that, you know, Taiwan risk is huge. And because of that and the centralization of resources in Taiwan,  him having his robot chips in Texas and also being a separate supply chain that is not as constrained by no one's making AI chips really on Samsung besides Nvidia's new LPU that they launched They're launching it next week,  but we're recording it the week before.

**Dwarkesh:**
[(2:28:21)](https://podwise.ai/dashboard/episodes/7508210?locate=8901)
It's coming out this week. This episode is coming out Friday.

**Dylan Patel:**
[(2:28:24)](https://podwise.ai/dashboard/episodes/7508210?locate=8904)
Oh, this episode is coming out before, sick! So they're launching this new AI chip next week, which is built on Samsung,  but that's like sort of a recent development from Nvidia. And then that's the only other AI demand there, whereas on TSMC, everything is competing. So he gets this like both geopolitical diversification, but also supply chain diversity for his robots. And he's not as competing as much with the willingness to pay of infinity of the data center of geniuses.

**Dwarkesh:**
[(2:28:52)](https://podwise.ai/dashboard/episodes/7508210?locate=8932)
Okay, final question. On Taiwan, if we believe that tools are the ultimate bottleneck,  How much of Taiwan's place in the semiconductor supply chain could we de-risk simply by having a plan to airlift every single process engineer at TSMC out when things come to,  if they get blockaded or something? Or do you actually still need to ship out the EUV tools,  which would be multiple plane loads per single tool and would not be practical?

**Dylan Patel:**
[(2:29:23)](https://podwise.ai/dashboard/episodes/7508210?locate=8963)
If you ship out all the process engineers and assuming it's like hot enough that you destroy the fabs,  no one has all the fabs in Taiwan now. Which is a big risk, right? These tools actually use a lot of semiconductors, which are manufactured in Taiwan. It's like a snake eating its own tail sort of like meme,  because you can't make the tools without the chips from Taiwan,  which you can't use without the tools in Taiwan. There's obviously some diversification there, and they don't use super advanced chips in lithography tools,  but at the end of the day, there is some tail eating the dragon.

[(2:29:55)](https://podwise.ai/dashboard/episodes/7508210?locate=8995)
Just shipping out all the engineers and blowing up the fabs means China has a stronger semiconductor supply chain than the rest of the world. Right. In terms of verticalization, now that you've removed Taiwan, and now you've got all the know-how,  but you've got to replicate it in, let's say, Arizona or wherever for TSMC. And it's going to take a long time to build all the capacity that TSMC has had built over the years. And so you've drastically slowed US and global GDP, not just growth, you've shrunk the GDP massively. And you've got a lot bigger problems. And your incremental ability to add compute goes to almost zero, right? Instead of hundreds of gigawatts a year by the end of the decade,

[(2:30:37)](https://podwise.ai/dashboard/episodes/7508210?locate=9037)
 let's say by the end of the decade,  something happens to Taiwan. Now you're at maybe like 10 gigawatts across Intel and Samsung or 20 gigawatts. It's like nothing. But now all of a sudden you've like really caused some crazy dynamics in AI. Of course you have all the existing capacity,  but that existing capacity pales in comparison to the capacity that's being expanded.

**Dwarkesh:**
[(2:30:55)](https://podwise.ai/dashboard/episodes/7508210?locate=9055)
Yeah. Okay, Dylan, that was excellent. Thank you so much for coming on the podcast.

**Dylan Patel:**
[(2:30:59)](https://podwise.ai/dashboard/episodes/7508210?locate=9059)
Thank you for having me and see you tonight.

