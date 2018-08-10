# CredScore: Fighting the Fake News Infestation #
* Fact-checks will always arrive too slowly to stop the viral spread of fake news.
* But many parts of the fact-check process can happen automatically.
* We can instantly produce a reliable estimate of a story's credibility using just its URL.

Many <a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">fact-checking steps</a> could be computer-assisted. The results, combined and weighted, could quickly generate a CredScore, 0–100, from fake to fact. 

Simple site checks like: Is the website in the <a href="http://www.editorandpublisher.com/databook/data/?djoPage=search_details&djoPid=25874">Editor &amp; Publisher DataBook</a> and the <a href="https://news.google.com/">Google News Index</a>? Or is it in a curated <a href="https://github.com/hearvox/Research/blob/master/News-Trust/fake-news-site-lists.md">fake news site list</a>, such as <a href="https://infogram.com/politifacts-fake-news-almanac-1gew2vjdxl912nj">PolitiFact's Fake News Almanac</a> or the <a href="http://www.fakenewscodex.com/">Fake News Codex</a>?

Story checks like: Is the article plagiarized or full of fake-news flags (e.g., CAPS or !!!)? Does the markup meet HTML and security standards?
  
No one indicator is conclusive. Scores of weighted factors go into a reliable CredScore.

## The Cred Badge of Courage ##
<img src="https://raw.githubusercontent.com/hearvox/Research/master/News-Trust/assets/FB-fake-news-post.png" width="450" alt="Mockup of Facebook post of fake news link with low CredScore" align="right" />Use cases:<br>
1. An online form: People submit an URL then get a score, and the ability to submit issues and comments on the results. (Perhaps a tool like <a href="http://filterbubbler.org/">FilterBubbler</a> can help crowdsource the best weightings.)

2. A WordPress plugin: All the links in a draft post automatically get CredScored as the URLs are entered.

3. A browser extension: People right click on a link in an article to get the linked resource's score.

4. An API service: If social site let people auto-submit a link before they post, some might not post links with low CredScores. If people submitted all their shared links, they'd get their average shared-link CredScore. People might want to display their number publicly as a badge of cred honor. High-scoring sites might also publish their badges.

### You can run, but you can't hide ###
Preliminary tests run on known fake-news and fact-based stories already reveal statistically significant differences. Real news domain registrations are an average of three years older. Fake stories show a lower average grade level (and percentage of complex words) in readability analyses and more errors in accessibility tests.

With each submitted URL, CredScore builds a better history of a site's trustworthiness. Soon CredScore history becomes another indicator. 

CredScore can continually auto-update and grow, chasing down all a fake-news site's connections: domains registered to the same owner, or using the same Google Ad or Analytics IDs, also redirects — these sites go dark often, as the scams are detected, then pop up in a new domain. 

When sites try to game the algorithm, they'll find many indicators time-consuming (a11y) and costly (year online) to fight. Consuming time and money is an anathema to the business model of fake news. 

### Showing our hand ###
This should be an open-source project, maintained by a community not a company. Transparency is key: People need to trust CredScore to trust its credibility estimates. Each CredScore would have a clickable info icon to list the main factors in the score's calculations. The methodology must be detailed, published, and open for review and revision. 

### It ain't the meat, it's the motion ###
Bots can infect social sites with fake news but hoaxes go viral only with human help. CredScore attacks fake news via people, controlling its spread by dampening the network effect, until fact-checks and common sense take over. To contain an epidemic outbreak you act quickly. That's the goal of this project. We hope to:
* Break up the fake-news business model by interfering with its ability of make a quick ad-buck on clickbait.
* Disrupt the viral spread by treating fake news like a virus, inoculating for it early, often and everywhere.

Will CredScore be a substitute for massive media fact-checking, widespread digital literacy, or people finally engaging their God-given built-in bullshit detectors? No. Never. But it can help get us there.

<div align="center"><img src="https://raw.githubusercontent.com/hearvox/Research/master/News-Trust/assets/cbs-fake-news-screenshots.gif" alt="Screenshots of fake news articles" /></div>

Below are a few of the machine-readable indicators (and existing API services) that will enable us to distinguish fact from fake news.

### Site checks ###
* Analytics/AdSense IDs (<a href="http://spyonweb.com/">SpyOnWeb</a>)
* Date domain registered (<a href="https://domainbigdata.com/">DomainBigData</a>)
* Domain authority (<a href="https://moz.com/researchtools/ose/">Moz Open Site Explorer</a>)
* Lists: Legitimate publisher (<a href="http://www.lionpublishers.com/members/list/">LION</a>, <a href="https://journalists.org/">ONA</a>, etc.)
* Lists: Fake-news site (<a href="http://www.opensources.co/">OpenSources.co</a>, <a href="https://isitfakenews.com/">Is It Fake News?</a>, etc.)
* Ranking (<a href="https://www.alexa.com/siteinfo/">Alexa</a>)
* Security (<a href="https://sitecheck.sucuri.net/">Sucuri</a>)
* Social shares (<a href="https://app.buzzsumo.com/research/most-shared">BuzzSumo</a>)
* Subdomains (<a href="https://findsubdomains.com/">FindSubDomains</a>)
* Technologies (<a href="https://builtwith.com">BuiltWith</a)
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
<li><a href="https://fact.pubmedia.us/">Fact-check Feed</a></li>
</ul>
