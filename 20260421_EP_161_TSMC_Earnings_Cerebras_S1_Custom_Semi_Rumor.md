---
podcast: "The Circuit"
episode: "EP 161: TSMC Earnings, Cerebras S1, Custom Semi Rumors, Apple CEO Change"
link: https://podwise.ai/dashboard/episodes/7806027
publish-time: "2026-04-21"
save-time: "2026-04-21"
---
# Summary

TSMC’s recent earnings report highlights robust growth driven by unprecedented AI demand, with the company successfully managing margin expansion and increased capital expenditure despite broader industry cycles. While advanced packaging remains a critical bottleneck, TSMC is scaling CoWoS capacity and planning for future nodes like A16. Cerebras’ recent S-1 filing underscores the industry’s intense focus on inference-optimized compute, though the company faces challenges regarding customer concentration and training scalability. Meanwhile, the semiconductor landscape is fragmenting as hyperscalers diversify their custom ASIC design partners to secure supply. Amidst these shifts, Apple is transitioning leadership to John Ternus, signaling a continued commitment to hardware-centric innovation and cultural preservation. Across the sector, compute scarcity remains the dominant constraint, forcing companies to prioritize efficiency and explore new architectures to meet the surging demand for AI-driven workloads.

# Takeaways

* TSMC’s recent financial success is driven by a consistent, across-the-board surge in demand for AI-related compute, which has effectively offset potential weaknesses in the traditional phone and PC markets.
* The semiconductor industry is experiencing a structural shift where custom ASIC portfolios are fragmenting into multiple, specialized product lines per generation, necessitating a more diverse and flexible approach to design partnerships.
* Inference compute has emerged as a high-margin utility, with the potential for significantly faster returns on hardware investment compared to the traditional, training-heavy business models.
* Advanced packaging, specifically CoWoS and upcoming glass substrate technologies, remains the primary technical bottleneck for scaling next-generation AI chips, with no viable shortcuts available to bypass the required multi-year engineering and material science development.
* The current market for AI compute is so severely constrained that any viable, high-quality hardware solution—including alternative architectures like Cerebras’ wafer-scale engines—is being rapidly adopted to meet the insatiable demand for inference tokens.
* Apple’s leadership transition to John Ternus signals a strategic commitment to maintaining the company's long-standing engineering-first culture while preparing for a new, aggressive hardware growth cycle.
* The concept of "premium tokens" suggests a future where AI inference services may implement tiered pricing based on latency and priority, mirroring quality-of-service models found in telecommunications.
* Server CPU demand is creating a secondary, significant pressure on ABF substrate supply, exacerbating existing scarcity issues originally triggered by the surge in AI accelerator production.

# Q & A

**Q: Why has TSMC’s business performance been so robust despite the cyclical nature of the semiconductor industry?**

A: TSMC is benefiting from a period of unprecedented demand driven by AI, which has allowed for significant margin expansion. While they have historically operated in a cyclical, moderate-margin industry, the current AI-driven cycle is proving to be durable. By executing well on new nodes like N3—which are reaching corporate average margins by the second half of this year—and maintaining a strategy of helping partners succeed rather than just squeezing them for higher prices, they have solidified their position as the essential bottleneck of the industry.

---

**Q: What is the current status of TSMC’s advanced packaging, and why is it considered a technical challenge?**

A: Advanced packaging, specifically CoWoS (Chip on Wafer on Substrate), remains a critical bottleneck for the industry, particularly for NVIDIA. While TSMC is actively expanding capacity and coordinating with OSATs (Outsourced Semiconductor Assembly and Test) to ramp up, the technology is inherently difficult to execute. They are currently piloting next-generation packaging, but it is a complex, multi-year engineering effort. There are no shortcuts; it requires significant material science innovation and time to reach volume production.

---

**Q: How has the market for custom ASICs shifted recently?**

A: The custom ASIC market is fragmenting. Previously, companies would design a single primary ASIC per generation. Now, we are seeing a shift toward a product portfolio approach where companies launch multiple specialized chips—some for inference, some for performance, and some for energy efficiency—within a single generation. This diversification allows hyperscalers like Google to shop around and potentially mix design partners for different products, rather than relying on a single, expensive vendor for everything.

---

**Q: What is the core thesis behind Cerebras’s repositioning toward inference?**

A: Cerebras’s unique wafer-scale engine is technically impressive, but it was not originally designed for the massive "scale-out" networking required for efficient model training. However, because their architecture performs AI math very quickly, it is highly effective for inference. Given the current, severe shortage of inference compute, repositioning around this demand makes strategic sense. They are essentially finding a niche where their specific capacity can be utilized while the industry struggles with a general compute deficit.

---

**Q: Is the industry facing a genuine, long-term shortage of inference compute?**

A: There is a strong consensus that the industry is in a state of compute scarcity. Even if some of this is driven by specific companies scaling faster than anticipated (like Anthropic), the overall trend is toward a massive, persistent deficit. As AI agents become more prevalent and models evolve, the demand for high-quality inference compute is likely to outstrip supply for the foreseeable future, making any viable compute solution highly valuable.

---

**Q: What is the significance of the "premium tokens" concept discussed by Jensen Huang?**

A: The concept suggests that not all AI tokens are fungible. In the future, there may be "premium tokens"—prioritized, low-latency outputs—that command higher prices. This is essentially a quality-of-service model. While some argue that the industry will eventually optimize away the need for such tiers by simply providing more bandwidth and faster hardware, the idea highlights a potential future where businesses pay a premium for faster, real-time AI outcomes, such as in voice-based agentic interactions.

---

**Q: How does the transition to John Ternus as Apple's next CEO reflect the company's long-term strategy?**

A: The transition is a positive development that provides clarity for the market. John Ternus is a long-time Apple veteran with a deep engineering background, making him well-positioned to lead the company's next hardware growth cycle. His appointment, alongside the elevation of Johnny Srouji to Chief Hardware Officer, signals a continued focus on Apple's core competency—hardware. Tim Cook’s primary legacy has been the preservation of Apple’s unique culture post-Steve Jobs, and Ternus is seen as a leader who will continue to foster that philosophy while driving execution.

---

**Q: Why is substrate availability becoming a major concern alongside chip production?**

A: The demand for server CPUs is growing significantly, with some models suggesting the market could reach $110 billion by 2030. This surge is putting intense pressure on the supply of ABF (Ajinomoto Build-up Film) substrates. It is no longer just the advanced AI chips (like H100s) driving this scarcity; the CPU demand is creating a supply imbalance, meaning the entire hardware ecosystem will likely face substrate shortages for the foreseeable future.

# Outlines

