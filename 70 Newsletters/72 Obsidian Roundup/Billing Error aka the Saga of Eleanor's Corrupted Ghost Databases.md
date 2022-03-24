- [<] Status Log
	- created:: [[2021-09-12]]
	- status-updated:: [[2022-03-18]]
	- current-status:: #nonfic/evergreen 
- [S] Marketing
	- purpose:: explain a problem with the [[Ghost publishing platform]] to subscribers of the [[Obsidian Roundup]]

I'm sending you this email on a Sunday (not a usual newsletter day) because I found a corner case with my newsletter provider (Ghost) that led my subscriber database to become hopelessly corrupted. Don't panic — the only people really hurt by this are myself and my poor husband, who spent about a week helping me track down the problem and try to troubleshoot bug reports and potential solutions.

**The tl;dr is that if you probably won't be able to log in to The Iceberg and The Obsidian Roundup for at least part of today. All paid subscriber accounts for The Iceberg (and probably some for the Obsidian Roundup, I haven't been able to run tests because of technical reasons) are about to be flagged with a free, complementary, lifetime subscription to whichever of my newsletters I have a record of you having subscribed to.**

The records are hopelessly entertwined, though, so if you could double-check sometime, say, Monday or Tuesday, to make sure your account(s) are set up the way it should be, that would be great. 

