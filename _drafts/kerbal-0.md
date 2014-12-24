---
layout:     post
title:      "Kerbal Space Program: Pre-Flight Checklist"
subtitle:   "An Introduction to Modding KSP"
#date:       2014-12-18 10:00:00 EST
author:     "Wisq"
header-img: "img/home-bg.jpg"
---

From where I'm standing, things are looking pretty good for space exploration.  Major missions are reaching completion, new ones are being launched, NASA got *more* funding than they asked for, and public interest is at a level I don't remember since my childhood back in the 1980s.

I'd like to think that *Kerbal Space Program* (or "KSP" for short) had some small role in that last bit.

Set in a miniature solar system with the proverbial "little green men" as your titular space-faring protagonists, it challenges you to establish a full-fledged space program, starting from nothing more than a single-occupant pod strapped to a rocket engine and going "up" from there.  Along the way, you get to learn about rockets, about orbits and burns, about the kinds of challenges facing a space program and spaceflight, and about the beauty and vastness of outer space itself.

KSP just released version 0.90, their first "scope complete" beta version.  They'll still be adding features, but they've established the basic gameplay framework needed for the final game.  Regardless, it's been eminently playable for years, and gained quite a bit of popularity over the past year since they added a proper progression system.

In my opinion, KSP is well worth the regular asking price, but right now you can [grab it for 25% off at Steam][KSP-steam] until the new year.

In this series of posts, I'll introduce some of the community-made game mods I currently use and recommend.  After that, I hope to post a longer series documenting a modded playthrough.

## Modding

Like *Minecraft*, KSP is a full-fledged game, and newcomers would be well advised to play it "vanilla" or "stock" (unmodded) until they've got the hang of it.  But also like *Minecraft*, the vibrant modding community is where it really starts to shine.  For those wanting more content, or maybe more realism and challenge, there are countless mods available out there to improve and customise your KSP experience.

To manage your mods, I highly recommend you grab [CKAN][ckan], a mod manager that automatically downloads and installs mods (and their dependencies) for you.  It also tracks the versions you have installed and offers to upgrade them when new versions are released.  It's the new hot thing in Kerbal modding, and it's well worth using — unzipping and installing mods gets to be a major pain once you have a dozen or more.

Using the CKAN graphical interface is pretty easy.  First, click "Refresh" to update the list of mods.  Check off the mods you want, then click "Changes" to see what needs doing.  Apply those changes, then launch KSP, either via CKAN or via your normal method.

In the mod descriptions below, I'll be giving out links to the mods so you can get more information — but if that mod is available in CKAN, you should probably install it there instead.  It's just less fuss that way.

## Realism Mods

For most games, I'm of the opinion that adding realism is generally a good thing so long as it doesn't actively harm gameplay.  Reality is complex and interesting, and adding realism usually creates some equally interesting interactions that the game designers didn't forsee, rewarding player creativity.  It also creates tricky challenges, often via injecting a bit of chaos.  And at the very least, it lets players better reason about how things will work.

In KSP, there's another reason to add realism: *Education!*  A lot of us enjoy playing KSP because we get to learn how space works, and using realism-enhancing mods (or even just researching what they do) can take that to the next level.

However, be warned that a lot of realism mods are also going to add difficulty, because in its stock form, Kerbal makes spaceflight a lot easier than it really is.  Don't start delving into these until you're pretty comfortable with flight and orbital mechanics, unless you really want a challenge.

### FAR

The stock Kerbal aerodynamic model is exceedingly primitive — parts all contribute a certain amount of atmospheric drag, regardless of position or orientation.  A tall, slender rocket is no more aerodynamic than a flat "pancake" ship, and using nosecones to make your ship sleeker actually *adds* to drag!

[Ferram Aerospace][FAR], or "FAR", fixes all this.  It's a complete remodelling of planetary atmospheres and flying within them.  Your ship's shape actually matters, and non-aerodynamic bits will cause trouble very quickly, e.g. by breaking off.  And an ill-designed ship or plane can be completely impossible to control, flipping until it breaks up.

