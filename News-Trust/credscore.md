# CredScore: Fact vs. Fake #
NOTE: DRAFT

Fact-checks can't stop fake news. The fact-checks arrives long after a viral hoax has already infested social sites.

To contain an epidemic outbreak you must act quickly. That's the goal of this project. Using just the URL, computers can instantly do enough <a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">fact-checking steps</a> to reliably estimate a news story's credibility. 

Simple checks like: Is the website in the <a href="http://www.editorandpublisher.com/databook/data/?djoPage=search_details&djoPid=25874">Editor &amp; Publisher DataBook</a<? Or is it in <a href="https://infogram.com/politifacts-fake-news-almanac-1gew2vjdxl912nj">PolitiFact's Fake News Almanac</a>, the <a hrwef="http://www.fakenewscodex.com/">Fake News Codex</a>, or any curated <a href="https://github.com/hearvox/Research/blob/master/News-Trust/fake-news-site-lists.md">fake new site list</a>? 
  
All the indicators will be pulled from existing API services. No one indictator will be conclusive. Dozens of weighted factors will go into a CredScore. Content checks for plagiarism and sentiment analysis. Tech checks for HTML and security standards. Network checks for link quality and page authority.  

## The Cred Badge of Courage ##
If a social site let users auto-submit a link before they post, they might not post at all if the link's CredScore was low. If uses could  submit all their shared links, they'd get their average CredScore, and perhpas, if high, could display their number publicly as a badge of cred honor.

## You can run, but you can't hide ##
Initial tests are already yeilding statically significant differences between fact vs. fake news sites, e.g., the year a site went online, the percentage of complex words in an article, and the number of its accessibility errors.

Some indicators would be costly (a11y) or even impossibilie (year online) for fake news sites to fight. CredScore would build upon itself: More URLs means more history of a site's past CredScores. This becomes another indicator, for that site's stories and for story links to and from other sites.

## Showing our hand ##
Best would be to make this project open source, maintianed by a community not a company. Transparency would be key: People need to trust us if their to trust our credibility estimates. CredScores would come with an info icon listing the factors in the score's calculations. Our methodology would be detailed, published, and open for review. 

## It ain't the meat, it's the motion ##
Bots can infect social sites with fake news but hoaxes go viral only with human help. CredScore attacks fake news via people, controlling its spread by dampening the network effect, until fact-checks and common sense take over.

I've been testing news and fake-news sites for dozens of indicators to findd those that best distinguish between the two. I'll post those results soon. I also have a 


## Story checks ##
* Page authority
* Quality of links in the article
* Warnings, e.g., ALL CAPS or "!!!" in headlines
* Author page and link to Google search
* Perspective
* URLscan.io
* Plagiarism
* Sentiment Analysis
* Date of article

## Site checks ##
* Check against OpenSources list of “Not Credible” sites
* Site ranking (World and USA)
* Date domain registered
* Domain authority
* Site security
* Google PageRank
* E&P database
* BuzzSumo
* URLscan.io
* Alexa
* Whois (DomainBigData)
* Subdomains (FindSubDomains)
* Analytics/Adsense IDs (SpyOnWeb)

## Author checks ##
* Twitter handle
* Email (LinkedIn)
* Facbook (IntelTechniques)
* ClaimReview (schema.org)


Fakes news is not a new problem. The centuries-old saying, "A lie can travel halfway around the world before the truth can get its boots on," <a href="https://quoteinvestigator.com/2014/07/13/truth/">has its roots</a> in the 1700s:
<blockquote>As the vilest Writer has his Readers, so the greatest Liar has his Believers; and it often happens, that if a Lie be believ’d only for an Hour, it has done its Work, and there is no farther occasion for it. Falsehood flies, and the Truth comes limping after it; so that when Men come to be undeceiv’d, it is too late; the Jest is over, and the Tale has had its Effect.<br>
<cite>Jonathan Swift, The Examiner newspaper (1710)</blockquote>
  
Maybe this is the century we finally have the tools to fight the fake news infestation.

