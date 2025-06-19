---
slug: devtoolsguild-origin-story
title: Dev Tools Guild origin story
authors: [conor]
tags: [launch]
---

# Dev Tools Guild Origin Story

_**TLDR**: Origin story of Web3j in 2016 and Dev Tools Guild launching today._

After almost a year of coordination, we're finally ready to announce the Dev Tools Guild (DTG)  to the world.

Composed of many of the teams responsible for the core infrastructure powering developers building Ethereum, the Dev Tools Guild has been established to accelerate the development of DApps on Ethereum.

<!-- truncate -->

Whilst the goals of Guild are driven by supporting Ethereum's DApp ecosystem, my own personal interests in getting the Guild going have been driven by my own personal experience with open source software.

It is my belief that guild structures can provide a more sustainable foundation for providing long-term sustainable funding for open source software. I will return to how we get there shortly, but first some background.

## The Power of Open Source

In the 1990's we had proprietary UNIX operating systems powering the majority of the world's servers, with Sun Microsystems, IBM and Hewlett-Packard dominating the landscape.

Linux emerged during this period, an open-source UNIX variant, written by coders and hackers who believed in the importance of free software that was available to all.

At this point, I was just starting out in my professional career and was learning everything I could about Sun's Solaris OS. I was aware of Linux, but given the dominance of Sun and others, this felt like a safer commercial bet.

I attended Solaris user groups in London, getting excited by the big innovations that were happening, such as their dynamic tracing framework (D-Trace) which dynamically instrumented kernel tracing to understand what was happening in real-time in production systems.

However, as exciting as all of this was, I hadn't been paying attention to the growth of Linux emerging from the sidelines.

To compete with Linux, Sun Microsystems decided to open source Solaris, to much fanfare. However, it was too little, too late. Over time we saw Solaris fade into obscurity and Linux establishing itself as the dominant server OS, powering significant portions of the internet.

This lesson really struck a chord with me, as it taught me to never bet against the power of community.

## The Origin of Web3j

Fast forward to 2016, I stumbled across Ethereum. I'd been aware of Bitcoin, but it had never captured my imagination due to its more narrow focus of being a decentralised digital currency.

Ethereum, on the other hand, fascinated me — a programmable world computer. I wanted to find a way to contribute to this vibrant and emerging ecosystem.

This contribution opportunity emerged with Web3j — the Java and Android integration library for Ethereum, which I started in September 2016 and announced to the world shortly after. I'd spent years working with large financial institutions, building on the Java Virtual Machine (JVM), and it seemed a no-brainer that there would be demand to link these corporate systems up with Ethereum, given how much they were touting blockchain as a solution to many of their woes.

Web3j started off as a passion project. I'd always wanted to create meaningful open-source software, and I was fortunate that the library gained traction and adoption. People were creating issues, submitting pull requests and asking questions in our Gitter chat room. I was maintaining it as a side project, then in the summer of 2017, I created Web3 Labs with a view to commercialise it.

## Sustaining OSS is Hard

The problem was, no-one wants to pay for open source software such as integration libraries. It's commodity software, like a database driver which you expect to be readily available for your project.

Having created Web3j opened plenty of doors in the web3  ecosystem, and enabled Web3 Labs to survive primarily on consulting services. However, doing this work alongside sustaining Web3j was a balancing act as commercial opportunities always needed to be prioritised to keep the lights on.

Fortunately over the years, via a number of different grant programs, Web3j has qualified for additional funding which has helped us to sustain a couple of dedicated developers working on the project. However, this funding has been lumpy and been over-reliant on the Ethereum Foundation.

Abandoning Web3j has never been a consideration. As long as there's a community of users, I view it as systemically important software for Ethereum. The Android operating system powers significant numbers of the world's smartphones, and Java is still consistently one of the most widely used programming languages in the world.

Although the majority of DApps are written using JavaScript/Typescript, adequate support for other platforms is paramount to ensuring Ethereum's accessibility to the widest possible number of developers — especially those in corporations still relying heavily on the JVM and those building on Android.

In the beginning of 2024, we decided to propose Web3j become a Linux Decentralised Trust Foundation (LDTF), (formerly Hyperledger) project. The reason being that LDTF, like the Apache Software Foundation and Cloud Native Foundation and others under the Linux Foundation, provided high standards of governance for OSS, which given Web3j's maturity we believed to be a good home to help sustain the project for the long run.

