- [<] Status Log
	- created:: 2021-07-08
	- status-updated:: 2022-03-18
	- current-status:: #nonfic/evergreen 
- [S] Marketing
	- purpose:: Have something to link to when people ask me how self-hosting [[Ghost publishing platform]] for the [[Obsidian Roundup]] went. 
	- Link:: [Ghost Tips: My Experiences Running a Self-Hosted Newsletter » Eleanor Konik](https://eleanorkonik.com/ghost-my-experiences-running-a-self-hosted-newsletter/)

When I started [the Obsidian Roundup](https://obsidianroundup.org/), I had two primary motivations. First, I wanted to help out people who had a lot to contribute to the [Obsidian.md](https://obsidian.md/) community but didn’t have time to keep up with the firehose of (very useful!) information in the community Discord, for example plugin developers. Second, I wanted to check out [Ghost](http://ghost.io/), which I heard about during a [period of controversy surrounding Substack](https://www.wired.com/story/ghost-substack-platforms-publishers/). I was never going to join Substack (I like controlling my own “branding” too much), but it seemed like a nice alternative to MailerLite, which was what I had settled on for my [Monday Morning Research Roundup](https://eleanorkonik.com/subscribe/) (which is due for a rebrand actually, I have too many “Roundups” now, even tho MMRR came first) but caps out at 1k subscribers for the free tier. 

A bunch of people told me it was great, super easy, so nice–but those people were using the managed hosting option, and at $9/mo for up to 1k members, it would be significantly more expensive than Mailerlite. Some other folks said they self-hosted it and it was great, but these are also the same people who think nothing of using git or [pandoc](https://pandoc.org/) or any other command line interface tool that I had never heard of six months ago. 

I like saving money, though, and I figured if I ran into too much trouble _somebody_ would help me, so I dove in. Here’s a compilation of what I learned, compiled for your reading pleasure and in hopes that it helps someone else out who has been thinking about trying out Ghost. 

## Step 1: Finding a Host

I spent a hilarious amount of time reaching out to various webhosts to do price comparisons (since I was also planning to migrate my personal website sometime soon, as Siteground’s customer service has gotten a lot more difficult to access over the years, and paying a premium for customer service is only worthwhile when you’re getting premiere customer service) and most regular web hosts don’t really do server hosting too. So the first thing to realize when deciding to go with Ghost is that you aren’t going to be able to use a normal webhost like GoDaddy or whatever, you need someone that will let you have a whole server thing.

Not many services have a one-click-install for Ghost, and of the ones that do, I prefer DigitalOcean. Most people I know use it, it’s super cheap, and they have a nice little referral program that lets you have plenty of seed money to mess around with. [This link](https://m.do.co/c/fbd625dd9f32) will give you a $100 credit that you have 60 days to spend, which is more than enough time to figure out whether you like it. 

## Step 2: Setting Up

The big thing I didn’t know when I was setting up my ghost installation on DigitalOcean was that a digital ocean droplet is _an entire server,_ not just a widget or app or program or whatever like I was used to from places like SiteGround, so I accidentally paid for two droplets (one for my wordpress site, one for my ghost blog) which is totally unnecessary. At $5/mo (of free money) this isn’t a crisis, but nonetheless, learn from my mistakes. 

I followed [this step by step guide](https://www.codeclouds.com/blog/setting-up-ghost-with-digitalocean-a-step-by-step-guide/) that, shockingly, was actually pretty good. The most fraught part is waiting for the DNS stuff to take effect, but that’s true whenever you’re doing anything with domain names, and since Digital Ocean doesn’t handle domain names for you, you’ll need to purchase one elsewhere and point it to your new server. I recommend [Gandi.net](https://www.gandi.net/) mostly because it’s no frills, their customer service people are very patient, and they don’t try to sell you any unnecessary crap. 

There were two main things that I don’t think that guide called enough attention to, though, probably because they assumed it was obvious. The number of times I have tried to follow a technical guide on the internet and run into trouble because of something that would have been obvious to a professional programmer but was very much not obvious to me (sudo bash commands are only for Linux, but sudo bash commands are being provided in Windows installation directions, wut? whyyyyy). Anyway: 

In order to [set up mailgun](https://ghost.org/docs/config/#mail) (resources [here](https://xtabbas.com/how-to-setup-mailgun-for-your-ghost-blog-and-start-sending-out-newsletters/) & [here](https://bironthemes.com/blog/ghost-mailgun-config/)) so that your ghost blog actually functions as a newsletter and not just a blog, you need root access to the `config.production.json` (or, I don’t know, maybe you don’t, but this was the method I found and I needed help from my husband for this part) which is fine and dandy and you _can_ do that through the [ghost command line tool](https://ghost.org/docs/ghost-cli/), but you can also use a program called WinSCP to access the file system. 

PS: For the command line tool, when you’re reloading your ghost installation (which you have to do a terrifying number of times, messing with live servers is terrifying, it’s my least favorite part of Ghost), you have to navigate to `var/www/ghost` before you reload. 

## Reaction to Setting Up

So, for context, I am a neophyte developer with one hacked together Obsidian theme and one plugin that a **lot** of people helped me with under my belt. I’ve technically got a ghost installation running on my local machine (more on that in a moment) and that’s a “developers-only” tool, so, sure, fine, we can call me a developer in the technical sense. But my day job is middle school teacher and my hobby is writing fiction; I’m not even an experienced hobbyist. 

Rolling my own ghost blog was not easy. Self-hosting WordPress is a breeze by comparison. I’m pretty sure that publishing a website using a static site generator like Hugo using git would have been easier. Digging through the mailgun documentation, figuring out the ghost CLI stuff, etc took me like three days of constant poking, and I _never_ would have succeeded without my husband’s intervention at critical moments. If you’re a non-technical user just trying to run a cheap newsletter, use Substack. If you object to Substack’s business model or ethics, check out [Buttondown](https://buttondown.email/). If you really, really want your newsletter emails to come from your own custom domain on the cheap, while also being able to control what it looks like, and want them to be available through RSS on the web, and it matters to you a lot that you can do paid subscriptions? Ghost is a good way to go. 

But! It’s not *easy.*

## The VS

Though it bills itself as a Wordpress replacement, I think their claims are a little unfair. Ghost’s “managed hosting” is cheaper than Wordpress’ technically, but only if you count “managed hosting” to mean _literally hosted by Wordpress_. Hosts like Siteground will manage your Wordpress installation for _way_ cheaper (and still super easy) than $9/mo, and “self-hosting” Wordpress is _so much easier_ than self-hosting Ghost that anyone seriously evaluating whether to use Wordpress or Ghost just shouldn’t even bother looking at the comparison chart. 

When comparing self-hosted Ghost to self-hosted Wordpress, Wordpress comes out on top for *blogging*, in my opinion. There are _way_ more free themes, the plugins are actually easy to use, there are more plugins and the plugins actually help you with SEO (the Yoast free tier is great), and the search actually works out of the box. You don’t have to fight with APIs or read obscure documentation to do every little thing. 

But even aside from the technical difficulty stuff, the Ghost UI is lacking in some fairly shocking ways. The Wordpress sidebar where I can set metadata like tags and schedule a post is always open. Ghost prefers to give me a “clean” writing interface, which, sure okay fine I guess some people write directly into their browser when they’re composing (I write all my newsletters in Obsidian, personally). But when I toggle open the sidebar in Ghost to assign tags and metadata *I then can’t seem to scroll up or down on the post*, which means I can’t skim my post to remind myself what my tags should be without toggling closed the sidebar, scrolling, re-opening the sidebar, navigating to the section I want… you get the idea. So what ends up happening is that I have my notetaking app where I wrote the newsletter open in one window, and then scroll _it_ while assigning tags – which, by the way, I seem unable to navigate to the beginning of the list to insert tags there instead of at the end, which would be fine except a lot of themes seem to use the first tag to indicate category. Having to delete all of the tags I’ve assigned (I wasn’t able to copy them) and then re-type everything just because I wanted to insert one at the beginning isn’t fun. 

It’s little things like that where I get frustrated at all the hype. I know it’s FOSS software and I can just submit a pull request or “fix it myself,” so I’m not trying to complain at the developers (don’t look a gift horse in the mouth and all that), I just find it frustrating how it gets shilled as this amazing perfect modern thing. I mean, it’s been around for almost a decade, but when I was typing into the editor, the my usual “undo” hotkey worked fine but “redo” didn’t, and boy howdy was that distracting. 

Also: the Wordpress dashboard is customizable and useful. I can get a nice overview of recent comments, draft right into an empty textbox, click to open my recent drafts, etc. Ghost gives me a chart of member signups and membership information, and a bunch of marketing articles that I can’t get rid of. It’s basically one big advertisement for the “correct” way to run a newsletter, with helpful examples that feel like product placements for things I don’t want. I hate it. Eventually I’ll probably dig into the source code to get rid of it, but I would much prefer to have a little “x” to clear the nagging lessons on branding that I don’t want to read. 

Who knows, though, maybe all of this is just classic PEBKAC and grumpiness. A lot of people really do seem to love it, and with reason: it very good at being the thing it’s very good at. 

## The Good

It’s not really better than Wordpress at a lot of things, it doesn’t have proper membership tiers like Patreon, it’s a technical pain in the butt to use and it costs more than Substack or Buttondown–so why am I using it? 

I get the impression that Ghost has lot of hype from their marketing department because they make their money from their (frankly kind of expensive by my standards) managed hosting options, but on the self-hosting end, it’s the cheapest option out there that I’m aware of that lets me control everything, and that matters to me a lot. Mostly the cheap part, if I’m being honest, but only because the Roundup has over a thousand subscribers and I wanted a custom domain and an easy way for people to help me pay for the costs of running it. 

Ghost is pretty good at its one specific niche: being a highly customizable cheap newsletter solution for technically skilled users who want to own their own data, have paid memberships, a bunch of API options (do _not_ make the mistake of confusing the “integrations” with plugins), and a clean interface that doesn’t let you get “bloated” but also isn’t going to hold your hand for things like keyword density or version control or anything really. 

It’s not horrible or anything, I just feel like it’s a bit overhyped. I would not embark upon this path unless you are a developer, are very close with someone with a lot of development experience who will hold your hand. 

## Local Development

If you’re planning to roll a self-hosted option on your local computer just to try it out (or, you know, play around with editing themes somewhere _other_ than your live server environment that has to be restarted every time you want to look at your updated CSS), beware that the developer version is pretty limited. You can’t experiment with what the newsletters will look like because you need to be hooked up to mailgun before they’ll even let you preview a newsletter, for example. Also: the documentation currently says that it will work with NodeJS version 14.x.x but this is outdated: you actually need 14.17 – 14.15 didn’t work when I tried to do this, and I spent a fair amount of time banging my head against Google search results trying to figure out how to get npm to let me upgrade NodeJS before ~~I~~ my husband realized that NodeJS can be upgraded on Windows with a one-click-install GUI option. 

Anyway. It’s been a wild ride and I’m not sorry I did it, but a couple of people have asked me how using Ghost has been going for me and which guides I used to get it started, and I don’t want to give a false impression that it’s easy for nontechnical users just because my reputation in the Obsidian community is more on the academic side than the programmer side of things. 