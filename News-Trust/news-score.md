# CredScore: Fact vs. Fake #
NOTE: DRAFT

Fact-checks happen too slow to stop the viral spread of fake news. The fact-check will always arrive long after the hoax has infested social sites.

Quick containment control is what controls an epidemic outbreak. This is a proposal to instantly analyze the veracity of a news story.

Fact-checking will always take humans and hours, but machines can rapidly answer many critical fact-checking questions.

Is the website listed in Editor &amp; Publisher's DataBook? Is it in PolitiFact's Fake News Almanac? Does the story link to an author page? What is the Page Authority of the external links in article? 

We can grab dozens of <a href="https://github.com/hearvox/Research/blob/master/News-Trust/news-verification-checklists.md">fact vs. fake</a> indicators from existing APIs. None are conclusive on their own. But if combined and properly weighted, we could generate a 
reliable estimate of a story and website's credibillty.

People could submit a URL for which we'd return a CredScore, 0–100. Social sites could permit users to auto-submit a story before they share, or to submit all their links to get an average score for the stories they share. 

Those with high avergages might make their scores public, a source of pride. Maybe the social sites themselves would publish the average of all their users, a badge of the site's social resposibility.

more coming...

info button w/ detail on score.


  


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

