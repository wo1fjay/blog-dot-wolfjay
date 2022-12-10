---
layout: post
title:  "Unstable Diffusion"
subtitle: "Some q's about responsibility in the age of AI art"
date:   2022-12-09 20:56:18 +1000
categories: wolfjay-lore
excerpt: "art, AI, and responsibility"
description: ""
type: article
content:
thumbnail:
color: "#3E5D36"
permalink: /unstable-diffusion
emoji: "👾 🚨 🌍"
---

My timelines were filled this week with artificial intelligence generated illustrations from comedians, musicians, friends, and family - **all very convincingly capturing their likenesses**.

I tried out a few text prompt based AI art generators a few months ago when they first started making waves online. It was possible to make some visually interesting images if you found a sweet spot in the text prompt system, but for the most part their images generated were careless, smeary messes.

What I was seeing now was **different**. Using an image based prompt system where the user uploads photos of themselves, the images I've seen from this new system are, despite being heavily stylised, distinctly recogniseable. They retain key details that make the user look like themselves. I recognised them instantly. They looked like my friends. **They looked like my family.**

Caught off guard by how far these tools had come in only a few months, I decided to take another look.

##### Part 1:
## Tool, or thief?

From my basic understanding and unscientific research, artificial intelligence systems work by analysing a data set, identifying patterns, then using that data to create rules to follow. A user gives it a prompt, either a word or a phrase or an image, and it generates something based on the prompt following the rules it's created.

**The more data the system has to work with, the more intricate the rules it can create, and the more detailed the result it generates will be.**

I've [read about cases](https://every.to/superorganizers/linus-lee-is-living-with-ai) where someone will feed an AI system with samples of their work, and use the system to augment and automate parts of their workflow. It seems like a very powerful and positive development. **But what happens when your work is included in a data set without your consent, and used to generate things against your best interests?** 

