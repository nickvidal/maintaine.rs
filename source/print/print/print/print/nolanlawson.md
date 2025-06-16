# @nolanlawson -- Nolan Lawson

> ![](https://i0.wp.com/github.com/nolanlawson.png?resize=200%2C200&ssl=1){ width=64px height=64px }  
> [github.com/nolanlawson](https://github.com/nolanlawson)  
> [maintaine.rs/nolanlawson](https://maintaine.rs/nolanlawson)

I first got involved in Open Source in the early 2010’s. Back then, it was a fun hobby project – a good excuse to flex my coding muscle, gain a little clout, and put my vision of software out there in the world.

Nowadays, Open Source is still the realm of tinkerers, dreamers, and hobbyists, but it has also exploded in popularity. Nearly every piece of software in the world relies on it. And yet, a lot of our practices around Open Source have not evolved to meet the challenges of this new reality: supply chain attacks, maintainer burnout, and never-ending dependency upgrades are all problems that we’ve only begun to grapple with.

In this article, I’d like to humbly offer some advice to my fellow maintainers to meet the moment of today’s Open Source landscape.

## My background

My first major Open Source project was [PouchDB](<https://en.wikipedia.org/wiki/Hoodie_(software)>), a JavaScript database. I got involved because I felt I could offer something useful to the project – bug fixes, performance improvements, new APIs. And plus, it was fun.

However, I quickly learned that spending every weeknight and weekend toiling away at open GitHub issues is a quick path to burnout. I wrote an article[^66] on the topic that struck a nerve with the Open Source community, and eventually coincided with my stepping away from the project in 2017\.

Since then, I’ve learned a lot about how to pace yourself with Open Source projects, how to avoid burning out, and when to call it quits. My key advice to new maintainers would be:

**You do not owe anyone anything.** There is a reason Open Source licenses have all-caps warnings like “THE SOFTWARE IS PROVIDED ‘AS IS,’ WITHOUT WARRANTY OF ANY KIND.” There can be a perverse effect in Open Source where the more work you do, the more is asked of you. Remember that just because you did work in the past does not give others a right to demand more from you, no matter how urgent they may sound in a GitHub issue.

**If it’s not fun anymore, you can step away.** Think about why you got into Open Source in the first place. Was it to scratch an itch? Explore a new language or framework? If the conditions that led you to Open Source in the first place have changed, then you should reflect on whether it makes sense to keep doing it, or whether you should move on to other projects.

**Leaving a project is not the end of the world.** As my friend Jan Lehnardt has said, “The tech comes and goes, but the people remain.”[^67] You can step away from a project without sacrificing the community or reputation you’ve built up in the interim. And in the end, your software still _works_ and delivers value for people, even without you actively working on it. And by leaving, you may even open up space for newer contributors to fill your shoes.

## Making Open Source work for the long haul

Despite my experience with burnout, I do still believe that Open Source is a force for good in the world, and that there is value in being a long-term maintainer of a project. But I’ve also learned some techniques that can help reduce the maintenance burden and keep burnout at bay.

I still maintain several small Open Source projects, but my years of experience have caused me to temper the naïve enthusiasm of my early days. Here is the advice I would give to maintainers who want their projects to thrive in the long run:

**Be careful adding new features.** In any successful Open Source project, the number of feature requests tends to grow (perhaps until it can read email[^68]). But due to the Pareto Principle[^69], _these are not the same requests_. You may find that you have 10 people asking for 10 different features, but each one is only useful to those 10 individual people. And if you add all those features to the project, you make your project more complex, harder to maintain, and harder for new users to understand. Sometimes it is worth saying “no” to a feature request, or suggesting that the user do what’s great about Open Source: just fork it\!

**Reduce dependencies.** This is not only helpful for long-term maintenance, but also supply-chain security[^70]. Every dependency is something that must be tended to and upgraded, especially as the laundry list of CVEs[^71] piles up. Do you really need to support Internet Explorer 9 and Node.js 6? Do you really need a utility library to pad a string[^72]? If not, unburden yourself and trim your project down to the bare essentials.

**Avoid breaking changes.** Many Open Source maintainers have taken Semantic Versioning[^73] as an invitation to make breaking changes whenever they feel like it. Don’t like the way you named an API? Just rename it\! However, think about the maintenance burden this places on consumers of your software (who may be other Open Source maintainers\!). Every breaking change is something you have to document (potentially forever), and it immediately obsoletes the informal documentation built up in Stack Overflow, blog posts, etc. Breaking changes should be as infrequent and minimal as possible.

## Conclusion

I love Open Source, and I’m grateful for the friends and experiences I’ve gained from it, as well as the talented pool of other Open Source maintainers who keep the whole system humming. I do believe, though, that we maintainers should take some responsibility for the software we’ve built, and to be cognizant of the way the rest of the world has grown to rely on it.

Of course, the burden does not fall on us alone. The “random person in Nebraska”[^74] is not to blame for the rest of the world relying on their work: as I said before, they don’t owe anyone anything. Companies that use Open Source should make an effort to give back – either through money or time – to the software that sustains them.

That said, we don’t live in a perfect world, and currently Open Source is in a strange moment where it’s often created by part-time hobbyists for the benefit of stupendously profitable corporations that give very little back. There is still value in doing it, and the relationship can be reciprocal, but maintainers often have to navigate this world alone, and to jealously guard their own mental health and the long-term health of their projects.

If you are just now getting into Open Source, I would say: wonderful\! It’s desperately needed, and you will likely learn and grow in a million ways throughout the process. Do try, though, to be respectful of your own well-being, and of the well-being of a world that has taken Open Source as a critical dependency. Very likely, the world will be counting on the next generation of maintainers to do it well and to do it sustainably.

\newpage


[^66]: https://nolanlawson.com/2017/03/05/what-it-feels-like-to-be-an-open-source-maintainer/
[^67]: https://narrativ.es/@janl/113339884688525095
[^68]: https://www.laws-of-software.com/laws/zawinski/
[^69]: https://en.wikipedia.org/wiki/Pareto_principle
[^70]: https://en.wikipedia.org/wiki/Supply_chain_security
[^71]: https://cve.mitre.org/
[^72]: https://en.wikipedia.org/wiki/Npm_left-pad_incident
[^73]: https://semver.org/
[^74]: https://xkcd.com/2347/