If you're annoyed you didn't win this delightful lottery for the Obsidian Roundup, I have good news: it was always free (sorry if that wasn't obvious 😅 I tried to make it clear but I was bad at modifying themes in the early days) and you can cancel your subscription any time and still get the information via email, RSS, or just visiting the website once a week. For obvious reasons I kind of hope you don't, though, since my monthly revenue is about to get slashed to the ground 🙃 

If you feel bad about this and would like to give me money anyway (I use it for supporting other developers, paying for tech support and themes, and things like book covers / editing — not food. I am not going to starve because of this, please don't worry about anything except my sanity), I'll share some steps down below for workarounds, but first, let me tell you what happened because otherwise it won't make sense what you're working around.

Buckle up, it's a mess. 

## First There Were None

The Iceberg began life as a mailing list run off of the free tier of mailerlite, and for the first eight months or so it was called "the Monday Morning Research Roundup" and this was fine. But I found myself wanting to link to past issues when they came up in conversation, and the mailerlite link preview mechanism was a little awkward and painful. I eventually heard of substack, but I also heard there were some controversies, and I didn't really like the lack of customization options or want to be permanently associated with the substack brand, which I have no control over. I'd heard of Ghost, but wasn't really ready to switch over to it, because switching is always harder than starting from scratch. 

So when a member of the Obsidian.md Discord server asked for a newsletter to help summarize major developments in the Obsidian community — where the state of the meta can charge a lot in just a few days, as plugins get made, themes get updated, and workflows get shared pretty constantly — I jumped on the chance to learn more about running a newsletter on Ghost. 

## To Self Host or Not to Self Host

There was always a possibility that other people might help out with the Roundup — what if I went back to work and couldn't maintain it, or got pregnant and needed to take a couple of months off, or it made sense to run two editions of it? At the time I was setting up the Roundup it would have cost $80/mo for managed hosting that let me have one additional user, because the tier that allowed for it was intended at big group newsletter consortiums and newsrooms. I assumed (somewhat naively in retrospect, you all are amazing) that I would be paying for the hosting costs totally out of pocket and was leery of committing that much money to something I wasn't sure would ever see more than 20 readers. 

Most newsletters cap their free tiers at 1000 users, and I was hopeful that my personal newsletter might one day surpass that, so it seemed like a good opportunity to try out what was, to the best of my knowledge, the cheapest decent way to run a newsletter. 

I was a little nervous about self-hosting, but I've been self-hosting Wordpress for years with only minimal problems— (like the one time I ran an update that made it impossible for me to actually access my website from the web at all 🙃 — and, well, the Obsidian community is full of helpful developers so I figured that if I ran into too big of a pickle, somebody would help me out. It was to be a grand experiment! 

## It Went Pretty Well

Honestly [the problems I ran into with setting up Ghost](https://eleanorkonik.com/ghost-my-experiences-running-a-self-hosted-newsletter/) weren't that bad. I wouldn't recommend it to non-technical users, but I was right about being able to lean on my community for help and I learned a lot. I learned how to edit SCSS so I could change the theme, I learned about how email _really_ works, I learned how to use a terminal to access a server, it was pretty cool. A bit over my head at times, but I'm married to a professional software developer and in some ways it was kind of a neat bonding experience. 

So I went ahead and made my fatal mistake. 

## A Tale of Two Ghosts

When I installed Ghost for the Roundup, I used the one-click installer for Digital Ocean and it went... mostly fine. But I'd heard that you could run more than one thing on a single Digital Ocean server and felt pretty dumb for paying $6/mo per server when I thought I didn't need to, so I asked my husband for help putting my worldbuilding research newsletter — now rebranded as the Iceberg —  on the same droplet (server). I wanted this mostly because I wanted them both to be under the same domain name, which is to say the newsletter would be a subdomain of eleanorkonik.com 

This was super complicated and without going into more details, a terrible idea because we wound up having to upgrade the server size anyway, otherwise I ran out of memory and had horrible performance. There were easier ways to do this and I should have used them. Happily, doing it this way didn't actually break anything — I swear. 

No, my mistake was thinking that the Roundup and the Iceberg were both "products" under my "Eleanor Konik" brand and therefore _related from a business perspective_. 

## Enter, Stripe. 

Stripe is the credit card processor that handles payments for Ghost newsletters and Obsidian, too. To the best of my knowledge they have the cheapest processing fees and are therefore pretty popular. On their FAQ, they're pretty clear that you should use separate "business accounts" (inside of your "dashboard" account) for unrelated businesses. But to my mind, the Roundup and the Iceberg are related insofar as they're the two of the three things that most strongly "build my brand," the latter being the articles I share on my wordpress site. 

I uh, I don't know if you know this, but Eleanor Konik isn't my real name. I'm a teacher do you think I want kids Googling me? 

Anyway, the Ghost interface let me connect the Iceberg membersehips to a product called "The Iceberg" under my Eleanorkonik account on Stripe and all seemed fine. Some of the numbers seemed a little weird (which is to say: low) at first, but I'm kind of bad at remembering numbers and figured I was just doing the mental math wrong for how the yearly discount was lowering the price and of course there are Stripe fees... but eventually I realized:

Wait no, something is really wrong. 

Specifically, Stripe was reporting a monthly recurring revenue amount that was roughly a third of what Ghost was reporting and by the end of the first month of the Iceberg having a paid tier for extra content, aka short fiction and analysis pieces a little more "open" than I would normally be on the internet, there was enough expected revenue that the numbers were big enough for me to notice the discrepancy. 

## Missing Subscribers

Around this time, Stripe was reporting about 20 recurring subscribers to the Iceberg while Ghost was reporting closer to 90. Crap! So I checked the Roundup, thinking that maybe they'd somehow gotten sent over there. 

Well, that was definitely part of it! Some of the subscribers to the $2 tier of the Iceberg had been charged for the $1 Roundup "product." But I also had about 15 fewer paid subscribers to the Roundup in the Stripe — definitely people missing, but a different percentage. How strange. All told, there were fifty people who Ghost thought were subscribed but Stripe had _no record of_. 

Which is bad. 

For what I hope are obvious reasons but totally aside from the missing money I was terrified that this cross-pollination between newsletters was breaking people's accounts, and it definitely meant that every time I logged in and was confronted with the Ghost dashboard that I can't (easily) change (well, I can but it won't persist between updates and would be a nightmare) to turn off the money/membership tracking  information, every time I logged into either of my newsletters to write I was confronted with these weird, unreliable numbers, which drove me kind of nuts. 

I like things organized, yanno? 

## Tech Support

I reached out to stripe first, since Stripe actually makes money from these transactions and Ghost is pretty up front about self-hosting being an unsupported option intended for skilled developers who are expected to figure out their own solutions to problems (although I've always gotten help when I showed up hat in hand to help, I have done enough tier one tech support for Obsidian that I wanted to be able to give them a comprehensive bug report when it was time). 

Stripe has a helpful little chat button on the dashboard, but when I clicked it and tried to share information with the nice tier one tech support person, I immediately ran into a problem (because of course I did, are you getting a feel for this yet?). The chat software wouldn't let me upload attachments, even though the functionality was right there and the file sizes I was using were tiny. So we had to switch to email, which is much clunkier, but turned out to be fine because all tier one tech support could really do was acknowledge that something sure was hinky and assure me that they were forwarding my problem to tier two tech support, aka someone who could help. 

Eventually. 

After I hadn't heard anything from Stripe for a couple of days — and after talking through things with some of the Obsidian moderators and nice folks in the Ghost community — I decided I had enough information file a bug report with Ghost. You can read it [in all its earnest glory](https://forum.ghost.org/t/incorrect-billing-amounts-with-multiple-instances-of-ghost/25415) on their forum if you're so inclined. 

Basically, I finally had a theory: connecting two stripe products under the same _account name_ to two different ghost newsletters is a weird corner case that you're supposed to be smart enough to not do and also who seriously runs two tonally different newsletters under the same branding effort, anyway? 

😳

## The Hope

Around this time, Stripe got back to me with a variation of "hey sorry this sounds like a Ghost problem, not an us problem," which... seemed true, honestly, so I didn't push. 

By this point I had an inkling of a plan: I could nuke the database for the Iceberg back to the ground, reset to 0 MMR. But wouldn't it be nice if I didn't have to? If I could somehow prune back just the corrupted/incorrect stuff and keep the _accurate_ records of subscriptions, then export it, disconnect stripe from Ghost, move the stripe product over to a new account like I should have done in the first place apparently, and then reimport? 

Alas, the kind staffers at Ghost dashed my dreams. Again, they are not actually making a cent off of me using their software, I am a free rider, I hold them no will-will whatsoever, broadly speaking Ghost is an amazing program that does what I want it to do, which is connect with you all — and looks pretty slick, too!

The staffers shared a link: somebody back in March ran into a similar problem... except much worse 😬 I think his subscribers were erroneously getting charged for _expensive_ things. From what I can tell everyone impacted by this got billed less than they signed up for, i.e. the Roundup price instead of the Iceberg price. Anyway, the solution to this problem was basically "well, you can manually delete one by one, or if you're comfortable with databases, you can nuke it all at once using mysql." 

Yay? 

## A Learning Experience 

So I spent all night Friday looking at the mysql databases in Ghost. Which is to say, my husband showed me how to do mysql queries of a database via the terminal. Then we cross-referenced the member information and product information and emails against the Stripe database. We used a frankly exhausting combination of Excel sheets and vlookups, which I had never heard of, but I guess might ever come in handy if I need to do something complicated in excel one day. 

Once we had the data laid out in front of us (which took roughly three hours) we were able to confirm that the problem started happening around the time I hooked up the Iceberg to Stripe. We were also able to confirm that subscribers to the Iceberg who were _only_ subscribed to the Iceberg (and were not paying for the Roundup) had corrupted data, i.e. were listed as customers of the Roundup in Stripe's database.

For those still following along at home (or wherever, I guess), this is bad because it means I can't just delete the Iceberg product and move on with my life — the list of subscribers to the Obsidian Roundup product in Stripe is _also_ incorrect. 

## The Faint Hope

Now that ~~I~~ my husband understood how the Ghost database worked, we had a dim hope that we could maybe hack Ghost to let us disconnect from stripe _without_ having deleted all of the member subscription data, but it would only work if Stripe could be convinced to help. Which was frankly unlikely, there are super good reasons that you're not supposed to mess around with that data — it's a great way to corrupt your database 🙃 

But come on. At this point it was worth a shot, right? 

So I reached out to my point of contact at Stripe in the faint hope that they could somehow move the uncorrupted stuff over to a new product on the new account (or the old product onto the new account, whatever) but alas, it was not possible. 

Which brings me to the reason for this email. 

## Nuking the Database

The only way I can figure out to resolve this is to delete all of the Iceberg's paid subscribers, disconnect from Stripe, delete all of the Iceberg-related entries in Stripe, create a new Stripe product under a new subaccount thing, re-connect to Stripe, re-import all of my paid subscribers, and then go through and manually give everyone a complementary subscription. I may or may not need to do the same thing to the Obsidian Roundup membership database, but either way it's going to involve a lot of cross-checks and on-the-fly troubleshooting. 

**If you are subscribed to The Iceberg and do not get the free Monday morning email that summarizes my research into obscure historical and biological facts about _cheese_ please view it on [the website](http://newsletter.eleanorkonik.com/) instead. If you don't get an email _next_ week, please reach out to me so I can fix whatever has gone wrong.** I have every intention of having this fixed before I go to bed tonight, but just in case, I want there to be a workaround available. 

## Upgrading from Complementary 

The only problem with giving everyone a complementary yearly subscription is that there is literally no way for users to cancel this subscription or upgrade to a paid subscription in any rational way. If you cancel the complementary subscription, it will run out _this time next year_ at which point you'll just ... stop getting premium emails, I guess. I have no way if knowing if you'll get warned about this, because for obvious reasons I can't wait a year for testing 🙃 there is no monthly complementary subscription option. 

The design of Ghost sort of assumes that you're doing one very specific thing and if you try to do something other than that one specific thing, you're on your own. 

So! Workarounds. They're painful, but I promised: 

In theory you can just make a new account with a different email address, if you're like me and have multiple email accounts filtering into the same inbox, and then pick an account to "unsubscribe from emails" from. Bonus points if you send me an email with the account you'd like me to delete from my end, because hahaha I discovered during the course of this that [you can't delete your subscriber account in Ghost](https://forum.ghost.org/t/letting-members-delete-their-accounts/20187)... and I'd prefer not to have duplicate accounts giving me a bloated number for how many folks are signed up, since I have this dream of launching on ProductHunt if I ever get to a thousand members for the Iceberg. 

If you're a one-email-for-life kind of person, you can (**tomorrow please**) log in to your newsletter of choice by either:

*  _Make sure javascript is enabled_ (if you don't know what that means, you're fine) and click the `+ Membership` (the Iceberg) or the Subscribe (Obsidian Roundup) button, click sign in, follow the directions, get back to that section (the account modal will be your gravatar icon) and change your email there. 
* If you don't want to enable javascript because you don't trust Ghost (...fair), you can click the `Sign in` button at the top, `change billing information` and then click "back" at which point it will finally let you edit your email address. 🙃 Want to guess how long that took me to figure out? 

Once you're able to change your email address of record, make a dummyaccount like `deleteme28365@sharklasers.com` (don't literally use that one). Sharklasers.com is great for dummy accounts, but you do need to be able to check the inbox once so you can confirm the email you're switching your complementary account to. Then, in theory, you can create a _new_ account with your real email (the one you've been using all this time) and whatever subscription you feel like signing up for. **Please do not feel like you need to do this. I am fine if you stay on the complementary email, triply so if you have a credit card statement saying you paid me. If you paid through Stripe and your credit card reflects this, I probably did actually get the money. Only some payments were underpaid or lost in the ether.**

I am including this section because I expect questions about it and in an effort to be thorough, because you are all so nice, not because I need this money to not starve. I will not starve because of this. It's just bad for my ego and might just take a little longer to save up for a fancy book cover, which is fine. Honestly, I'm gratified to have readers at all, and the nicest thing you can do for me is share my newsletters and articles with friends who might be interested in the content (**tomorrow please**), or reach out with a link if you come across something you think _I_ might find interesting.

That said, if you'd like to sponsor my work but no longer trust my Ghost database (which is ... fair), you're welcome to [sponsor me on GitHub](https://github.com/sponsors/eleanorkonik). If you didn't have a pre-existing subscription, but would like one and don't trust my Ghost database (also fair!) just shoot me an email after sponsoring me on GitHub and I'll give you a complementary lifetime subscription too. We'll call it Early Bird Pricing 🕊️🙃 

## End of the Line

If you made it this far, thanks for listening to my tale of woe. Wish me luck! 

I'll try to send a (much shorter) email once I think everything is working as expected. 