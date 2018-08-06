# CredScore: Fighting the Fake News Infestation #
* Fact-checks will always arrive too slowly to stop the viral spread of fake news.
* But many parts of the fact-check process can happen automatically.
* We can instantly produce a reliable estimate of a story's credibility using just its URL.

Many <a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">fact-checking steps</a> could be computer-assisted. The results, combined and weighted, could quickly generate a CredScore, 0–100, from fake to fact. 

Simple site checks like: Is the website in the <a href="http://www.editorandpublisher.com/databook/data/?djoPage=search_details&djoPid=25874">Editor &amp; Publisher DataBook</a> and the <a href="https://news.google.com/">Google News Index</a>? Or is it in <a href="https://infogram.com/politifacts-fake-news-almanac-1gew2vjdxl912nj">PolitiFact's Fake News Almanac</a>, the <a href="http://www.fakenewscodex.com/">Fake News Codex</a>, or other curated <a href="https://github.com/hearvox/Research/blob/master/News-Trust/fake-news-site-lists.md">fake news site list</a>?

Story checks examine the article (and its links) for plagiarism and sentiment analysis (e.g., CAPS or !!!). Tech checks test HTML and security standards and page authority. All pulled from existing API services
  
No one indicator is conclusive. Scores of weighted factors go into a reliable CredScore.

## The Cred Badge of Courage ##
People submit an URL then get a score, and the ability to submit issues and comments on the results. (Perhaps a tool like <a href="http://filterbubbler.org/">FilterBubbler</a> can help crowdsource the best weightings.)

If a social site let people auto-submit a link before they post, some might stop posting links with low CredScores. If people submitted all their shared links, they'd get their average CredScore. People might want to display that number publicly as a badge of cred honor.

### You can run, but you can't hide ###
Initial tests already reveal potentially usable differences between fake and fact. Fake site domains are newer (an average of three years). Fake stories have a lower average grade level, fewer complex words, and more accessibility errors.  

When fake news tries to game the algorithm, they'll find many indicators expensive (a11y) and difficult (year online) to fight. Meanwhile, with each submitted URL, CredScore builds a better history of a site's trustworthiness. Soon CredScore history becomes another indicator. 

CredScore can continually auto-update and grow, chasing down all a fake-news site's connections: domains registered to the same owner, or using the same Google Ad or Analytics IDs, also redirects — these sites go dark often, as the scams are detected, then pop up in a new domain. 

### Showing our hand ###
This should be an open-source project, maintained by a community not a company. Transparency is key: People need to trust CredScore to trust its credibility estimates. Each CredScore would have a clickable info icon to list the main factors in the score's calculations. The methodology must be detailed, published, and open for review and revision. 

### It ain't the meat, it's the motion ###
Bots can infect social sites with fake news but hoaxes go viral only with human help. CredScore attacks fake news via people, controlling its spread by dampening the network effect, until fact-checks and common sense take over. To contain an epidemic outbreak you act quickly. That's the goal of this project.

Below are a few of the machine-accessible indicators (and API services) that will enable us to distinguish between news and fake-news.

### Site checks ###
* Analytics/AdSense IDs (<a href="http://spyonweb.com/">SpyOnWeb</a>)
* Date domain registered (<a href="https://domainbigdata.com/">DomainBigData</a>)
* Domain authority (<a href="https://moz.com/researchtools/ose/">Moz Open Site Explorer</a>)
* Lists: Legitimate publisher (<a href="http://www.lionpublishers.com/members/list/">LION</a>, <a href="https://journalists.org/">ONA</a>, etc.)
* Lists: Fake-news site (<a href="http://www.opensources.co/">OpenSources.co</a>, <a href="https://isitfakenews.com/">Is It Fake News?</a>, etc.)
* Ranking (<a href="https://www.alexa.com/siteinfo/">Alexa</a>)
* Page rank (<a href="https://pr.domaineye.com/pr/">Google PageRank</a>)
* Security (<a href="https://sitecheck.sucuri.net/">Sucuri</a>)
* Social shares (<a href="https://app.buzzsumo.com/research/most-shared">BuzzSumo</a>)
* Subdomains (<a href="https://findsubdomains.com/">FindSubDomains</a>)
* Technologies (a href="https://builtwith.com">BuiltWith</a)
* Whois (<a href="http://whois.domaintools.com/propornot.com">DomainTools</a>)

### Story checks ###
* Accessibility (<a href="https://wave.webaim.org/">WAVE Accessibility Evaluation</a>)
* Content quality (<a href="https://www.webpagefx.com/tools/read-able/">WebpageFX</a>)
* Links quality/Page authority (<a href="https://analytics.moz.com/">Moz Link Explorer</a>)
* News article and author meta (<a href="https://schema.org/NewsArticle">Schema.org</a>)
* Plagiarism (<a href="https://www.copyscape.com/">Copyscape</a>)
* Security (<a href="https://securityheaders.com/">Security Headers</a>)
* Sentiment and syntax (<a href="http://saifmohammad.com/WebPages/NRC-Canada-Sentiment.htm">Sentiment Analysis System for Tweets</a>)
* Web standards (<a href="https://validator.w3.org/">W3C Markup Validation</a>)

### Author checks ###
* Facebook user data (<a href="https://inteltechniques.com/menu.html">IntelTechniques</a>)
* Twitter bots (<a href="https://botometer.iuni.iu.edu/">Botometer</a>)

## Swatting falsehood flies ##
Fakes news is not a new problem. The centuries-old saying, "A lie can travel halfway around the world before the truth can get its boots on," <a href="https://quoteinvestigator.com/2014/07/13/truth/">has its roots</a> in the 1700s:
<blockquote>As the vilest Writer has his Readers, so the greatest Liar has his Believers; and it often happens, that if a Lie be believ’d only for an Hour, it has done its Work, and there is no farther occasion for it. Falsehood flies, and the Truth comes limping after it; so that when Men come to be undeceiv’d, it is too late; the Jest is over, and the Tale has had its Effect.<br>
<cite>Jonathan Swift, The Examiner newspaper (1710)</blockquote>
  
Maybe this is the century we finally have the tools to fight the fake news infestation.

### CredScore Resources ###
<ul>
<li><a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">News verification checklists</a></li>
<li><a href="https://github.com/hearvox/Research/blob/master/News-Trust/fake-news-site-lists.md">Fake News site lists</a></li>
<li><a href="https://hearingvoices.com/tools/credscore/">CredScore API tests</a></li>
</ul>