Just yesterday I opened Instagram to see @Carlosbob, an artist I follow, [posting about discovering that their work was in the latest release of LAION's image-text dataset](https://www.instagram.com/p/Cl7MkmABQ9-/).

![carlosbob-instagram](../../../../../assets/images/ai-art/carlosbob-instagram.jpg)

<figcaption>"Did a quick search and found that almost every painting I've ever shared has been used to train the Al that Lensa is using to create portraits. Lensa app is making a profit on stolen, uncredited and uncompensated art."</figcaption>

So what is AI? Is it a useful tool? Or a faceless thief? Will it make things better? Or way way way fucking worse. Does it even matter? **I tried to find out.**


##### Part 2:
## Unstable Diffusion.

### 🚨 ❶ Common Crawl

[Common Crawl](https://commoncrawl.org) is where it all starts, a non-profit with the aim of "democratizing access to web information by producing and maintaining an open repository of web crawl data that is universally accessible and analyzable".

Basically, they look at billions of sites and records that content in a big database, **which is free for anyone to access.**

### 🚨 ❷ LAION

The next step in the chain is [LAION](http://laion.ai) (Large-Scale Artificial Intelligence Open Network), another non-profit that looks up all the content that Common Crawl lists in its database. In particular, it looks at images and their descriptions and adds them to something called a 'dataset'.

In September 2022, visual artist Lapine [shared on Twitter](https://twitter.com/LapineDeLaTerre/status/1570889343845404672) that they had **found photos of themself taken privately for clinical documentation by a Doctor in 2013 on ['Have I Been Trained'](https://haveibeentrained.com)**, a tool created to help artists see if their art had been included in an AI system dataset.

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">🚩My face is in the <a href="https://twitter.com/hashtag/LAION?src=hash&amp;ref_src=twsrc%5Etfw">#LAION</a> dataset. In 2013 a doctor photographed my face as part of clinical documentation. He died in 2018 and somehow that image ended up somewhere online and then ended up in the dataset- the image that I signed a consent form for my doctor- not for a dataset. <a href="https://t.co/TrvjdZtyjD">pic.twitter.com/TrvjdZtyjD</a></p>&mdash; Lapine (@LapineDeLaTerre) <a href="https://twitter.com/LapineDeLaTerre/status/1570889343845404672?ref_src=twsrc%5Etfw">September 16, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
After the Doctors death in 2018, these images were stolen and published online, making them accessible by Common Crawl, which in turn meant they ended up in LAION's dataset.

That dataset currently contains **5 billion entries** of images and text descriptions. It's LAION's belief that if it is publicly accessible, it is appropriate to catalogue, **regardless of the content, it's copyright status, or any privacy concerns.**

**They have no moderation process** for what is entered into their dataset, and while they do accept requests to remove content, they only action requests if the content in question explicitly includes personally identifiable information like someones name, phone number, or address.

It is trivially easy to take content from LAION's dataset, **which they make available for free for anyone**, and cross reference it with other online services to quickly find someones personally identifiable information off just a photograph.

Feeling anxious yet?

### 🚨 ❸ Stability.ai

Stability.ai is the company resonsible for Stable Diffusion, currently one of the main image generating AI systems. They're currently valued at over $1 billion, and **distribute Stable Diffusion for free.**

**They use LAION's dataset to generate images, with no restrictions on what content can be created using their tools.** This includes applying their tool to image of people without their knowledge or consent to create pornographic or violent imagery.

Their founder, Emad Mostaque, told The Verge in September 22 that "ultimately, it’s peoples’ responsibility as to whether they are ethical, moral, and legal in how they operate this technology".

[They acknowldged](https://stability.ai/blog/stable-diffusion-public-release) when releasing the system to the public that it could be used to create unsafe content, but they hoped "everyone will use this in an ethical, moral and legal manner".

**They recently raised $101 million in their latest funding round to extend the scope of their tool to also include video and audio.**

### 🚨 ❹ Prisma Labs and their peers

While heaps companies have been able to build AI image generation tools that use Stable Diffusion due to its open source distribution, Prisma Labs' Lensa.ai is currently the most popular option.

Though Prisma Labs say they delete all user data after 24 hours, they also say that **they own the images you create. Forever. In perpetuity. With no way to opt out.**

In the past, **Prisma labs [received $2m in investment from Mail.ru](https://twitter.com/MildlyAmused/status/1598470417710469120/photo/3),** which was founded by Yuri Milner, who acted as an intermediary for **Vladimir Putin** to make large investments in Facebook and Twitter between 2009 and 2011. They now [claim on social media](https://twitter.com/PrismaAI/status/1598719118399705088?s=20&t=K7tWIcEmLymPMmZqsPhSig) that Mail.ru stopped investing in Prisma Labs in 2019, and that the company has no involvement in Russia.

**Another tool that offers this functionality, Different Diffusion Me,** looks like a basic web front end for Stable Diffusion, but **is actually run by Tencent,** the Chinese multinational technology and entertainment conglomerate also responsible for TikTok. Tencent last made facial recognition news in 2021 when it used it's tech to detect when underage users in China were attempting to avoid a state mandated digital curfew of 10pm.

##### Part 3:
## Bleak shit.

AI generated content is going to affect us all significantly in the very near future. **This is so much more than stylised avatars.** This is about what makes us ourselves.

For decades, we've been told to be active on platforms. To share our work, our process, our private lives, ourselves. And in return we'll be granted visibility. An audience. Attention. Maybe a career, or oppurtunities, or income, or fame.

**But what happens when all of that content, all of that imagery, all of those private details find their way into a dataset like LAION's?**

What happens when someone uses Spotify's vast database of music and metadata to extend your listening preferences with AI generated content? Maybe an AI won't create the song you open Spotify to listen to, but what about the song that plays automatically after that?

What happens when TikTok or Youtube start serving you supplementary content in the style of your favourite creator? Maybe they don't try to pretend it's them, but the avatar on your screen shares their face, or their voice?

![la-meme-young-spotify](../../../../../assets/images/ai-art/la-meme-young-spotify.jpg)

source: [La Meme Young on Instagram](https://www.instagram.com/p/Cl6pZqvO-j3/?igshid=YmMyMTA2M2Y=)

What happens when you start getting served ads that feature a model who shares physical traits with people you've swiped right on on dating apps, or someone wearing an item of clothing you've been looking at online, while music plays that sounds _almost_ like your current favourite song?

What happens to your privacy if someone can impersonate you almost perfectly online? Or can post content that you're not even sure you didn't post yourself?

What happens to the content we do post, if people become so used to their feeds being full of AI generated content? Will creators have to start emulating trends created by an AI system? What if AI generated content doesn't replace human created art, but people are happy enough with this new category of simplified and personalised content that they just aren't bothered with the extra messiness of something made by a human?

**What will our art be worth then?**

<!-- What happens to consumers of content if they become so hooked on tailor made content designed to ellicit a passive response so they keep consuming? When [criticised that they were censoring protest footage last year](https://www.buzzfeednews.com/article/ryanhatesthis/tiktok-users-are-finally-posting-about-hong-kong-but-only), TikTok said that the content wasn't proliferating across the platform because people just didn't want to see it. They preferred the sickly sweet, overly cheerful, non-critical, snack-sized content that the platform is known for. They had no interest in anything else.

**This is happening now.** -->

##### Part 4:
## Being online.

We aren't at that point yet, but it's not hard to imagine that future, and it'll be enabled by the way we act online now.

**What does it mean to "be online" if any action you take, or content you share, just helps an AI to become a better impersonation of you?**

If any participation you have in a platform just strengthens a system designed to impede a users ability to act in their own best interest?

In his talk ['How Designers Ruined The World'](https://www.youtube.com/watch?v=qIcM21l61TE), Mike Monteiro talks about the effect creating things without also taking responsibility for them can have on the world. "When designers disregard the effect their work has on our environment they are best negligible, and at worst culpable". When design is practiced without forethought to consequences, without responsibility, what we get is not creation - but destruction."

I see very little difference in this context between designers and anyone who is active online.

What responsibility do we have? To each other, and to ourselves?

##### Part 5:
## Where's the brain?

I have memories of visiting my Grandma as a child, having recently gotten a new gizmo or gadget. Maybe a Gameboy, or an iPod, or a digital camera. Every single time her reaction to these toys was the same. Caution, verging on disdain. 

After several years of being aware of this, she gave a justification. _"If you can't see where it's brain is, don't trust it."_

I realised that while, to me, it made sense how these pieces of technology functioned, and what allowed them to perform their functions, it must have been a mystery to my elderly Ukrainian grandmother. 

But I now realise that while those memories are still vivid, I have not remembered that lesson while growing up. **I am surrounded by and beholden to things that I absolutely do not understand.** Systems and processes that I've put blind faith in. Either to make money, or participate in a community, or just because it's what everyone else around me is doing.

My privacy conscious friends have warned me of certain products or fads, but my reaction has often been "oh well, if it goes bad I guess we'll all go down together". A fool. What I hadn't considered are the specific things in my life that are meaningful to me, and how quickly those things could be torn away from me using data I've handed over online without a second thought. 

I started this post wanting to better understand the mechanisms that are a part of AI systems, but upon finishing it I realise that **I need to better understand the systems I'm apart of.**

I started writing and researching yesterday morning, around 10:18am. I sat in my lounge room, next to my dog, with some music on. I moved to the kitchen in the afternoon. Today, I finished it off in my study. What have tech companies learned about me during that time? What data points of mine have been added to a dataset that may one day inform an AI system?

Maybe they know from the ambient sensors in my tablet that I've had the lights off, but the curtains open.

Maybe they know from the white noise coming through the microphone in my smartphone that I've had the air conditioner on./

Maybe they know from the photo I sent a friend this morning that I'm wearing activewear, despite my smartwatch showing I've barely made any progress on my activitiy goals for the day.

**How will this information be used?** Will I see more Nike products in my timelines this week? Will I be shown different jobs from recruiters to apply for? Will my utility premiums increase because my provider can see I'm spending more time at home? Maybe my health insurance premiums will go up because I've been less active than normal.

**Of all of these systems, I can definitely start saying no to the obviously superflous ones; the ones asking for my personal data in exchange for some anime avatars.**

I can practice being more critical. I can begin to question if the systems around me are actually serving me, or the communities I'm a part of, or the art I want to create and surround myself with.

And if not?

## **Fuck off.**