# Engineering practices in big tech

## Google
* <ins>Eng. Practices Guide ([wiki](https://google.github.io/eng-practices/))</ins>
* <ins>Software Engineering at Google ([paper](https://arxiv.org/pdf/1702.01715.pdf))</ins>
   * **Software development**
     * development always at "head"
     * code ownership
     * hermetic build system
     * each push must be reviewed by at least one engineer
     * small changes encouraged over bigger ones (CLs labeled as S, M, L, XL)
     * Buganizer: bug tracking system. Bug triage practices
     * insist on using limited number of (5) programming languages: C++, Java, Python, Go, or JavaScript
          * advantage: 
            * reduces obstacles to code reuse and programmer collaboration
          * Protocol buffers for interoperating between different programming languages
          * single command set for usual tasks no matter which language (e.g. check out, edit, build, commit, file bug, ...)
      * canary services
      * post-mortems
      * Frequent software re-writes (each 1-2 years) !!
          * benefits exceed the cost
          * motivations:
            * requirements change significantly in few years in a typical project, software designed around old requirements is most of the time not optimal for current requirements
            * software accumulates complexity over years
          * benefits:
            * increases sense of ownership of new engineers in the project
            * encourages mobility of engineers between projects
            * ensure code is written in recent tech and methodology
          * costs:
            * time spent
    * **Project management**
       * each engineer allowed to spend upto 20% time on any project
       * Objectives and Key Results (OKRs)
    * **People management**
       * tech leadership and people management distinction
       * seperate career progression for engineering and management
       * Roles:
          * Engineering manager
             * selects tech leads, responsible for team performance, coaching assistance in career development, performance evaluation, some aspects of compensation and hiring
             * manages 3 to 30 people. 8 to 12 is most common
          * Software Engineer
          * Research scientist
          * Site-realibility engineer (SRE)
          * Product manager
          * Program manager / Technical program manager
            * similar to product manager, buut rather than product manages processes (e.g. data collection)
    * **Facilities**
      * open plan seatings
        * Pros: encourage communation, economical
        * Cons: less concentration
        * Blog arguing against open offices 
           * some research/news suggesting open office is a bad idea: ([blog](https://stackoverflow.blog/2015/01/16/why-we-still-believe-in-private-offices/)), [damages productivity](https://www.dezeen.com/2014/11/21/open-plan-office-designs-unpopular-with-workers-damage-productivity/), [less satisfaction](https://journals.sagepub.com/doi/abs/10.1177/0013916502034003001), [open-office trap](https://www.newyorker.com/business/currency/the-open-office-trap)
* <ins>What It Takes to Get Certified to Review Code At Google ([news](https://dev.to/pullrequest/getting-the-certification-to-review-code-at-google-55ng))</ins>
* <ins>Modern Code Review: A Case Study at Google ([paper](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/80735342aebcbfc8af4878373f842c25323cb985.pdf))</ins>
* <ins>Why Google Stores Billions of Lines of Code in a Single Repo ([talk](https://www.youtube.com/watch?v=W71BTkUbdqE))</ins>
   * Trunk-based development
   * Advantages of a monolithic repo
      * single source of truth
      * diamond dependency problem
      * easier to modernize codebase
   * tooling support
      * code review, code search, tricorder, presubmits, testing before and after commit, auto roll-back, change distribution and management
   * Warning: this may or may not be the right approach for your company
      

## Microsoft
* <ins>Company's Research department for empricial research on software productivity. Find many research papers at ([RISE website](https://www.microsoft.com/en-us/research/group/research-software-engineering-rise/))</ins>

## LinkedIn
* <ins>Scaling Collective Code Ownership with Code Reviews ([blog](https://engineering.linkedin.com/blog/2018/06/scaling-collective-code-ownership-with-code-reviews)) ([talk](https://scna.softwarecraftsmanship.org/#7)) -> gives links to very useful empirical research papers</ins>
* <ins>Effective Code Reviews and File Ownerships ([blog](https://engineering.linkedin.com/blog/2016/01/effective-code-reviews-and-file-ownerships))</ins>

## Netflix
* <ins>How we build code at Netflix ([blog](https://medium.com/netflix-techblog/how-we-build-code-at-netflix-c5d9bd727f15))</ins>

## Review Papers
* <ins>Rigby, Bird. 2013. ACM. Convergent Software Peer Review Practices ([Microsoft Research paper](https://www.microsoft.com/en-us/research/publication/convergent-software-peer-review-practices/))</ins>
    * *"We examine two Google lead projects, Android and Chrome, three Microsoft projects, Bing, Office, and MS SQL, and one project internal to AMD. We contrast our findings with data taken from traditional software inspection conducted on a Lucent project, a compiler, and from open source software peer review on six projects, including Apache, Linux, and KDE"*

## Empiricial Studies
* <ins>Bird, Bacchelli. 2013. IEEE. Expectation, Outcomes, and Challenges of Modern Code Review ([Microsoft Research paper](https://www.microsoft.com/en-us/research/publication/expectations-outcomes-and-challenges-of-modern-code-review/))</ins>
  <ins>  * *"We empirically explore the motivations, challenges, and outcomes of tool-based code reviews. We observed, interviewed, and surveyed developers and managers and manually classified hundreds of review comments across diverse teams at Microsoft"*</ins>
* <ins>Code Reviewing in the Trenches: Understanding</ins>
* <ins>Challenges, Best Practices and Tool Needs ([Microsoft Research paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/05/MS-Code-Review-Tech-Report-MSR-TR-2016-27.pdf))</ins>
* <ins>The Best Kept Secrects of Peer Code Review ([Palantir book](https://smartbear.com/resources/ebooks/best-kept-secrets-of-code-review/))</ins>

## Resource resources
* <ins>Software Craftmanship North America Conference ([talks](https://scna.softwarecraftsmanship.org/#7))</ins>

## Insights from classics
* The Mythical Man-Month (https://www.amazon.com/Mythical-Man-Month-Software-Engineering-Anniversary/dp/0201835959/ref=sr_1_1?crid=39RLOV4C701C0&keywords=the+mythical+man+month&qid=1572769488&sprefix=the+mythical+man+%2Caps%2C517&sr=8-1)
  * adding manpower to a late software project makes it later (known as Brook's Law)
  
## Little related
* "The idea behind microservices is that some types of applications become easier to build and maintain when they are broken down into smaller, composable pieces which work together." ([blog](https://francois-encrenaz.net/an-introduction-to-microservices/))