## TSMC Financial Performance and Advanced Packaging Strategy
[(00:05)](https://podwise.ai/dashboard/episodes/7806027?locate=5)
TSMC reported strong quarterly results, exceeding expectations in revenue and margins, driven primarily by unprecedented AI demand. Despite market concerns regarding capital expenditure increases, the company is aggressively expanding N3 node capacity and advanced packaging, specifically CoWoS. While technical challenges in CoWoS persist, the company maintains a long-term roadmap for A16 and glass substrates by the end of the decade. TSMC continues to prioritize partner success over aggressive price hikes, maintaining a collaborative approach to the semiconductor value chain.

---

## Cerebras Systems and the Inference Compute Bottleneck
[(17:36)](https://podwise.ai/dashboard/episodes/7806027?locate=1056)
Cerebras' S-1 filing highlights a strategic pivot toward inference workloads for its wafer-scale engine technology. While the architecture excels at AI math, it faces scaling limitations in training compared to GPU clusters. The company faces significant customer concentration risks, with primary ties to the UAE government, though recent partnerships with OpenAI and AWS signal potential expansion. The broader market is currently experiencing a severe shortage of inference compute, leading to increased demand for any viable hardware solutions, including potential adoption of AMD's upcoming offerings.

---

## Custom ASIC Market Fragmentation and Tokenomics
[(31:03)](https://podwise.ai/dashboard/episodes/7806027?locate=1863)
The custom ASIC market is shifting from a single-product model to a diversified portfolio approach, with hyperscalers like Google exploring multiple design partners, including Marvell and MediaTek, to optimize costs and performance. Concurrently, the industry is debating the future of "premium tokens"—a concept where high-priority, low-latency inference tasks command higher prices. While some suggest this mirrors quality-of-service models in telecommunications, others argue that rapid silicon advancements will eventually commoditize tokens, leading to a flat-rate pricing structure as compute becomes more abundant.

---

## Leadership Transition at Apple
[(46:09)](https://podwise.ai/dashboard/episodes/7806027?locate=2769)
Tim Cook is set to step down as Apple CEO, with John Ternus designated as his successor. This transition marks the end of a significant era of growth and cultural preservation post-Steve Jobs. Ternus, an engineer with a long tenure at Apple, is viewed as a strong choice to lead the company into its next hardware growth cycle. The appointment of Johnny Srouji as Chief Hardware Officer further signals a focus on maintaining Apple's internal silicon leadership and product development philosophy during this leadership change.

# Keywords

|Keywords|Explanation|
|---|---|
|TSMC|Taiwan Semiconductor Manufacturing Company, the world's largest dedicated independent semiconductor foundry. It manufactures chips designed by other companies, such as Apple and NVIDIA, and is currently a critical bottleneck in the global AI hardware supply chain.|
|N3|A specific manufacturing process node (3-nanometer) used by TSMC to produce highly advanced, efficient semiconductor chips. In the transcript, it is highlighted as a key driver of revenue and margin growth due to intense demand for AI-related computing.|
|CapEx|Capital Expenditure, which refers to the funds a company uses to acquire, upgrade, and maintain physical assets like factories and equipment. TSMC is significantly increasing its CapEx to build new fabrication plants to meet the global surge in chip demand.|
|CoWoS|Chip-on-Wafer-on-Substrate, a sophisticated advanced packaging technology developed by TSMC. It allows multiple high-performance chips to be stacked together, which is essential for the high-speed data processing required by AI hardware like NVIDIA's GPUs.|
|OSAT|Outsourced Semiconductor Assembly and Test, which refers to third-party companies that provide packaging and testing services for integrated circuits. TSMC is coordinating with these providers to help manage the overflow of advanced packaging demand.|
|Wafer Scale Engine (WSE)|A unique, massive chip design created by Cerebras that uses an entire silicon wafer as a single processor rather than cutting it into smaller individual chips. This design is engineered to perform AI mathematical operations at an extremely high speed.|
|Inference|The process of using a trained AI model to make predictions or generate content based on new data. The speakers note that while training models is a one-time cost, inference is becoming a massive, ongoing utility-like market with high profit margins.|
|ASIC|Application-Specific Integrated Circuit, a chip customized for a particular use rather than intended for general-purpose computing. Large tech companies are increasingly designing their own custom ASICs to optimize performance for specific AI workloads.|
|SerDes|Serializer/Deserializer, a critical component in high-speed communications that converts data between serial and parallel interfaces. It is a specialized piece of intellectual property often associated with companies like Broadcom that design high-performance networking chips.|
|John Ternus|The executive currently overseeing hardware engineering at Apple who is slated to succeed Tim Cook as CEO. His transition represents a shift in leadership toward a figure with a deep engineering background within the company.|

# Highlights

- [(08:07)](https://podwise.ai/dashboard/episodes/7806027?locate=487) We know our value and our position, but our partner's success is what is most important. We want to ensure our customers can be successful in their markets, and at the same time, we grow together.
- [(23:33)](https://podwise.ai/dashboard/episodes/7806027?locate=1413) We are at such a compute deficit that there is a small window for companies to position themselves accordingly, because the hyperscalers just need every ounce of available quality compute they can get.
- [(32:21)](https://podwise.ai/dashboard/episodes/7806027?locate=1941) The market for custom ASICs is fragmenting. It is no longer about making one custom chip; it is about having a product portfolio where you launch many chips a year.
- [(44:59)](https://podwise.ai/dashboard/episodes/7806027?locate=2699) The cost per token will continue to decline with advances in silicon. We won't need premium tokens; we will just need more tokens for certain things.
- [(49:42)](https://podwise.ai/dashboard/episodes/7806027?locate=2982) Tim Cook's real mission was to maintain Apple's culture post-Steve. He wanted to be the arbiter and preserver of that culture to ensure it would live on.

# Transcript

**Ben Bajarin:**
[(00:05)](https://podwise.ai/dashboard/episodes/7806027?locate=5)
Hello, everyone. Welcome to another episode of the circuit. I am Ben Beharin.

**Jay Goldberg:**
[(00:11)](https://podwise.ai/dashboard/episodes/7806027?locate=11)
Greetings, programs. I'm Jay Goldberg.

**Ben Bajarin:**
[(00:16)](https://podwise.ai/dashboard/episodes/7806027?locate=16)
So just for everybody's context, we are recording this on Monday, the April 20th,  because Ben was out of town last week, so we couldn't get it. So tight turnaround, which means you get some juicy news that also dropped today as a part of this podcast. Let's start. Last week, kind of the big news was TSMC's earnings. And before we get into that, I just want to hearken back to the early days of The Circuit,  where I tried to find this out, but I distinctly remember TSMC was about 90 with a forward P.E. of, I want to say, low teens. And I remember asking, like talking to you about this and being like, Jay,  I don't understand why Like, why is their PE not higher? Like, why is it? And I mean,

[(01:09)](https://podwise.ai/dashboard/episodes/7806027?locate=69)
 the obvious answer is everybody trading in those days knew that semis were cyclical and they are an okay margin business,  but they're not the best margin business. It's not software. So what we know about TSMC today People just didn't know back then,  but I remember us having that conversations burned into my mind when I looked it up,  when we were doing this, that it was, you know,  and I just was a little surprised it wasn't trading higher,  but hindsight's 20 20. And now we are here. They are doing remarkable things, including that which I have talked about numerous times as the trend of the industry,

[(01:45)](https://podwise.ai/dashboard/episodes/7806027?locate=105)
 which is margin expansion because their margins were Pretty surprising for a semiconductor foundry. So, um, okay. I will let you jump off with the highlights and then we will unpack a couple of dynamics that I think we both think were,  were interesting.

**Jay Goldberg:**
[(02:06)](https://podwise.ai/dashboard/episodes/7806027?locate=126)
Yeah. I mean, they, they reported last week and numbers were, I think, above, above expectations across the board,  both for the March quarter and for their guidance. Again, another one of these weird things where everything looked great and the stock was down on the news. But let's set aside that because we talked about that last week. Nothing makes sense anymore. It was a good quarter and I think what stood out for a lot of people on the call was just like,  it was pretty much across the board. Margins were better, revenue was better. CapEx, they increased their CapEx. They increased their expansion plans. They're adding another N3 fab. I mean, like how much more good news could they,

[(02:59)](https://podwise.ai/dashboard/episodes/7806027?locate=179)
 I can't think of anything else they could have said that'd be more good news.

**Ben Bajarin:**
[(03:03)](https://podwise.ai/dashboard/episodes/7806027?locate=183)
Yeah, I agree. I mean, I don't know if your take was the same,  but I just wonder if there was a little bit of uneasiness around the CapEx rays. I mean, I think that's what most people wanted. I know that was what was expected by the street,  but I think they spent a lot of time Really emphasizing,  you know, these investments will pay off. I mean, I don't think we should expect 60% margins forever. I think it was about 61. I saw some people estimate it could touch 67 going forward. I mean, to be honest with you, they are not in a place where I mean, I could be wrong. Maybe they are, that they're just going to keep milking margins for as long as this lasts.

[(03:48)](https://podwise.ai/dashboard/episodes/7806027?locate=228)
But as we've talked about, right, with Micron, even with TSMC,  names that haven't historically been high High margins in semis are benefiting from very high margins in semis right now,  and I think that's just a time of the cycle. But they need that CapEx, right? They've got to expand. I thought it was interesting that even later nodes are still driving a lot of revenue. You know, 5 nanometer, I think even some 7 nanometers contributing. There's legacy bits and maybe another part of the concern was, you know, just perhaps weakness in phones and PCs,  which is still sort of a variable that we expect or assume that's going to be down. But I don't know, maybe that drugs them down.

[(04:35)](https://podwise.ai/dashboard/episodes/7806027?locate=275)
I mean, it seems to be holding, not abysmal, but you're right, like it was all pretty good,  with the exception of where will phones and PCs be at the end of the year?

**Jay Goldberg:**
[(04:46)](https://podwise.ai/dashboard/episodes/7806027?locate=286)
Yeah,  I think there is a weird dynamic in the market where people sort of expect a lot and these guys met even those raised expectations,  I guess. There are a lot of perennial questions about valuation around TSMC and I don't wanna get into them all. I mean, it's just one of these weird things like there is a complex dynamic Across a lot of factors,  Taiwanese investors who own most of the shares tend to be a little more conservative in their valuation multiples than you get in the US,  especially around peak times like this. I don't fully understand how it's valued anymore,  but I will say that just on a fundamentals basis,  they did very well.

[(05:37)](https://podwise.ai/dashboard/episodes/7806027?locate=337)
I'll tell you, my favorite part of the call was the Q&A,  where See if you can detect the pattern. The first question is why are you doing more N3? And the answer was AI. And then the next question was, why are you raising your CAPEX guidance? And the answer was AI. And then the third question is, why are you raising your guidance? You seem more bullish. And the answer was AI. It was just like, yeah, it was just steady. Like it to me, it was just kind of calm. I didn't quite sound that way. But reading the transcript, I was just like, oh, the answer to that is AI. Just across the board.

**Ben Bajarin:**
[(06:17)](https://podwise.ai/dashboard/episodes/7806027?locate=377)
Which should be obvious. You know, one would think there's unprecedented demand. You know, I mean, I think this is the second sort of quarter where,  you know, management was really pushing to just still get everybody to understand this is going to last a while. You know, the cycle is durable. Spending time talking about You know, just because I guess part of my question is I wonder how many quarters this requires. Like at what point in time are we just like, yeah,  we've bought in or are you going to have to keep explaining and justifying? I mean, I get at least for the foreseeable future, but like how long?

[(06:59)](https://podwise.ai/dashboard/episodes/7806027?locate=419)
But I just find it interesting that that's still the, you know, look, we've got to keep pushing on. It's justified, right? These fabs we're building aren't going to sit, you know, empty at some point in time in the 10-year horizon. And so that just seems to be still an underlying, you know, subtlety of commentary.

**Jay Goldberg:**
[(07:20)](https://podwise.ai/dashboard/episodes/7806027?locate=440)
So I think there are two chief criticisms I hear lobbed against TSMC broadly,  not just by investors, but sort of broadly in the community. One is they need more capacity, right? They're the bottleneck for everything else. And I think they, you know, they're building with two extra fabs, one extra fab. They're adding another fab in Tainan, their Gigafab campus. That'll be N3. And then the second fab in Japan will be N3 as well. So we're adding two fabs. And then the other one I hear a lot is like, oh, TSMC is in a monopoly. They should raise the prices. And somebody asked on the call, do you recognize your value? You have such an important place in the value chain for the industry.

[(08:05)](https://podwise.ai/dashboard/episodes/7806027?locate=485)
Do you recognize that? And their answer, I thought, was pretty telling because they said, of course,  we know our value and we know our position,  but we also view that Our, I'll paraphrase here,  but they said that our view is that our partner's success is what's most important. We want to make sure that our customers can be successful in their markets. And at that same time, we grow together. Right. And I thought that's a pretty neat encapsulation of TSMC's culture. And I think if they say it a few dozen more times,  maybe people will stop asking them if they're going to raise prices because it doesn't sound like they did. It doesn't sound like they raised pricings.

[(08:46)](https://podwise.ai/dashboard/episodes/7806027?locate=526)
It's just they were executing better. N3 volumes are now a significant amount, and those are actually starting to yield at good levels. They said N3 margins will reach corporate average second half of this year. So that's the big thing. That's their thing about their margin levels vary as they bring on a new process. The new process doesn't yield as well, so their margins get hit by that. And that's just a matter of time as learning as they get that up and running. So I, you know, I think everything's there is going exactly as it should be going.

**Ben Bajarin:**
[(09:19)](https://podwise.ai/dashboard/episodes/7806027?locate=559)
Yeah, did you I saw a chatter about this and I listened to it,  but did you Read into anything about the I guess the softening of the view on Intel's competition whereas before it was pretty Throw-off like we're not worried,  and I don't think they're worried, but it was like we're not gonna We're not gonna underestimate them now people. Oh, they've you know Okay.

**Jay Goldberg:**
[(09:45)](https://podwise.ai/dashboard/episodes/7806027?locate=585)
I got that. There was definitely a sense, I don't have the exact quote here,  but like they were asked about competition a couple times. One time it was the context of TerraFab and they really didn't address TerraFab because they don't know any more than the rest of us do about what TerraFab involves. Right. I mean, they know more than us, but nobody knows what it means. But then again, they were asked about Intel. And they said, you know, we take our competitors seriously, right? Intel is a partner, and also a competitor or customer and a competitor. And they are, you know, they have a lot of talent is basically what it came down to.

[(10:20)](https://podwise.ai/dashboard/episodes/7806027?locate=620)
Yeah, I will say the one little little hint of Softness was around advanced packaging. They got asked a couple questions about advanced packaging and one was very pointed on the topic of what their roadmap is for advanced packaging and the context here is They are still constrained by CoOS packaging. That's their current advanced packaging. It's incredible stuff, but they only have so much capacity. They've added a lot to it, but that's still a bottleneck, especially for NVIDIA. And Intel, of course, seems to be doing very well around their advanced packaging alternative called eMIB. And EMIB allows for larger packages than COBOS does.

[(11:08)](https://podwise.ai/dashboard/episodes/7806027?locate=668)
And so people are sort of overreading that and saying, oh, Intel's going to be better at this than you. Like, should we be worried? And TSMC is aware of this. They have another packaging called COBOS on the horizon. It's piloting now. It'll be in production in two years. And that's the story. There was an article in the Chinese press this week saying that COPAS was delayed.

**Ben Bajarin:**
[(11:33)](https://podwise.ai/dashboard/episodes/7806027?locate=693)
I saw that.

**Jay Goldberg:**
[(11:34)](https://podwise.ai/dashboard/episodes/7806027?locate=694)
I didn't go back and look at everything they've said about it, but I don't think it is delayed. It's just going to take a long time. And it could be one of those things where the press reports that it's going to be available at X date,  and then that's actually the wrong number. And so when they get the real number, they say, oh, it's delayed. But it definitely sounded like their co-pos is having, I don't wanna say troubles, but it's hard stuff to do. They said that repeatedly. They said it's very challenging technically, right? Very challenging technically. They said that a couple of times. So it sounded a little bit like they're struggling with that.

[(12:13)](https://podwise.ai/dashboard/episodes/7806027?locate=733)
But still, it's in pilot now, so it's never gonna be perfect. Give them two years, I'm pretty confident they'll.

**Ben Bajarin:**
[(12:21)](https://podwise.ai/dashboard/episodes/7806027?locate=741)
Yeah, I mean, I think both with that and then again, right, just leading edge as we move toward,  you know, two nanometers, so roughly A16 and beyond. I think the narrative arc for that really and next generation packaging is just, you know, there's no shortcuts. Like this is just work that's got to get done, engineering work that's got to get done,  learnings that need to be made. Trust us to get it done, but this timeline is not perhaps what you would expect. I think the broader consensus, and I've heard this multiple times in the supply chain,  is they are ramping up what they're willing to do with OSATs to help with packaging as well.

[(13:09)](https://podwise.ai/dashboard/episodes/7806027?locate=789)
They're going to take people who have capacity I help, you know,  fill that out with fabs as needed and use the OSAPs to help. But again, that's now a level of coordination, right? It's not all under necessarily one roof, which most people like doing with TSMC. It's just a little bit more coordination. So the eye on the OSATs to be able to ramp as fast as possible is the key to maintain their growth because I think most people are still assuming they maintain,  at least for the next couple of years,  growth in the 30% and they need to keep ramping advanced packaging Really,

[(13:48)](https://podwise.ai/dashboard/episodes/7806027?locate=828)
 and new nodes to keep doing that and pushing their AI revenues higher because we just don't know what's going to happen in non-AI,  so phones and PCs and whatnot. AI is more than enough to offset that now, and hopefully that continues.

**Jay Goldberg:**
[(14:08)](https://podwise.ai/dashboard/episodes/7806027?locate=848)
Yeah, they said A14 or A16 will be shipping in 2028. So just for a moment, think about that. That means they'll have COPOS and A16 2 nanometer Shipping at the same time. I mean those are gonna be crazy chips, crazy packages.

**Ben Bajarin:**
[(14:29)](https://podwise.ai/dashboard/episodes/7806027?locate=869)
And somewhere around there we should see glass substrates because you know I've gotten a lot of questions about that lately and everything I had heard is that it's toward the end of the decade. Again it's not going to ship in volume but we got to start working out the kinks of glass substrates. So Again, very, very hard. No shortcut to a whole new material science being used in packaging,  but that's also around that timeline where we should start to see it show up at least in little quantities. So they're going to be there with advanced materials from the wafer equipment makers to start bonding chips to glass,  which I can't wait to see what that looks like, to be honest.

[(15:19)](https://podwise.ai/dashboard/episodes/7806027?locate=919)
I've seen glass substrates at Intel's, but I've never seen it with a dye on it or a package on it.

**Jay Goldberg:**
[(15:28)](https://podwise.ai/dashboard/episodes/7806027?locate=928)
Yeah, it's it's super interesting. I, you know, I'm just thinking about it. I think Intel will have that before them. Right.

**Ben Bajarin:**
[(15:35)](https://podwise.ai/dashboard/episodes/7806027?locate=935)
They're both saying. I don't know that to be honest with you,  but they're both saying around closer to the end of the decade.

**Jay Goldberg:**
[(15:43)](https://podwise.ai/dashboard/episodes/7806027?locate=943)
Yeah.

**Ben Bajarin:**
[(15:45)](https://podwise.ai/dashboard/episodes/7806027?locate=945)
I've heard people say it could come in 27 again, just because EMIB makes sense for it,  because like you pointed out, they can do larger packages and larger packages are where you get past the support of organic substrates. But I don't know, like this is the hardest part. There's a lot of people talking about, you know, I think getting over their skis,  if you will, on timing, particularly some of the optical stuff. And that includes glass because they're constantly like, I gotta be ahead of it. And you're like, that's great. But it's also a lot farther off than you think. These things start to scale in volume. So we just, we have to know timing. But I can't, I mean, it's gonna be so trippy, man,

[(16:24)](https://podwise.ai/dashboard/episodes/7806027?locate=984)
 to see chips packaged on glass is gonna be wild.

**Jay Goldberg:**
[(16:31)](https://podwise.ai/dashboard/episodes/7806027?locate=991)
You know, it's interesting. Nobody asked them about COOP, about silicon photonics.

**Ben Bajarin:**
[(16:36)](https://podwise.ai/dashboard/episodes/7806027?locate=996)
That's interesting. Yeah, right. Now that I think about it.

**Jay Goldberg:**
[(16:39)](https://podwise.ai/dashboard/episodes/7806027?locate=999)
I don't think they mentioned it in their prepared remarks either.

**Ben Bajarin:**
[(16:42)](https://podwise.ai/dashboard/episodes/7806027?locate=1002)
I mean, it's tiny revenues right now, but still.

**Jay Goldberg:**
[(16:47)](https://podwise.ai/dashboard/episodes/7806027?locate=1007)
It's strategic. It's strategic. And they know it's strategic. I know they're telling their supply chain, get in gear. It's coming. I guess if you think about volumes for For co-packaged optics, it's really still 2028 before the volumes really kick in. So I guess they didn't want to talk about it yet. I know it's important to them behind the scenes.

**Ben Bajarin:**
[(17:14)](https://podwise.ai/dashboard/episodes/7806027?locate=1034)
I guess. I'm sure they'll get a question by the end of the year.

**Jay Goldberg:**
[(17:23)](https://podwise.ai/dashboard/episodes/7806027?locate=1043)
Oh, yes. At the end of the year.

**Ben Bajarin:**
[(17:24)](https://podwise.ai/dashboard/episodes/7806027?locate=1044)
We'll keep a tab on. Hey, we got one. Let's go. Timing.

**Jay Goldberg:**
[(17:29)](https://podwise.ai/dashboard/episodes/7806027?locate=1049)
The world's geekiest drinking game.

**Ben Bajarin:**
[(17:32)](https://podwise.ai/dashboard/episodes/7806027?locate=1052)
Yes. Well, while that is the foundry news from last week, this week Intel report,  so I'm sure we will talk about that when we record the next episode of The Circuit. Alright, so, also happened Cerebras brought out their S1, which I thought was very interesting. We love S1s. We like to read through S1s. There was definitely good data on the revenue. There was obviously a whole slew of concerns of risk factors of customer concentration, which is always a conversation. Customer conversation, customer concentration never goes away. I know they had been very Inference language,  but I thought they were also like really pushing training with their chips.

[(18:26)](https://podwise.ai/dashboard/episodes/7806027?locate=1106)
It seems like reading through this it they put a lot more emphasis on on inference, which I don't again. It's not a pivot. It's just I think they realize inferences where. You can start to intersect some of this demand, so maybe that's a good place to be. Anyway, what were some of your takes?

**Jay Goldberg:**
[(18:46)](https://podwise.ai/dashboard/episodes/7806027?locate=1126)
So let me take a step back. Cerebras, for people who may not know it,  is a company that is designing a chip that covers an entire wafer. Typically, you put multiple chips on a wafer and you cut them up afterwards. They've just said, we're going to use the whole wafer and that's going to be a single chip. And from an engineering standpoint, this is super cool. I think everybody's very fascinated by this. I've talked to real engineers who've come up with all kinds of corner cases and Sarah Bruss has thought through all of this. What do you do with yields and how do you handle failures? They've worked through all that. They have all the software to work with it, all the drivers.

[(19:29)](https://podwise.ai/dashboard/episodes/7806027?locate=1169)
Super interesting technically. Commercially though, They've been searching for a market. And I think if you look at the way the chip is, they don't call them a chip,  it's a wafer scale engine, WSE. The way they have these wafers set up is It's very, very fast, right? Because you think about it, you can have, you know,  a chip is sort of bound by how many cores you can fit on a single chip. And they can fit, I think it's like 100 times more than even a Blackwell. Blackwells are massive already, right? They can fit a huge number of cores on this chip. They can do all that sort of AI math at At very large scale relative to anyone else.

[(20:17)](https://podwise.ai/dashboard/episodes/7806027?locate=1217)
The bottleneck they have, though, is it really wasn't designed for putting lots of these wafer scale engines together. And if you think about all the conversations we've had over the last two years about networking and the whole idea of scale up and scale out and scale across in what we're seeing with NVLink in these big GPU systems,  Especially when it comes to training,  being able to connect up multiple chips to each other so they're all communicating and sharing memory and sharing data is really,  really important. And Cerebras' chip wasn't designed for that. And I think there's a bottleneck. there that makes it very hard for them to work in training.

[(21:02)](https://podwise.ai/dashboard/episodes/7806027?locate=1262)
I don't think they're competitive in training but they can do AI math very quickly which lends itself to inference and as we all know there's a big shortage of inference compute right now and so it makes sense to me that they've now sort of repositioned themselves around this inference story. It makes sense. I think there are technical limitations of what they can do for training,  and I don't know how easy they are to solve. Even if they respawn the chip, it'd be tricky. But that's fine. There's a lot of demand for inference. But that of course leads us to the big question, which is they really have two customers,

[(21:40)](https://podwise.ai/dashboard/episodes/7806027?locate=1300)
 and both of those customers are affiliated with the government of the United Arab Emirates. Now, as part of, or right before the filing, they announced a deal with,  or they'd already announced a deal with OpenAI, but they put some language around it. They sized it up. They also announced something a little bit more nebulous with Amazon,  where it sounds like they're gonna be deploying Cerebras systems inside of AWS. But it is a pretty significant question around, like, who's the customer here? You know, I know adding OpenAI is obviously a good thing. OpenAI is big, but OpenAI is It's promiscuous. They have deals now with almost everybody.

[(22:27)](https://podwise.ai/dashboard/episodes/7806027?locate=1347)
And so how much will OpenAI actually end up spending on Cerebra systems is an important question that nobody knows the answer to right now.

**Ben Bajarin:**
[(22:37)](https://podwise.ai/dashboard/episodes/7806027?locate=1357)
Yeah. I mean, I think there's an interesting question around You know,  is there enough inference compute to go around when we constantly hear,  you know, compute constraints, which, you know, is part of the argument as to,  you know, why AMD's got a shot to grow, right? They're going to intersect against some of the inference workloads as they move to training. And I think that's kind of been like the pockets of wins that Cerebras has gotten is exactly that. They've got capacity. People need capacity. It's very specific to inference. And I think this could go a couple of ways, right? The same dominant players just continue to hold the vast majority of market share for inference,

[(23:29)](https://podwise.ai/dashboard/episodes/7806027?locate=1409)
 which is what I think most people would assume. Or is there air pockets? We are at such a compute deficit that there's a small window for some of these companies to position themselves accordingly and go do deals like this because You know,  the hyperscalers, either via themselves or via the neoclouds,  just need every ounce of available quality compute they can get.

**Jay Goldberg:**
[(24:01)](https://podwise.ai/dashboard/episodes/7806027?locate=1441)
Yeah, I mean that's obviously the hot topic right now. There's a theme running around these circles where we're talking about comparing OpenAI and Anthropic, right? OpenAI has signed all these deals with everybody and they seem to have ample compute and Anthropic is now throttling customers and doing all kinds of things because they didn't invest as heavily. That's at least the thesis, right? I think there is some truth to that because I'm a big Claude customer and Anthropic has clearly slowed it down. Well, it's improved this week a little bit. But at the same time, there is this narrative of we're super constrained in inference compute. Really emerged four weeks ago. You can see it in the data.

[(24:52)](https://podwise.ai/dashboard/episodes/7806027?locate=1492)
There's a point about four weeks ago when prices for H100, spot prices for H100 to the NeoCloud spiked up. Blackwell too, but really H100 is the noticeable one. And that lines up pretty well with the surge in demand we saw for Anthropic, especially around OpenClaw. And so How constrained are we in inference compute right now or is it everybody's constrained or is it just Anthropic is really constrained because they made some bad decisions last year don't have enough another scrambling and I think like I've heard that debate. I don't I don't know that I have a clear opinion on it.

[(25:31)](https://podwise.ai/dashboard/episodes/7806027?locate=1531)
I think definitely the way that the trend is working is I think more people will be more compute constrained as we get through the year.

**Ben Bajarin:**
[(25:40)](https://podwise.ai/dashboard/episodes/7806027?locate=1540)
Yeah, I mean, I think to your question, whether or not Anthropic just didn't invest,  I think they scaled a lot faster than perhaps they thought. Like some of these things, you just can't see that level of customer coming. And even today, they did a deal with Amazon where Amazon's going to invest Money in them,  they're gonna get, Anthropic's gonna use, Tranium, it'll be interesting,  I have no idea if this is credits or how it's gonna show up in the balance sheets,  but either way,  I'm sure they did a deal that was favorable tokenomics to Anthropic and favorable to look like return on invested capital to Amazon,  AWS. But all that is is just another absolute You know,

[(26:27)](https://podwise.ai/dashboard/episodes/7806027?locate=1587)
 pin for we don't have enough compute and and we'll take as much as we can. You know, to be honest with you, like I'm I'm really interested when just to this conversation,  like when we're Like when AMD is shipping Helios to see how it gets adopted in this moment in time where compute constraints are so significant. And it sounds like they have been trying to ramp volume to meet, to at least have capacity available,  demand available to go to the market. And so that part of that, I think will play out this thesis of, again, are we so compute constrained? That any viable compute, particularly for inference, will be adopted because that's essentially like my theory, right?

[(27:16)](https://podwise.ai/dashboard/episodes/7806027?locate=1636)
There's viable, there's non-viable solutions. And then there's viable solutions that just require some software work and agentics making it easier for you to port workloads. But some of these wins, right, for like an AMD, for Cerebras and whatever,  Would help sort of justify that, that yes,  there's so much demand for inference that any available quality compute is going to be adopted.

**Jay Goldberg:**
[(27:44)](https://podwise.ai/dashboard/episodes/7806027?locate=1664)
Yeah, I mean that's that that's the thesis right now holding in the market is there's just not enough. It's going through, demand is going through the roof and we need all kinds of compute and not just for GPUs. We now have a shortage in CPUs. In fact, in fact, TSMC talked about that as well.

**Ben Bajarin:**
[(28:00)](https://podwise.ai/dashboard/episodes/7806027?locate=1680)
Yeah.

**Jay Goldberg:**
[(28:00)](https://podwise.ai/dashboard/episodes/7806027?locate=1680)
And I'm going to, you know, I could see, like I said, there's a debate. I've heard up, I've heard the counter. TSMC seem pretty adamant that they're seeing big demand for CPUs as well. And I think that that's just kicking off. That still has a ways to run.

**Ben Bajarin:**
[(28:18)](https://podwise.ai/dashboard/episodes/7806027?locate=1698)
Yes, agree. Yeah, there's a lot of headroom. If it's the 80 to 100 billion, you know,  being modeled that that we we threw a model at Morton Stanley came out today saying it could be as high as 110 billion for service CPU by by 2030.  Whatever it is, it's going up. The slope is up. How much is the question? But I mean, I think That thesis is now well adopted. It was debated for a while, but I think we know we're gonna need more CPUs. We don't know how many. So what was interesting though from the Morgan Stanley note that I didn't do in mine,  because I just didn't want to get into the soil this right,  was the CPU demand is actually causing us more shortages in substrate.

[(29:01)](https://podwise.ai/dashboard/episodes/7806027?locate=1741)
So it's like your ABF substrate is getting worse not just because of The A6 but the CPU demand is putting equal pressure of that and we're going to have a supply imbalance where people are just going to be scrambling for every bit of substrate they can for CPUs as well. And so yeah, so substrates looking to be a shortage, a scarcity, if you will,  for who knows how long, but for the foreseeable future.

**Jay Goldberg:**
[(29:32)](https://podwise.ai/dashboard/episodes/7806027?locate=1772)
So, if you think about it, there is a real possibility if Anthropic continues to grow the way it's been growing. It's probably turned down a little bit, but still growing strong. And let's assume OpenAI comes out with a new version of ChatGPT later this year. And that starts to become really appealing as well. There is a really good likelihood that we just will not have enough compute.

**Ben Bajarin:**
[(30:00)](https://podwise.ai/dashboard/episodes/7806027?locate=1800)
Yeah.

**Jay Goldberg:**
[(30:01)](https://podwise.ai/dashboard/episodes/7806027?locate=1801)
Right. I think that is a very realistic scenario where just like nobody can grow enough, everything's throttled. People are going to leave money on the table just because everything's so log jammed up.

**Ben Bajarin:**
[(30:13)](https://podwise.ai/dashboard/episodes/7806027?locate=1813)
Yeah. Yeah, anyway, that's crazy. Computers, compute constraints as far as you can see. Anyway, so that'll be interesting to see. I'll be curious when Cerebras does IPO and see how the market reacts because to what you point out,  the customer concentration came up in every conversation I had. Revenue looks good. But again, I'll come back to the thesis I want to see play out,  which is any viable compute gets adopted when we're in a compute, you know,  scarcity, constraint, all of those types of things. You know, I guess we'll know by the end of the year, give or take, ish, ish. All right.

**Jay Goldberg:**
[(31:03)](https://podwise.ai/dashboard/episodes/7806027?locate=1863)
So personally, personally, yes, I'm doing everything I can to contribute to the shortage because we all are. Right.

**Ben Bajarin:**
[(31:10)](https://podwise.ai/dashboard/episodes/7806027?locate=1870)
I'm running I'm running agents like it's nobody's business, man.

**Jay Goldberg:**
[(31:13)](https://podwise.ai/dashboard/episodes/7806027?locate=1873)
Yeah. Yeah. I was I was at a meeting this week and somebody somebody tried to pitch AI to me like we were just talking about the context of some project we're working on. And I had to stop them. I said, look, While we're sitting here on this video call, I have five Claude agents running in the background. And frankly, if I weren't on this call, I would have 20 running. So I don't think you have to pitch that to me.

**Ben Bajarin:**
[(31:34)](https://podwise.ai/dashboard/episodes/7806027?locate=1894)
Preaching to the choir. There's also been some interesting, well one, Marvell's been on a bit of a run lately for a host of things. There was a rumor, it was very interesting, That came out from the information,  so take it as you will, that they were working with Google for some TPUs,  and then that got sort of starkly shot down by JP Morgan today, who basically said,  we are confident it is not for TPUs. It might be for a LPU-like thing, so a Grok-like thing, but not Grok,  but something for Google that is a inference accelerator. But the stock has been up and so the point I wanted,  the reason I'm bringing this up is I do sense that The market for custom ASICs is fragmenting,

[(32:32)](https://podwise.ai/dashboard/episodes/7806027?locate=1952)
 meaning that it was like, here's our one ASIC. Now it is, here are our multitudes of ASICs. Some might be inference-based, some might be performance-based, some might be energy. I don't know, but they're breaking the portfolio out. In Google's case, we know that's the case. The thing I think is interesting, though, is that it doesn't necessarily mean that they have to use as they,  you know, expand their portfolio of products, use the same player. The programs they had with Broadcom go away. It's that they expand into new products with perhaps someone else. That's the speculation that they're doing with MediaTek. We don't know what they're doing with Marvell.

[(33:16)](https://podwise.ai/dashboard/episodes/7806027?locate=1996)
But my point is, we used to look at it as custom ASICs was one sort of a thing. You make your one custom ASIC and you go. And now they have a product portfolio. And so within that, I can see diversity of partner, of design partner,  when you're working on a couple of different chips,  two, three, maybe even four at some point, right, that they launch, not just one a year,  it's many a year. And so I can see mixing up design partners to the degree that we're having this conversation. It's not, you know, that's all like somebody loses because somebody else wins getting another. It's again greenfield expansion and product diversification is I guess how I would land on it.

**Jay Goldberg:**
[(34:01)](https://podwise.ai/dashboard/episodes/7806027?locate=2041)
Yeah, so I've had some thoughts on Broadcom lately in this context and as I was talking to people about it,  it was very interesting to me the amount of Let's say emotion that some people carry into this debate.

**Ben Bajarin:**
[(34:17)](https://podwise.ai/dashboard/episodes/7806027?locate=2057)
Lots of emotion.

**Jay Goldberg:**
[(34:18)](https://podwise.ai/dashboard/episodes/7806027?locate=2058)
There's lots of emotion, right? Because the status quo today is Google uses Broadcom for its TPUs, right? Google designs the chip and Broadcom does the sort of the perimeter of the chip and has IP and packages and sort of designs it all up and takes it to the fab. They're the design partner. And there is some awareness that that's expensive. Broadcom, not a company known for low prices. And it arguably has a pretty solid borderline monopoly on some of its IP, especially around things like SerDes. And so there is a perception that Google wants a lower cost alternative. And they've clearly piloted something with MediaTek.

[(35:06)](https://podwise.ai/dashboard/episodes/7806027?locate=2106)
And it is one of the most debated topics I know on the street right now is how much share did MediaTek get at Google at Broadcom's expense. It doesn't sound like it's Enough to really scare Broadcom into changing their prices,  but now there's this idea that Marvell is in the mix as well, which seems pretty possible. I'm sure Google is looking at SRAM-based alternatives for TPUs, right? Because let's remember that this whole approach to LPUs or SRAM-based Accelerators came from a company called Grok and the founder of Grok was one of the original TPU designers. So Google knows this space well. Everybody needs cheaper, more efficient inference solutions.

[(35:58)](https://podwise.ai/dashboard/episodes/7806027?locate=2158)
We've just been talking about that for 20 minutes. And this LPU approach doesn't require HBM, which is another big bottleneck. So, yeah,  it makes sense that Google's looking at it and I'm sure they're going to send out their bids to ask for bids from all the vendors. I think we're a long way away from knowing how that's going to shake out. Could Marvell be in the mix? Absolutely. Are they going to defeat Broadcom? Who knows? Who knows?

**Ben Bajarin:**
[(36:29)](https://podwise.ai/dashboard/episodes/7806027?locate=2189)
Yeah. No, agreed. And I think, again, if we're Google, if we're Amazon or whatever, we're talking to all the design partners. We're looking at what we can do. It's not uncommon to shop around. Doesn't mean you decide, doesn't mean you scale, doesn't mean that design partner wins,  but you're certainly going to do your due diligence as you evaluate a host of things. So none of that should surprise anybody that they're in those customer conversations,  that they're talking to all of those different customers. But that doesn't necessarily translate to specific design wins. I think that's important, broader, important context. But anyway, it's been good to see Marvell gets a lot of hate.

[(37:16)](https://podwise.ai/dashboard/episodes/7806027?locate=2236)
They've got good stuff. I think, again, as this market fragments. As ASICs break out into multiple products per generation, it'll be competitive. It's not one market. It's many markets and there's many business models going around. That's essentially how to look at it. But before we go to the last news bit of the day, let's talk about the Jensen podcast with Dwarkesh. Since you won, the point you wanted to bring out kind of ties to Grok or the LPUs and inference tokens. So I'll let you do that and then we'll talk about the infrastructure's role in this point.

**Jay Goldberg:**
[(37:57)](https://podwise.ai/dashboard/episodes/7806027?locate=2277)
Major topic of conversation in all of my circles this week or over the weekend was Jensen was on Dworkesh's podcast and it got pretty heated when they were talking about China. And I think it's interesting to see who Dworkesh decides to push and who he doesn't. But he gave Jensen a pretty good run for his money there. I won't get into that. That's a very complex subject that I'm happy to discuss some other time. But I thought there's a lot of other interesting things in there beyond that. Having Jensen talk for almost two hours about how he sees the market is worth listening to,  not just because of the little debate, although that was good radio, but in particular,

[(38:41)](https://podwise.ai/dashboard/episodes/7806027?locate=2321)
 he raised this topic of premium tokens. And I think he's actually mentioned this once before, either at GTC or the last earnings call. He like just touched on it. But his thesis is that right now we sort of treat tokens as a fungible commodity,  but with time they're going to be some tokens that are higher priority that are worth more. And he was really speaking about this in reference to the acquisition of Grok,  right, where he's saying like, if you want to do,  Grok is really good for low latency inference,  which Is sort of you think about like speech, speech recognition, right? If you want your, your AI agent to be sort of talking to you in real time,

[(39:24)](https://podwise.ai/dashboard/episodes/7806027?locate=2364)
 you need that inference to be very low, low latency. And right. And if you think about that, then you need a, like you,  there's a premium attached to the tokens around something that's in a hurry. This is, you know, for, for networking people,  this is sort of quality of service type idea where you're there are premium bits and,  and It's a really interesting thesis. I don't think it plays out that way. I don't think it ends up going that way. I think we optimize around it. That's certainly what happened in the networking world. But it's an interesting idea, right, that we're going to have different tiers of tokens,  some that are worth more that are prioritized over others.

[(40:06)](https://podwise.ai/dashboard/episodes/7806027?locate=2406)
And I think it's interesting not just in terms of sort of base tokenomics,  because that's always fun to talk about,  but also in the idea of this evolving market for AI services and how we're gonna need different kinds of compute for that. I tied it back to our conversation about CPUs, right? Some things we're gonna do AI, we're gonna do agentic AI with CPUs. Is that a cheaper token? I don't know, but it's interesting to think through the implications of all that.

**Ben Bajarin:**
[(40:39)](https://podwise.ai/dashboard/episodes/7806027?locate=2439)
Yeah, yeah, yeah, he mentioned this at GTC. It was in relation to justifying Grok. His point was essentially that, you know, those who sell tokens might be able to offer tiers,  some that are drastically faster to outcome, which is where Grok would come in. Or if you don't care because you're a free service, then You're just, you know, turning those tokens. You want to pay the lowest rate possible because you're making that up on ads. So I definitely think that makes sense. Again, it's not everybody. It's not going to be every business, but there will certainly be some businesses who will be willing to pay more for a faster outcome. And fine, you know, that makes sense. We'll see.

[(41:21)](https://podwise.ai/dashboard/episodes/7806027?locate=2481)
How much but I think it's a plausible theory and there's good reason to have faster compute or again vastly accelerated infrastructure In order to be able to charge a premium for tokens So that's that it seems plausible. But yeah, I mean I like I It seems really early to be talking about because you're like,  first of all, just get tokens adopted. Then you can start saying who wants to pay more. But the fragmentation of prices certainly makes sense. And, you know,  we're going to do a report on tokenomics because Max on my team has been benchmarking infrastructure from an inference standpoint. And suffice it to say, we have a lot of good data to basically Confirm that inference margins,

[(42:12)](https://podwise.ai/dashboard/episodes/7806027?locate=2532)
 so your margins on inference tokens, are very, very, very good. And when inference becomes, like training is just you train. That's a sunk cost. You pay that cost in the hopes that you can then get people to use your models and serve them tokens that they'll pay for. Once that kind of settles and the vast majority of the world is running on inference,  They're going to start making a lot of money. And I can see how you could say your tokenomics are even higher in value. Because really, if these are utilities, even the way my report on Anthropic was, it's an intelligence utility. The token that you can charge needs to be more than what it takes to produce it.

[(42:54)](https://podwise.ai/dashboard/episodes/7806027?locate=2574)
And if your margin is drastically higher, as it sounds like inference is,  you will return that investment or you will make money on that hardware way quicker than they really can on training or people paying you for training. So I think that will be some of the things that split tokenomics into different dynamics. But we are not in an inference, largely inference tokenomics world yet. That's still starting to ramp.

**Jay Goldberg:**
[(43:23)](https://podwise.ai/dashboard/episodes/7806027?locate=2603)
Yeah, the more I think about it, the more I don't think it's going to play out that way. And I'll tell you what really sort of catalyzed my thinking is Benedict Evans had his note out last night. I was reading through it. And his description of the changing pricing tiers around models, around AI, agentic AI and whatnot,  He keeps coming back to the parallel with telecom. And I understand AI is not telecom. They're very different industries when regulated or not. Like, I understand they're very different. But in terms of just sort of raw economics, where you have this massive upfront cost,  you have to build all this hardware, you have to buy all this hardware,

[(44:00)](https://podwise.ai/dashboard/episodes/7806027?locate=2640)
 you have to train the model, massive upfront costs that you then seek to monetize as efficiently and quickly as possible. There are some, it's a worthwhile comparison to make. And his take, and he was a telecom analyst for a long time and knows this stuff,  his take was ultimately this all goes down to tiered flat rate pricing, right? And I know what happened in the networking world. There was a similar idea of quality of service where things like voice were going to get a certain flag that those would be prioritized and those packets we send through first. And that never ended up happening because the networks themselves got so much faster that you could just throw more bandwidth at it,

[(44:45)](https://podwise.ai/dashboard/episodes/7806027?locate=2685)
 that you didn't actually need to have those flags in place. And I think that's what happens here where the cost of Cost per token just will continue to decline with all the advances in silicon. You know, over a long term and we won't need sort of premium tokens. We'll just need more tokens for certain things and you'll pay for it that way. That's my guess is how this all ends up.

**Ben Bajarin:**
[(45:11)](https://podwise.ai/dashboard/episodes/7806027?locate=2711)
Yeah, I mean, it could be. I mean, I think I've seen people throw the same analogy around power. You know, it's hard to say that you're, again, you can charge different rates,  right, on peak times because there's volume or power is scarcity. And I think that's relatively true. I think there'll be some dynamics of that, right, that play out. But even if it goes to that model,  I think what we will prove with our economics is it's still going to be highly profitable from a margin standpoint above what it costs to produce that token in terms of hardware cost and energy at scale. And all that work just gives me A little bit more hope, right, that not only is it durable,

[(45:54)](https://podwise.ai/dashboard/episodes/7806027?locate=2754)
 that people will make that money up because inference margins will be so much larger than training margins are,  and it will scale so much farther than training. So, but this is like early days, so it's very hard to predict.

**Jay Goldberg:**
[(46:08)](https://podwise.ai/dashboard/episodes/7806027?locate=2768)
To be clear, my vision isn't unhopeful. It's just, it's a different trajectory. There's still going to be, I mean,  my trajectory is basically you need so much more compute Because you're just going to throw tokens at all these problems. I think that's how it shapes out.

**Ben Bajarin:**
[(46:23)](https://podwise.ai/dashboard/episodes/7806027?locate=2783)
Yeah. On that we agree. OK, lastly, Apple, Tim Cook has now said he will be stepping down from Apple, I believe. September or October 1st. So the transition is fully in play for John Ternus to become CEO, which I think is a good thing. We've talked about this before to the degree we've talked about the Apple's Leadership transition that,  you know, there's angst in the market. People want to know who's going to lead Apple for the next 10 or 20 years. And just getting into this position where we know it's going to be John Ternus. He's well liked. He's been an engineer. He spent almost his entire career at Apple. He's been responsible, you know, for overseeing a lot of the product development.

[(47:11)](https://podwise.ai/dashboard/episodes/7806027?locate=2831)
So there's really no Downside to this, I think a lot of hardware people will be very,  very excited to come there and to come work at Apple, to be honest with you. So I think it's a positive. I definitely don't see any downside to this. It doesn't seem like anybody seems to be To be, you know, down on this,  but it's interesting that, you know, something we've been waiting for,  kind of the end of the Tim Cook era too,  and on to the John Ternus and beyond. With that in conjunction, Johnny Struggi was named Chief Hardware Officer. So just sounds like a new role they created for him. He's going to be getting more responsibility for that, which I thought was interesting.

**Jay Goldberg:**
[(47:52)](https://podwise.ai/dashboard/episodes/7806027?locate=2872)
The Apple Silicon leader.

**Ben Bajarin:**
[(47:53)](https://podwise.ai/dashboard/episodes/7806027?locate=2873)
Apple Silicon leader, yeah, Johnny Trujillo. So yeah, you know, I don't know. Did you have any takes?

**Jay Goldberg:**
[(48:01)](https://podwise.ai/dashboard/episodes/7806027?locate=2881)
So first, everybody, I gotta say this is Ben called this. Ben and I are on a chat group with other analysts and This topic came up,  what, six months ago about, you know, is Tim Cook on his way out? And you said it was gonna be John Ternus who's gonna be the next CEO. So you called it. I think you got the timing right, too. Right around the 50th anniversary, he got through that and now. I think it's, yeah, I think it's a good time. I think the market was, it's better to leave when, you know, people will miss you. And I think the market is starting to get a little, the street was getting a little bit,  starting to question Tim Cook a little bit more.

[(48:42)](https://podwise.ai/dashboard/episodes/7806027?locate=2922)
Not, I don't think that's the reason why he left, but I think he's going out at the top. I imagine there'll be a few people wondering what's gonna happen on the software side because it's the big sort of Question mark hanging over apples. What are they gonna do an AI? but at the same time like they they they are a hardware company and It's important to you know,  that's how they make their money. So it's a It seems like a good a good move to me And I think it's it's good it's time for a change.

**Ben Bajarin:**
[(49:14)](https://podwise.ai/dashboard/episodes/7806027?locate=2954)
Yeah, and I think, you know, I've sort of had this conversation with friendlies,  you know, at Apple, I think, you know,  everybody gives Tim Cook a lot of credit and rightfully so for,  you know, taking Apple from a, I forget what it was, 30,  40 billion dollar company when he was CEO to now,  you know, 40 something, 425 or 4, I think, billion dollars a year. So huge. They give him a lot of credit for that execution. What I think was important, and I really firmly believe this was his real mission,  and perhaps the broader legacy that he wanted to leave,  was to maintain Apple's culture as best as he could post Steve. And, you know, because they had always sort of talked about, right, that Apple,

[(50:06)](https://podwise.ai/dashboard/episodes/7806027?locate=3006)
 when you work at Apple, it's not like anything else. It's a very different culture. You have a different point of view on products. People might not always agree with that externally, but there was a point of view. There was a philosophy. There's a culture. And the fear, right, when Steve Jobs died,  like I remember having many conversations with the media about this,  was what happens when he loses the culture, right? When your leader goes, it just all goes downhill from there. And, you know, again, it's not like Apple's been perfect every step of the way,  but they've maintained, I think, a lot of that culture for the long, you know,  the length of time that it's been that Steve is not around.

[(50:40)](https://podwise.ai/dashboard/episodes/7806027?locate=3040)
And I think Tim Cook He wanted to be the arbiter of the apple culture,  the preserver of the apple culture. And I think he wanted to make sure that that was going to live on. Before he stepped down and I think that played into his timing as much as anything and the good thing is John's been there long enough He was there when Steve was there. So he also has that pedigree and now again that execution I think they're I think they're ramping up for a hardware growth cycle And some of the aggressiveness they're gonna have on their roadmap,  you know, I think he's well positioned for that and again Can help keep and foster that culture going forward.

[(51:19)](https://podwise.ai/dashboard/episodes/7806027?locate=3079)
So, um, so yeah, it'll be, it'll be very interesting, but I think this will get,  you know, really well received. I'm very excited to hear his first earnings call and just see what the questions are,  see how he handles it. Um, you know, that'll be, that'll be super interesting, but, uh, but yeah, end of an era for,  for Tim Cook and onto the John Ternus era as CEO of Apple.

**Jay Goldberg:**
[(51:45)](https://podwise.ai/dashboard/episodes/7806027?locate=3105)
Yep.

**Ben Bajarin:**
[(51:46)](https://podwise.ai/dashboard/episodes/7806027?locate=3106)
Crazy times. Crazy times. All right, everybody. Thanks for listening. And we will talk to you next week. Actually, this week, still next week, it'll be published with a whole host of other topics. So we will talk to you then.

**Jay Goldberg:**
[(52:00)](https://podwise.ai/dashboard/episodes/7806027?locate=3120)
Thank you, everybody. Tell your friends. Click like and subscribe.