The only issue is, software foundations, whilst great for visibility and governance processes, projects are still on their own when it comes to funding them.

## Why Value Accrual For Open Source is Broken

The primary beneficiaries of open source are with the enterprises that have used it to replace proprietary systems.

The consultancies and system integrators these businesses pay to develop these solutions based on this free software. And finally the software foundations that enterprises pay hundreds of thousands of dollars to, none of which makes its way down to the individuals developing and maintaining the software.

Hence much of the value accrual from open source lies with the enterprises and system integrators who use it, and the software foundations who promote it.

Some of these organisations may pay developers of open source for auxiliary services such as training or support, but this tends to cover a small proportion of what it takes to produce and maintain this software.

This isn't an attack on any of these groups, but just the world we find ourselves in. Open source may have eaten the world, but its developers are still starving.

## Standing on the Shoulders of Giants

During 2024, as another of our grants from the Ethereum Foundation was coming close to ending, yet again I found myself thinking, there has to be a better way to sustain Web3j.

I'd been aware of the Protocol Guild for some time. It was incredible to see them reach a place of nirvana by providing a funding model to help sustain the ongoing development of Ethereum clients.

Their model appeared to offer exactly what Web3j really needed — a meaningful amount of funding to help sustain the library over a multi-year time horizon.

The thing was, I couldn't see a path through the trees. Protocol Guild was narrowly focussed on Ethereum client development and core protocol R\&D, not developer tooling.

This changed when I stumbled across a [post by Trent,](https://trent.mirror.xyz/MsXtV_TGZHp05FN_qmzeT8bBc1lRghR3Y0TPvAd-WrA) creator of Protocol Guild mid-way through last year. In this post Trent lays out some of the opportunities and challenges for Guild structures, and also suggested what a Dev Tools Guild could look like.

With this post I had a blueprint of what needed to happen, and I promised myself that I was going to do everything in my power to make a Dev Tools Guild happen.

After reaching out to Trent, he introduced me to folk at Gitcoin who were interested in the Dev Tools Guild idea. Between us we started bringing teams together on Telegram and I started working on coordinating teams and figuring out the what, why and how of this project.

We had a face to face get together for a number of teams in Bangkok during Devcon and since then we've been hard at work building up to the launch.

We've been fortunate to have support from Trent and Cheeky of Protocol Guild who have enabled us to mirror aspects of how they operate, but do some things differently where it makes sense.

But most importantly, the DTG would not exist were it not for their work with Protocol Guild, and Trent sharing his thoughts on what some other Guilds could look like.

## Back to the Guild Again

The mission of the DTG is *to accelerate Ethereum app development via world-class tooling.*

These are underpinned by the following values:

* We provide public goods for Ethereum.  
* We collaborate for the good of the ecosystem.  
* We measure success by impact, not profit.  
* We act with integrity and transparency.  
* We lower the barriers to entry for developers to build on Ethereum.  
* We champion a diverse ecosystem of languages, frameworks, and developer communities.

We want to see Ethereum's DApps ecosystem thrive via increased coordination among members as well as with the core protocol. In addition, we want to provide sustainable funding for public good OSS. This latter point is something that is not a solved problem both inside and outside of Web3, and we are hopeful of the DTG (and PG) being trailblazers in this regard.

This ties into my own definition of what success looks like for the Dev Tools Guild. I wish to see the DTG obtain enough funding to sustain its member projects independently of whether the organisation responsible for it continues to exist or not.

Public good OSS need not rely solely on organisations or armies of volunteers to sustain it, it should have robust incentives in place that reward contributors financially for their work, and continue to reward for as long as they dedicate their time and resources to it.

Guild's have the ability to sustain such *funding of the commons* as Trent would say, as the impact of their whole is so much greater than the sum of their parts. They also provide a filter via their membership criteria and governance to ensure their membership remains relevant and impactful in the ecosystem they serve.

The Dev Tools Guild may just be getting started, but it's building a foundation that has the potential for reach and impact in not just the web3 ecosystem, but open source as a whole.

**Donations of all sizes are greatly appreciated.  Donate to [donate.devtoolsguild.eth](https://etherscan.io/address/donate.devtoolsguild.eth).**




