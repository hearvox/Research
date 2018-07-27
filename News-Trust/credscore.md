# CredScore: Fact vs. Fake #
Fact-checks can't stop fake news. The fact-checks arrives long after a viral hoax has already infested social sites.

To contain an epidemic outbreak you must act quickly. That's the goal of this project. Using just the URL, computers can instantly do enough <a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">fact-checking steps</a> to reliably estimate a news story's credibility. 

Simple checks like: Is the website in the <a href="http://www.editorandpublisher.com/databook/data/?djoPage=search_details&djoPid=25874">Editor &amp; Publisher DataBook</a<? Or is it in <a href="https://infogram.com/politifacts-fake-news-almanac-1gew2vjdxl912nj">PolitiFact's Fake News Almanac</a>, the <a hrwef="http://www.fakenewscodex.com/">Fake News Codex</a>, or any curated <a href="https://github.com/hearvox/Research/blob/master/News-Trust/fake-news-site-lists.md">fake new site list</a>? 
  
All the indicators will be pulled from existing API services. No one indictator will be conclusive. Dozens of weighted factors will go into a CredScore. Content checks for plagiarism and sentiment analysis. Tech checks for HTML and security standards. Network checks for link quality and page authority.  

## The Cred Badge of Courage ##
If a social site let users auto-submit a link before they post, they might not post at all if the link's CredScore was low. If uses could  submit all their shared links, they'd get their average CredScore, and perhpas, if high, could display their number publicly as a badge of cred honor.

### You can run, but you can't hide ###
Initial tests are already yeilding statically significant differences between fact vs. fake news sites, e.g., the year a site went online, the percentage of complex words in an article, and the number of its accessibility errors.

Some indicators would be expensive (a11y) or even impossibilie (year online) for fake news sites to fight. CredScore would build upon itself: More URLs means more history of a site's past CredScores. This becomes another indicator, for that site's stories and for story links to and from other sites.

And CredScore would continually auto-update and grow, chasing down all the connections of a fake-news sites, domains registered to the same owner, or with the same Google Ad or Analayyics IDs, or redirects — as these sites are constantly being taken down and replaced as the scams are detected. 

### Showing our hand ###
This should be an open-source project, maintained by a community not a company. Transparency would be key: People need to trust us if their to trust our credibility estimates. CredScores would come with an info icon listing the factors in the score's calculations. Our methodology would be detailed, published, and open for review. 

### It ain't the meat, it's the motion ###
Bots can infect social sites with fake news but hoaxes go viral only with human help. CredScore attacks fake news via people, controlling its spread by dampening the network effect, until fact-checks and common sense take over.

Below are a few of the machine-accessible indicators and API services that will enable us to distinguish between news and fake-news.

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
* Web stanadards (<a href="https://validator.w3.org/">W3C Markup Validation</a>)

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
<ul>