To counter this, FAR also offers diagnostic tools that help you understand what's going on with your plane, both during construction and in flight.  Pre-flight simulations give you an idea whether your plane is stable or not, and in-flight readouts let you fine-tune your flight parameters.  For example, you'll want to learn what ["max Q"][maxQ] is, and you'll feel relieved every time you pass it uneventfully (as in a real launch).

### Procedural Fairings + Universal Storage

So if your rockets now need to be aerodynamic, how can you include non-aerodynamic equipment or assemblies on your rockets, such as science equipment or satellites?  Well, these two mods have you covered.

[Procedural Fairings][fairings] lets you put "shells" around components on your ship.  For example, you might place a *fairing base ring* near the top of your rocket and then build a non-aerodynamic probe on top.  Or, you might have a thinner section in the middle of your ship with science gear attached, and place base rings on either side (facing each other) to encase it.

In either case, you then attach the fairing shells (either conical or egg-shaped) and adjust their position in the staging sequence.  Once in space, stage them like any other component, and the shells will break apart via explosive bolts and be discarded, revealing the sensitive equipment inside.  It's quite dramatic, and fun to watch.

[Universal Storage][universal] gives you a less ambitious but more structural solution.  You first place down a "core" (comes in quad-, hex-, and octocore variants), then place wedge-shaped multi-purpose modules around it.  The empty *Science Bay* module lets you mount science equipment on walls inside the ship, while other modules offer various forms of integrated tanks and equipment.

In addition to these core modules, Universal Storage also offers a number of add-on packs that integrate with other mods.  These packs may add resource tanks or converters, or offer wedge versions of the mod's new equipment.  I'll mention these in those other mods' descriptions where applicable.

### KIDS

FAR does have one downside: It actually becomes *easier* to get into space.  Once you get over the hurdle of making rockets that don't break up on launch, you may notice that you need about a quarter less delta-v (effort) to make it into orbit as you do in stock KSP, meaning you can carry unrealistically large payloads into space.

The reason?  Because stock Kerbal engines are actually too powerful!  The KSP developers made the stock Kerbal atmosphere more like soup than air, and so they had to bump all the engine powers up to balance things out — but that breaks balance when the atmosphere is modeled realistically again.

To solve this, the [Kerbal Isp Difficulty Scaler][KIDS] mod ("KIDS", by the same author as FAR) offers a way to blanket-reduce all engine efficiency by an equivalent amount, returning balance to the universe and restoring the original difficulty.

(For the extra-realism-inclined, KIDS also offers the ability to make specific impulse affect thrust rather than fuel consumption — i.e. your engines *produce less thrust* within the atmosphere, rather than just *consuming more fuel*.)

### Deadly Reentry

Once you've faced FAR's aerodynamic challenges, and completed your mission despite a KIDS reducing your delta-v to realistic levels, it's time to face the final challenge of your mission: the [Deadly Reentry][reentry].

In stock KSP, it's almost impossible to actually burn up due to a botched reentry — as in, you pretty much have to be coming in straight down at an insane velocity (probably via cheating).  In reality, reentry angles are a real concern, and reentry itself is a fairly risky part of the mission.

Deadly Reentry brings this back.  Aside from adding the titular deadly consequences to steep reentry angles, it also adds ablative heat shields to crew pods and requires that you angle them so the shield is facing forwards.  You can even choose what thickness of heat shield to use for the larger Mark 3 crew pod, letting you trade mass for safety.

This tends to be the sort of realism feature that you get used to and then forget about … somewhat.  Once you're in the habit of coming in at a particular angle (periapsis altitude), this mod won't bother you much.  But on that one occasion where you screw it up, this will give you an epic and/or tragic story to tell.

### RemoteTech

Getting away from aerodynamics entirely, we have the [RemoteTech][remotetech] mod.  This mod completely revamps how communications and unmanned probes operate.  The idea is that probes require actual command signals, and are not just AIs capable of solving their own problems like a real crew is.

With this mod installed, you need a working communications link back to the Kerbal Space Centre if you want to control a probe or send science data back home (including from manned ships).  Antennae are now activated and deactivated manually, and cost power to operate while active.  Line-of-sight is required, meaning you'll need relay satellites to bounce signals around obstructions (e.g. planets).  And light-speed delay is in effect, meaning all that bouncing will lag your controls accordingly.

