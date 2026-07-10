---
title: "Teaching Analytics in the Age of AI"
layout: single
classes: wide
author_profile: true
permalink: /ceu-ai-podcast-2026/
redirect_from:
  - /ceu-ai-podcast-2026.html
---

I was a guest on **CEU's *Teaching Analytics in the Age of AI*** podcast, in conversation with **Eduardo Ariño de la Rubia**. We talked about how AI is changing what — and how — we teach data analysis: why almost every classic form of assessment is now in trouble, what "taste" is and why it has become the scarcest skill, how a single December of playing with coding harnesses like Claude Code upended a whole course, and why the real bottleneck to AI's economic impact is organisational, not technical.

*Listen to the episode here: [Teaching Analytics in the Age of AI — Gábor Békés (CEU Podcasts)](https://podcasts.ceu.edu/content/teaching-analytics-age-ai-gabor-bekes).*

Below is a set of highlights, a few memorable lines, and a lightly edited transcript of the conversation.

---

## Highlights

- **Every traditional assessment is under pressure.** Once students can interact with technology, the take-home assignment and the open exam stop measuring effort. What survives is the pen-and-paper, zero-tech exam — and a much harder question about what is actually worth teaching.
- **The scarce skill is taste, not coding.** Being able to write correct code to spec used to be the hire-worthy signal. That is now cheap. What matters is judging whether a question is worth asking and whether the data can even answer it — "even though I can do it, it's not going to bring an insight."
- **A single December rewired the course.** The jump from typing into a chatbot to running a model that works on your own computer and does real tasks (Claude Code and similar harnesses) turned "here's a neat trick" into "this is the thing we now have to teach."
- **The macro shift is huge but slow.** AI is probably as important as electricity or the internet — but the adoption bottleneck is organisational, not that your laptop can't reach the model. Rewiring an organisation to actually raise productivity takes years, not weeks.
- **Advice to students: be brave and experiment.** AI can do a lot, but nobody yet knows exactly what. Try things you don't think you can do, then go back and understand enough to judge the result. If you can, get someone to fund your tokens.

---

## Memorable lines

> "So you should say, *No* — even though I can do it, it's not going to bring in an insight. This is what I mean by taste. It's very important."

> "Having anything other than an in-class pen-and-paper exam is in jeopardy. Whenever students can interact with technology, examination as such is gone."

> "AI is at a stage where it can do a lot of things, but we don't exactly know what. So there is great room for experimentation. You should be brave — do things you don't think you'd be able to do, then go back and understand as much as possible so you can judge it."

> "The big picture is that we allocate resources — cutting some things and doing much more to figure out what AI means for us. That's the biggest risk: not doing that."

> "The barrier is how an organisation is able to completely rewire itself to let this technology become part of everyday work and increase productivity."

---

## The conversation

*For convenience this is a lightly edited version of a machine transcription of the episode — cleaned up for readability, with obvious transcription slips fixed. The wording is close to, but not a verbatim record of, what was said.*

### Background

**Eduardo:** Today I'm joined by Gábor Békés, a professor in the Department of Economics and program head of the MSBA program. His research includes football analytics, and he recently published interesting work on which teammates football players prefer to pass to. He's one of the authors of *Data Analysis for Business, Economics, and Policy* from Cambridge University Press. Thank you, Gábor, for joining us on *Teaching Analytics in the Age of AI*.

**Gábor:** My pleasure.

**Eduardo:** I'm especially glad to have you here because, in many ways, you're the reason I'm in the department — we've had that relationship over many years now. Your work sits at the intersection of analytics, research, economics, teaching, and the way AI is changing what students learn. Before we get into all that: can you give listeners the human version of your bio? What do you work on, what do you teach, how did you end up here?

**Gábor:** I'm an applied economist, which means I work on economic questions using data. I work on how people and companies collaborate, and how organisations work. In the past I worked on international trade — how companies decide and end up being part of global supply chains. Now I work mostly on open-source software: how people, rather than companies, collaborate and start new projects. I also have a very different strand using historical, archival data to understand firms joining international supply chains and how industrial policy affects that.

The common theme, when I ask myself what connects such different topics, is *large and unique data* — finding it and working with it.

That's the research side. On teaching, I've been teaching data analysis for about 15 years now. I wrote a textbook with **Gábor Kézdi** called *Data Analysis*, which has been out for a couple of years.

**Eduardo:** Clever SEO naming.

**Gábor:** Absolutely. The first title was *Patterns, Prediction, Causality*. Then Cambridge University Press said, you need something universities can easily identify — hence *Data Analysis for Business, Economics, and Policy*, exactly for your reason.

**Eduardo:** It's a great textbook — we use it in the program.

**Gábor:** We do, and it grew out of the program. I learned machine learning partly as a way to try to teach it — teaching is one way to learn things. I teach it mostly for social scientists, or people who want to become economists or political scientists, so I wanted to understand machine learning to a degree that's manageable for people who don't come from a computer-science background.

### What students needed then, and now

**Eduardo:** When you first started teaching, what did you think students needed from you — and what do you actually think they need now?

**Gábor:** When I started, I thought — and I still think this matters — that the job was to show them what good modelling and good analytic process look like: how to figure out patterns, prediction, and causality, and do it well. Students still need that, but maybe a bit less so. What I *didn't* appreciate then is how much it matters to talk about what makes a good question and how to start one. That's grown over time.

**Eduardo:** Was there a moment that changed your mind — students, the field, your own mistakes?

**Gábor:** Life in general. There was a point that led to the birth of the textbook: people had studied a great many methods but didn't know which one to apply or what to do with the results. That was the reason we wrote the book — not to invent new methods, but to curate a subset covering maybe 95% of use cases and guide people on which to use and what to do with the results.

There was a clear moment supervising capstones and theses when I realised the bottleneck had moved. With data now so easy to get, the hard part is no longer access — it's deciding what's a meaningful question. There's so much you *could* look at; why look at A and B and not the rest?

### The "Data Analysis with AI" course

**Eduardo:** You teach directly from the textbook — there's a sequence. Tell us about one course: the title, but really what it's about beneath the title.

**Gábor:** The book has four parts; I teach two, colleagues teach the others. Mine are predictive modelling and causal inference. Take causal inference: we teach how to understand and estimate treatment effects from interventions — policy changes in the economy or at companies — and their consequences. The big picture is *conditional comparisons*: finding the right conditions to compare treated and control groups meaningfully. A large part of analytics is exactly that — what can we learn by comparing meaningful units? In causal inference it's a causal question; in prediction it's why some units are higher-priced or larger.

On top of that — and this isn't in the textbook — I teach a class called **Data Analysis with AI**.

**Eduardo:** Tell me more about that class.

**Gábor:** It comes after students have studied the core of the textbook — descriptive analysis, prediction, the elements of machine learning, the core ideas of causal inference. Until then, the goal is that you understand everything and can do the work yourself. In this class we take off every control we have and let you use AI — to do things you already know how to do, but faster, and more importantly to do things you *don't* know how to do. The course is about getting to where you're doing things you couldn't do without AI, and then figuring out how much of that work you actually need to understand: where you need strong control and real comprehension, and where you can say, "fine, magic — I don't need to know."

### The December that changed everything

**Eduardo:** Do you remember a moment when a student really got it, or did something unexpected with AI?

**Gábor:** This is the second year I'm teaching it; the course starts in January. What I remember most is how much changed between planning it a year and a half ago and teaching it. There was a huge drop in how much the models hallucinated. Last year, students realised that once you use the paid models properly, they actually work quite well — contrary to the hallucination-and-errors stories, they hallucinate very little. Around then RAG arrived, and models simply got better.

Then, over this past winter, **harnesses like Claude Code appeared** — and completely destroyed my Christmas break, because I realised that everything I'd planned was no longer hard, and no longer a meaningful thing to demonstrate. Instead: oh my God, *this* is something we have to do. So this year the aha moment was really the capability of Claude Code and other harnesses.

**Eduardo:** That's one of the fun things about teaching at the cutting edge — a December happens, everyone goes home and plays with these harnesses, and you realise you can't teach a course on chatbots anymore.

**Gábor:** True. And here's my advice to anyone teaching: *don't* teach on the cutting edge. It's tremendous stress and work. You're barely ahead of your students on the technical capabilities, there's no set curriculum — it's exciting to figure out, but it's very hard.

The big story this year was that going from typing into a chatbot to having a model that works on your computer and does tasks is a very different proposition. The other aha moment is how far students can go over three weeks. In the last part of the class there's a three-week run where groups of three take a single capstone project from zero to hero — a complex problem where no one person knows all the parts. It includes NLP, complicated econometrics and causal inference, data collection, entity resolution. We teach all of it over a year, but students come from different backgrounds: a second-year economics master's student knows more econometrics, a business-analytics student knows more about handling data, and so on. In their group everyone knows something, but nobody knows everything — and I ask them to do a lot. Realising how far you can go is the other big experience.

### What AI breaks in teaching

**Eduardo:** Teaching in the age of AI is hard. Can you think of an assignment, exam question, or project type that used to work but is now just broken because of AI?

**Gábor:** Yes. All of them.

**Eduardo:** Say more?

**Gábor:** All of them. It's bonkers. Anything other than an in-class pen-and-paper exam is in jeopardy. Once students can interact with technology, examination as such is gone. Assignments are still useful for people who want to practice, but as a way to tell apart effort they're much weaker than before. There's no classic university activity that isn't massively undermined by AI — and I don't think many administrators or outsiders appreciate how taxing it is to rethink so much of what you do. Some people rethink it, some don't, and it's just the beginning.

We're still teaching mostly the same things and worrying about *measuring* student effort — which is honestly secondary. We're thinking less about the real question: what should we teach? Our program is a bit special here because we're genuinely interested in this, but even we are just starting to ask what university education should look like when AI can do a lot of things at 80–99% — or 110% — quality. One example of something new: having groups of humans and agents work together, and experimenting with that — I'm not even sure "teaching" is the right word — letting students try things. That's something I do now that I didn't do a year or two ago.

### Competence and "taste"

**Eduardo:** We're in a new world where raw intelligence isn't quite the bottleneck — you can buy it by the token. But humans aren't going away. At our alumni event in Budapest we asked whether people thought AI would replace or augment humans, and most said augment. But if you're augmenting humans, you have to pick the *right* humans — you need some signal of competence. What skill used to signal competence but doesn't anymore, and what signals it now?

**Gábor:** In the past, if you were a good computer-science person who could take a detailed spec and write good code that did exactly that — that was super useful. I hired assistants based on it. That skill still exists but matters much less. The most useful skill now, and the hardest to measure, is **taste**.

**Eduardo:** Go on.

**Gábor:** Taste is having the experience and ability to judge whether something makes sense — not superficially. You can run a regression that's technically correct: the right formulae, a result, a nice table. But *should* you run that regression? Does the model make sense for your question at a deep level? Is the data even appropriate to ask it? Sometimes you should say: no — even though I can do it, it won't bring an insight. That's taste. It's hard to acquire and very valuable.

**Eduardo:** Taste is also hard to teach.

**Gábor:** One of my favourite films, which I often mention in class, is *Arrival* — aliens arrive speaking an unknown language, and as the linguists work to learn it, their way of thinking changes. That's how I think about taste. You can't teach it directly. You showcase a lot of good work; as students work through good questions and case studies and hear from people with real experience, they think they're learning coding, regressions, machine learning, cloud computing, deep learning — and they are — but through those good examples they ideally develop what becomes taste.

### Rebuilding the curriculum

**Eduardo:** Imagine it's three years from now and we're rebuilding the MSBA curriculum. What do we cut or compress, and what gets highlighted that isn't today?

**Gábor:** We already change the curriculum about 20% a year — we moved from R to Python, added cloud computing, reduced classic ML in favour of more deep learning, increased the role of AI across courses. So there's constant change even before AI. I'm happy with the content we have now. Apart from growing this collaboration — humans and agents working in teams, which I see as the near-term growth area — I don't have a specific target I'm steering toward. The technology and practices change so fast.

A colleague and I were debating how much agile matters, and he said: we're now running a "dark factory" approach. For listeners — a dark factory is the idea that machines can work on their own, with no constant human oversight, so you can switch off the lights. They've appeared in some manufacturing, and now there's analytics done this way too, with computers running for hours without much oversight. How you manage that, I don't know. So: gradually more toward this space of human–AI collaboration.

**Eduardo:** I agree — we're at the dawn of the agentic age, where most employees, even individual contributors, will themselves be managers, managing these "dark factories" and swarms of agents. Three years from now that could be a much larger part of what we teach.

**Gábor:** Yes — and the question is how much we still teach the basics, partly *because* it helps develop taste. You still need to understand the core principles and the simpler stuff. I wouldn't let that go.

### Allow AI, or zero tech?

**Eduardo:** Students use AI — we encourage it in many courses, and they use it on their own. Can you think of a time a student surprised you with what they built or accomplished with AI?

**Gábor:** Honestly, no — and partly because university policies generally try to curtail AI use, so it's hard to see what's really AI. In my Data Analysis with AI class there were projects that were genuinely good, but I wouldn't call them surprises, because I *hoped* they'd be good — and they were.

There's a real tension. Because it's hard to judge effort when people use AI, one instinct is to repress it as much as possible — you design backwards from "what did they learn," and that pushes you to suppress AI. Sometimes you absolutely should: I run zero-tech classes, literally pen and paper. I used to allow tablets, but now that you can photograph and digitise handwriting with AI, a tablet's value as a writing tool has dropped, so I've moved to printed slides, pen and paper, zero tech.

So there's a divergence: sometimes you want people to use AI fully, sometimes zero AI. The messy middle is the problem. One risk is scale — with 500 students you can't run oral exams for everyone. Another, opposite risk is that people learn nothing because they rely on AI for everything, which is exactly why you need zero-tech environments too.

Overall, my fear is that universities won't allocate enough resources to deal with a vastly changed environment. What I keep advocating at my university is that we should *stop* doing some things and do much more on AI. If we have a hundred instructors, maybe we should have 95 and use the money to buy students six months of tokens from your favourite AI provider, then teach them how to use OpenRouter and run open-weight models on the cheap. Those are details — the big picture is reallocating resources: cutting some things to do much more to figure out what AI means for us. Not doing that is the biggest risk.

### How fast will it really change things?

**Eduardo:** Finish this sentence: by 2030, I think we'll be surprised that we spent so much time teaching students to ______.

**Gábor:** Wonderful question — and I have no idea. If I knew, I'd try to change it now. The AI era is maybe two years old; before that it was a toy. Arguably the real change — the kind that affects work — happened in the last six months to a year or two.

One thing economics teaches is that the effect of genuinely new technologies takes much longer than we think, because many of us live in a bubble — the same people talking about AGI arriving tomorrow, or the day after. Clearly this is an amazing technology, and there's a tail possibility — maybe 1%, 5%, 10% — that it becomes bigger than anything ever and changes our lives within five years. But the most likely outcome is that it's very important, comparable to electricity, the internet, or Zoom — maybe twice as important as the internet — and that it takes *decades* to deeply change how we work, because the human and organisational adoption bottlenecks are much bigger than people anticipate.

The hardest part of AI adoption isn't that your computer can't reach the model provider fast enough — that's not the barrier. The barrier is whether an organisation can completely rewire itself so the technology becomes part of everyday work and raises productivity. There's growing evidence people *do* more with AI, but whether it moves the bottom line is much more questionable right now. It will — but it'll take time, just as it took decades to see the internet's productivity gains.

My main scenario: it changes a lot, but more slowly than the bubble thinks, before the whole economy feels an impact that's genuinely different from other technologies. That doesn't mean the next five years won't bring fewer marketing assistants and, hopefully, more nurses, more people in healthcare, elementary education, or forestry — which would be good for humanity. There'll be fewer people in some knowledge-work jobs in developed economies, but people find different jobs: there used to be lift operators; there weren't yoga teachers until recently. New occupations appear. It's a very large shift, and its impact on education is huge because we're on the front line — but it'll take time to spread across the whole economy. We're just at the beginning.

### Gábor's own AI stack

**Eduardo:** Last, a personal question about your own productivity. How has AI affected it, and what's your preferred AI stack — what does Gábor actually use when he wants to get down to work with AI?

**Gábor:** I experimented with a bunch of tools. I mostly use **Claude Code**, though I use Gemini and ChatGPT for certain, often non-work tasks. For work I just use Claude Code — I'm not as much of a geek as you are, I don't want to experiment constantly or switch tools every month; it's good enough.

How has it affected me? I do a lot of "useless" side projects I wouldn't otherwise do, to experiment and have aha moments. I review and write more, which is a productivity increase. There's an interesting point some senior engineers have made: you're *supposed* to work less because of AI. But I'd now rather do things myself — write the code — than outsource to a research assistant I'd have hired in the past. So for certain tasks I don't hire people; I do it with AI, which means I work *more*. Am I more productive? Maybe. Do I work less? No — I do more, because instead of outsourcing I do it myself, and I take on more projects. I also do things that used to be too complicated: I'm not comfortable writing Python myself, but with AI I do text processing and work with text, where I have no formal training. So I use AI for many things — but has it completely changed what I do? I think the answer is no.

**Eduardo:** Back to augmentation.

**Gábor:** And the final point: honestly, a lot of what I do is still experimentation. Rather than bringing things into production or making a polished final product, I do a lot of prototyping — try something with AI, and if I like it, work on it more.

### Advice to students

**Eduardo:** What would you want students — or future students — listening to remember from this conversation?

**Gábor:** The number one point: AI can do a lot of things, but we don't exactly know what. So there's great room for experimentation. Be brave — do things you don't think you'd be able to do, then go back and understand as much as possible so you can judge the result. Experimentation is the most important skill, and it's how you figure out what works. If you have a supervisor or a university, try to get money to buy tokens and use it to experiment.

**Eduardo:** Gábor, that's all the time we have. Thank you very much for joining us — I'll see you around the hallways.

**Gábor:** Thanks a lot.

---

## Things mentioned

- **Textbook:** Békés, Gábor & Gábor Kézdi (2021): *Data Analysis for Business, Economics, and Policy*, Cambridge University Press — [gabors-data-analysis.com](https://gabors-data-analysis.com/)
- **Course:** *Data Analysis with AI* — [the open course materials](https://gabors-data-analysis.com/ai-course/)
- **Film:** *Arrival* (2016), dir. Denis Villeneuve — Gábor's running metaphor for how you develop "taste."
- **Tools mentioned:** Claude Code, ChatGPT, Gemini, [OpenRouter](https://openrouter.ai/), open-weight models.

*This page is a companion to the 2026 CEU podcast episode. The highlights and section headings are my own; the transcript is a lightly edited machine transcription, so treat quotations as close paraphrases unless checked against the audio.*
