# The Economic Impact of Cyber Warfare

#### (c) 2018 Karsten Johansson

* NOTE: This is a rough draught of an introductory article that will be published on the www.PENETRATIONTEST.com website. It is provided in this form for review purposes only. It is part of approximately 40 articles currently being edited for inclusion on the www.PENETRATIONTEST.com website over the next few weeks. It is a very large project that the author has spent countless hours on, so please don't ruin it by disrespecting the copyright.

It isn’t too difficult to see how leaked emails can be detrimental to the victim's reputation, but many companies have been chided for stating damages in the hundreds of thousands of dollars. How could such numbers be realistic? 

For instance, a few years back many skeptical people were asking how a simple denial of service attack could cost any significant amount of money, since the majority of Anonymous’ Low Orbit Ion Cannon attacks were not targeted against online sales businesses anyway. 

What they didn’t see is the “business end” of information security. There are many costs associated to information security, even when a company isn’t actively being targeted. This article attempts to explain where and how much of that money is spent.

## Understanding the Financial Impact

In business, everything is eventually classified by its ability to create money, or its penchance for losing it.

A sustained attack against an online business is said to cost anywhere from US\$500,000 to millions of dollars per day. This is just the revenue impact, which depends highly on the popularity of the site. For example, a 2011 attack on Sony is reported to have cost them in excess of US\$170 million. In 2012, News Corp. announced that hacking had cost them a similar amount. And we are increasingly hearing of massive losses like these today.

But how is it then, that some companies are on record saying that well publicized attacks against their systems only had a negligible impact while others claim crippling loss for what pretty much amounts to identical attacks? As we will investigate, either there is some hope that discrediting attacks - and by extension, the attackers themselves - will put an end to them, or the companies are genuinely naive and unaware of their actualized security expenditures. This is an area where we, as information security professionals, need to set the record straight, and educate right up to the corporate executive level.

> This is an area where we, as information security professionals, need to set the record straight.

In 2002, NIST published a study that is still as valid today as it was back then. In their study, they quantified the cost of fixing bugs (security or otherwise) throughout the typical project life cycle. NIST divided the prototypical project into the following stages:

1.	Design Stage
2.	Coding Stage
3.	Integration Stage
4.	Beta Stage
5.	Production Stage

NIST then divided the common bugs into the following categories:

1.	Design Errors
2.	Coding Errors
3.	Integration Errors

And here is how they presented those costs:

|  | Design Stage | Coding Stage | Integration Stage | Beta Stage | Production Stage |
|:-----:|:------:|:------:|:------:|:------:|:------:|
|**Design Errors**| 1x | 5x | 10x | 15x | 30x |
|**Coding Errors**| n/a | 1x | 10x | 20x | 30x |
|**Integration Errors** | n/a | n/a | 1x | 10x | 20x |

All security issues are a result of design, coding, or integration errors. However, for many web-based companies, the first dabble with security tends to be delayed to right before the production stage, if at all. Let’s follow this through with a couple examples to see how this impacts the company financially. 

We'll begin by underscoring the premise that many security issues begin at the design stage – yet so often, security is somehow tacked on at the end once the need becomes more readily and immediately apparent. In reality, it is at this early stage where security requirements should have already been defined and applied; well before the project is ready for coding.

If the designer merely stated that the application requires login and password use, and these credentials would be kept in a database, then all too often, this is exactly what the developer is going to code. Nothing more was asked, and nothing more is delivered. There was no security specification in the design, so there is unlikely to be any meaninful security control built into the code. 

So, how does producing weak code end up costing 5 times more than if the requirements for secure coding were already in the design stage? 

> ... so often, security is something that gets tacked on at the end as the need becomes apparent.

The coder is bound to programming precisely what it is they are hired to program. If a coder notices that there were no design decisions for protecting passwords, it is up to the designer then to specify how this needs to be handled. 

This means the coder, provided their security knowledge is sufficient to notice such flaws, reports the issue to the designer, who then rewrites the affected parts of their design specification, leaving at least part of the coding project on hold. You now have one person duplicating their prior work, and another person waiting on them so they can get back to coding. 

And it isn’t only the coder waiting – the entire project is on hold to varying degrees. But this isn’t as bad as it gets yet. So far it’s only costing 5 times the amount it would have if the mitigating requirement were built into the design in the first place.

Now let’s go even one step further and say that due to the lack of security considerations during the design stage, the coder is equally unskilled in terms of secure programming. Now the design flaw has been codified and released to the integrators. If a security flaw is discovered during the integration stage, it is typically due to hours or days of attempting to diagnose why the software is misbehaving in some way as the different components try to communicate. Eventually the coder may figure out what needs to be done, but again he or she will be forced to take up the matter with the designers. By this point, we’ve already dedicated three development cycles to a single issue that should have been detected long ago. According to NIST, the cost has now increased 10 times what it should have been.

> we’ve already added three development cycles on a single issue.

Matters get even worse if the security bug makes it past integration and into the beta stage. To some degree, this is what the beta stage is for - testing and ironing out any remaining issues that prevent it from being put into productive use. But security shouldn't wait until then. 

First, we've seen how a lot of people have to duplicate their work once the problem filters back to the designer, and new requirements are provided to the coder. However, this time there is a chance that the beta testing is to be conducted in a live environment. The issue has now spread to select customers, and it may even be accessible to the more nefarious sorts out there.

You’ll notice that both coding and integration errors cost 30 times more to fix if they make it into production. At first glance this sounds like a high number, but given the amount of duplicate cycling through the different phases, plus other things like customer satisfaction, corporate reputation, and potentially financial losses due to attacks that exploit those issues, this number seems pretty fair.

> ... given the amount of duplicate cycling through the different phases, plus other things like customer satisfaction, corporate reputation, and potentially financial losses due to attacks that exploit those issues, this number seems pretty fair.

The most expensive characteristic associated to the discovery of security flaws in the production stage exhibits a strongly bidirectional impact. Production stage security flaws are invariably discovered on customer sites, and very most often because of a successful attack against *their* assets. 

Given the costs, one can see how the 5- or 6- digit bug bounties actually *save* money!

But now the potential impact has spread outside to customers and maybe even the general public. Negatively affected customers typically end up hiring external consultants to conduct a forensic investigation and analysis to discover how a particular attack happened and what was at fault so that the issues can be remedied. Otherwise they'll probably just get hacked again. And again. We do see a lot of that in the industry, too.

When it becomes apparent that the vulnerability was attributed to a bug in the applications they are using, they then often need to work with the vendor to help them understand the issue so they can, as in the previous stages, work their way through the application development stage from beginning to end. Sometimes another external security expert is brought in to facilitate and coordinate the response activities. 

The use of external experts at the customer site, multiplied by the number of hours needed to help the customer keep their site reasonably secured while still vulnerable to attack, plus all the activity at each level of the application development side adds up very quickly. In such a case, the values given in the NIST study may even be a little on the conservative side.

The good news is there are a number of considerations that can be made at the earliest stages to keep these redundant cycling costs down. In the next installment of this series, we’re going to investigate a Security Requirements stage, and then discuss more broadly how it directly and positively impacts the subsequent Design and Coding stages. Through understanding of these key factors, the application penetration tester is better able to provide robust mitigating recommendations.