Controlling a satellite by hand would be nigh-impossible with several minutes of light-speed delay, so it also gives you a rudimentary flight computer.  Using this, you can send commands like "turn to prograde" or "burn at 25% throttle for 5 seconds", or create manoeuvre nodes and direct the flight computer to execute them at the appropriate time.  These commands continue to execute so long as the probe has power, even if you lose your communications signal.

RemoteTech lets you experience the suspense of waiting to see if your planned burn worked, and knowing it's too late to change anything if it doesn't.  It creates chaos and excitement when you don't plan far enough ahead and you lose signal at a critical moment.  And finally, it makes manned flights worthwhile again for those critical missions, even if there's no EVAing or flag-planting to be done.

### TAC Life Support

Finally, if RemoteTech makes unmanned probes risky and exciting, then [TAC Life Support][TAC] does the same for manned ships.  It introduces several resources that are required to keep your crew alive, with deadly consequences if they run out.

In the stock game, Kerbals are basically the perfect space creatures — they can float around in just a spacesuit for *years* without air, heat, food, water, etc.  This is great for going easy on beginners, but also eliminates any sense of risk, tension, or time limit for manned missions.  You'll never have the *Apollo 13*-esque excitement of a mission gone horribly wrong, for example.

TAC brings all this real-life excitement back.  It's fairly generous with resources — one big canister will hold enough to last a single Kerbal for 300+ days — but it still puts a time limit on your near-Kerbin missions, and adds a fair chunk of mass to your interplanetary missions.

It also makes unmanned probes a much more desirable option in many cases.  Without TAC, there's not a lot of value to an unmanned probe — you save a bit of mass but lose the option to do reports and EVAs.  But when a crewed ship means adding life support mass *and* taking on extra risk, the situation is quite different.

Plus, it brings excitement, and makes time actually *mean something* again.  Accidentally hit the stage button too soon and dumped most of your resources?  Hope you can prepare a rescue mission in time!  Missed that transfer window to get back home?  You can't just wait until the next one in a few years — better go for the risky option!  Etc.

Note that TAC interacts well with Universal Storage.  A [US TAC Pack][US-TAC] is available with tank wedges to carry the TAC resources and processors to recycle some of them, while the US Core parts let you either split (or produce) water into (or using) hydrogen and oxygen, all via methods used in real-life space flight.

## Other Mods

This is just the tip of the iceberg.  I currently run over 50 mods, and while I probably won't have a chance to introduce all of them, there are plenty more that are worth a mention.  I'll cover these in future posts, so stay tuned!

[KSP-steam]: http://store.steampowered.com/app/220200/ "Kerbal Space Program on Steam"
[ckan]: http://forum.kerbalspaceprogram.com/threads/100067 "The Comprehensive Kerbal Archive Network (CKAN) Package Manager — KSP Forum"
[FAR]: http://forum.kerbalspaceprogram.com/threads/20451 "Ferram Aerospace Research — KSP Forum"
[maxQ]: http://en.wikipedia.org/wiki/Max_Q "Max Q — Wikipedia"
[KIDS]: http://forum.kerbalspaceprogram.com/threads/52882 "Kerbal Isp Difficulty Scaler — KSP Forum"
[fairings]: http://forum.kerbalspaceprogram.com/threads/39512 "Procedural Fairings — KSP Forum"
[universal]: http://www.kingtiger.co.uk/kingtiger/wordpress/universal-storage-a-mod-for-kerbal-space-program/ "Universal Storage: A mod for Kerbal Space Program"
[reentry]: http://forum.kerbalspaceprogram.com/threads/54954 "Deadly Reentry — KSP Forum"
[remotetech]: http://forum.kerbalspaceprogram.com/threads/83305 "RemoteTech — KSP Forum"
[TAC]: http://forum.kerbalspaceprogram.com/threads/40667 "TAC Life Support — KSP Forum"
[US-TAC]: https://kerbalstuff.com/mod/364 "Universal Storage [TAC PACK] — KerbalStuff"