# The Dymaxion License

This page details the dymaxion license project and raison d'être. For the license content, see the [license file](LICENSE) or check the releases.

## What

Licensing is far too complicated.

The Dymaxion License is a highly permissive [copyfree](http://copyfree.org/) license intended to expressly license software and content in a single combined license agreement that protects the rights of contributors whilst respecting the rights of any incorporated components, dependencies, or upstream projects.

It's the "set it and forget it" of technical licensing.

## Problem

Dual OSS+Proprietary vs AGPLv3? BSD-3 vs Apache 2? Licenses that protect my freedom by giving me more restrictions? Great.

I am not a lawyer. I'm an engineer, programmer, hacker, tinkerer, maker, writer, designer, or architect.

When I contribute, I don't care what you do with the results... I just don't want to be sued. It should be understood that when the copyleft movement was started, the technology landscape was rather hostile, and it served a grand purpose much larger than itself. But times have changed. Not only do we have software licensing issues to deal with, but we also have associated media and content licensing issues to manage, both of which are largely incorporated into the web technologies that are ubiquitous today.

I have spent way too much of my life on [tl;dr legal](https://tldrlegal.com/), and have seen way to many online discussions and questions surrounding licensing. It's painful, boring, and annoying. That energy should be spent on productive pursuits rather than on legal matters.

\* I am not affiliated with tl;dr legal, but I do think they are cool. And they have an [auditing tool](https://fossa.com/) which seems epic for those interested in such things.

Originally called the "Copy Free Multilicense", I long ago had the idea to combine a traditional "multi-license" agreement used by some for-profit software projects, into a single "multilicense" that could be used for my own projects, explicitly publishing my content and code into the public domain whilst remaining compliant with any of the license requirements for any dependencies I might be using or leveraging.

Eventually, inspired by the license I found on [baserow](https://gitlab.com/bramw/baserow/-/blob/d3c47df5ebc2ae9d45099e32d303ef9d490ac777/LICENSE) (it's not just me who reads these right?), I decided to actually go ahead and write it so that I could at least start using it myself.

I am spiritually a supporter of the wtfpl and the [unlicense](https://unlicense.org/), and indeed I used to try and show my solidarity by using the unlicense for my own personal projects which I did not expect to be heavily utilised by third parties. I am, of course, aware that there are numerous [issues](https://github.com/github/choosealicense.com/issues/805) surrounding the use of such licenses, which honestly makes me feel like I'm stuck back in 2007.

Most people default to using the MIT license or similar licenses (although i feel most people also largely ignore license agreements altogether), but the reality is that so many licenses require some form of attribution, which ends up actually becoming a pain point for anyone who treats license agreements the proper respect. It also means that if you make a project from a simple HTML template, you are, in effect, still required (depending on where the law is applied) to include the original authors in the license, [even if every line of their original code is replaced with your own](https://opensource.stackexchange.com/questions/4345/theseus-paradox-applied-to-code-copyright). There are still compliance issues though, but we'll get to that shortly.

In theory you would also have to copy in a whole lot of license information from a copy-pasta snippet. Even stack overflow answers should effectively carry some license. Mostly, the internet just follows the rule that "if it's publicly available it's mine". But that's not always ideal. We don't know what audit tools, technologies, or other ramifications our current licenses will have on future technologies. The [GitHub Coilot licensing debate](https://fossa.com/blog/analyzing-legal-implications-github-copilot/) is proof enough of that.

My view is just license everything as freely as possible and rely on good behaviour from the community to enforce attribution or whatever it is you want from them. Chances are, by the time your project warrants it, you'll be [issuing your own custom licensing agreements](https://www.cockroachlabs.com/blog/oss-relicensing-cockroachdb/) anyway.

## Solution

So what license then? How can the world spend less time haggling and more time building? We realistically need a license that fixes this.

Enter 0BSD (Or MIT-0. They're pretty much the same thing.).

The 0BSD is pretty much a public domain software license that expressly limits publisher liability whilst being as permissive as possible. To the point where the license doesn't expressly have to be distributed with the outputs. Bingo.

Unfortunately, the 0BSD is not as widely used or supported as one might expect. Personally I think that this is an institutional failure. For some reason, even new GitHub projects can't be added from the list of templates (yet).

Even with existing public domain-equivalent licenses though, there's a catch.

Software licenses like the BSD do not explicitly cover content (although it's public domain equivalent, it still talks about software. Whether or not that would apply to content I feel could be debated or interpreted differently based on where it is applied). So the definition of "the software" _could_ include the writing in a web page template, or the documentation of a software package, or it could not. But what about code snippets and examples in the docs? What about content in the templates? Is my lorem ipsum covered by my license? Then my head hurts.

Honestly, I doubt there's any legal precedent for it anywhere in the world, so it's likely nobody cares. Unfortunately, we don't know what things will look like in 10 or 20 years, and having trivial limitations pop up on large community projects is painful for everyone.

Basically, my approach is to take the traditional "dual license" agreement - where something is licensed according to different use cases, and invert it by applying multiple licenses to the same set of assets to give blanket permission and protection. Of course there may still be license compatibility issues, but with permissive or public-domain equivalent licenses I'd bet it's largely a non-issue.

So the dymaxion license basically just states that _your_ code is 0BSD, _your_ content is CC0, and any third party components are licensed under the license with which they were distributed to you (which you'll need to provide alongside such elements).

## Dymaxion?

Yep. DY (dynamic), MAX (maximum), and ION (tension).

R. Buckminster Fuller](https://en.wikipedia.org/wiki/Buckminster_Fuller) was a bit of an oddball character, but he had some interesting ideas - from houses to cars to map projections. Amongst his many inventions, a number of them were called "dymaxion", which was a term ol' Bucky coined himself.

This collection of devices weren't terribly pragmatic, or even very functional, but they all had a few things in common - including the goal of "maximum gain of advantage from minimal energy input".

So why would I name a license after it? Well, I already stated above that IANAL, so the "legal" quality of the license document provided by this project is probably not yet enterprise ready at all. In fact, the de jure validity of the entire thing could be [bupkis](https://web.archive.org/web/20210301034640/https://www.bupkis.org/index.php/what-is-bupkis), so YMMV and you should use it at your own risk. This license is a seed, I'm just hoping that it blossoms into something much greater.

As stated in a NYT [Article](https://web.archive.org/web/20201112012751/https://www.nytimes.com/2008/06/15/automobiles/collectibles/15BUCKY.html) on the dymaxion car: "Fuller, who always saw the Dymaxion, as he saw much of the world, as a kind of provisional prototype, a mere sketch, of the glorious, eventual future."

## What now?

![standards](https://imgs.xkcd.com/comics/standards.png)

I think that like many new technologies, new licenses are written by folk who want to produce stuff with their name on it. Many people would rather be the king of their own hill than climb the mountain with everyone else. Each unto their own. But this is not that.

This is an idea that we could bundle a bunch of licenses into one big mass so that it is clear that whatever the original contributors produce is published into the public domain, regardless of the jurisdiction. Ideally it should be multilanguage too, but that's a bit beyond my scope.

The point of this repo is really to let someone else better than me take the idea and build something much more robust with it. I want to find the "One license to rule them all".

So long as in the future I can build what I want without thinking about licensing anymore. Just write a license that does what this does, but better. Or extend this one. Either that or find someone gracious enough to point me towards a resource that does it already.

> “a pessimist is either always right, or pleasantly surprised” - internet quote

## Limitations

This still doesn't cover everything, everywhere. It certainly doesn't cover explicit data licenses like the [ODbL](https://wiki.osmfoundation.org/wiki/Licence) or other elements where attribution is required. Each component just has to be evaluated on a case by case basis and treated accordingly until someone more clever than me finds a way around it.

There is also the whole issue of ("compatibility")[https://www.gnu.org/licenses/license-compatibility.html], which is a needlessly complicated way of trying to force copyleft onto downstream projects. At this point, I expect the wording is going to cover the majority of permissive or intermediate licenses, but I don't think "incompatibly licensed" components are going to be covered until I can afford a legal team.

The simple solution is to just ignore copyleft projects as dependencies and components. Substitute everything that's "free" for something "libre" and maybe by 2050 we'll have a society that's more concerned with progress than with quarrelling. If there isn't any reasonable substitution for copyleft components, then it's probably a whale of a project and better to just abstract everything to a set of API integrations anyway.

Maybe a license compatibility matrix could be built, but for now I'd say use copyleft components at your own peril.

Of course, if you are wanting to release your own project as copyleft, then this license isn't for you. The other thing is that releasing your code under copyleft pretty much saves you from having to deal with the issues of using copyleft components, but that's part of the problem this license tries to solve.

The other issue is patent exclusions (what the apache and mozilla licenses are big for) - so if you're worried someone hijacks your code base, develops a new feature on top of it, patents that as an invention and and they will limit you from developing that feature for yourself.

My personal view is that in todays world of cancel culture and social media fire, the likelihood of that hypothetical is pretty darn low and it carries a lot of risk for perpetrators, so in most cases you needn't worry. Maintenance of large projects is a huge issue so in most cases it's against everyone's best interest to do that until you get to the scale you need to write your own custom license agreement anyway.

## Process

Use this license for your project, but be sure that any dependencies and third party content have the proper attribution and license information provided alongside them.

For the most part, this simply means including the additional materials that were delivered with the components when they were attained or distributed. In most instances for software, just placing each dependency in it's own directory with a license file associated should do.

Remember to cite and reference third party content appropriately. For example, making a map or derivative dataset with OpenStreetMap data requires attribution to that project (I know - painful right?). One day the robot overlords will automate this for us or eradicate us for caving so sadly to our egos, but for now I can't see a way around it.

## Attribution

Using a license file for attribution is (IMO) just a generally terrible idea and attribution-required licenses are routinely ignored, pretty much never enforced, and needlessly complicate things for the downstream projects that matter (most of which would respect a simple "please attribute me" request). By requiring your attribution (which typically requires resources to figure _how_ exactly attribution), projects and content can be reasonably expected to be excluded from meaningful downstream projects and innovations.

Not that there's anything wrong with people wanting credit with their work (although in my experience with this, those concerned with attribution typically produce inferior work anyway), but I just don't think licenses are the way to do it. in much the same way that projects like [allcontributors](https://allcontributors.org) point out that contributions aren't just code, community software doesn't "belong" to the original publisher anyway, so "xyz and contributors" is a pretty meaningless statement.

It's just good behaviour to publish attributions appropriately. We should be voting with our wallets (i.e. not using projects with a history of poor attribution or stealing credit) and have a de facto process for creating a proper `ATTRIBUTIONS` file in all repos (if a community standard exists, please make an issue to let me know) so that we can all cite prior art in an easy to use, clear, and effective way (outside of dependency trees which manage much of that for us). Hopefully when AI takes our jerbs they'll sort this mess out automatically too.

If you really want attribution for your work, use twitter rather than your license file.

## Contribute

As stated, this is expected to be imperfect and evolve so feel free to submit a PR or opine in the issues section.
