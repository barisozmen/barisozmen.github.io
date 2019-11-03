# Engineering practices in big tech

## Google
* _Eng. Practices Guide ([wiki](https://google.github.io/eng-practices/))_
* _Software Engineering at Google ([paper](https://arxiv.org/pdf/1702.01715.pdf))_
* _What It Takes to Get Certified to Review Code At Google ([news](https://dev.to/pullrequest/getting-the-certification-to-review-code-at-google-55ng))_
* _Modern Code Review: A Case Study at Google ([paper](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/80735342aebcbfc8af4878373f842c25323cb985.pdf))_
* <ins>Why Google Stores Billions of Lines of Code in a Single Repo ([talk](https://www.youtube.com/watch?v=W71BTkUbdqE))</ins>
   * Trunk-based development
   * Advantages of a monolithic repo
      * single source of truth
      * diamond dependency problem
      * easier to modernize codebase
   * tooling support
      * code review
      * code search
      * tricorder
      * presubmits
      * testing before and after commit, auto roll-back
      * change distribution and management
   * Diamond dependency problem
   * Warning: this may or may not be the right approach for your company
      

## Microsoft
* _Company's Research department for empricial research on software productivity. Find many research papers at ([RISE website](https://www.microsoft.com/en-us/research/group/research-software-engineering-rise/))_

## LinkedIn
* _Scaling Collective Code Ownership with Code Reviews ([blog](https://engineering.linkedin.com/blog/2018/06/scaling-collective-code-ownership-with-code-reviews)) ([talk](https://scna.softwarecraftsmanship.org/#7)) -> gives links to very useful empirical research papers_
* _Effective Code Reviews and File Ownerships ([blog](https://engineering.linkedin.com/blog/2016/01/effective-code-reviews-and-file-ownerships))_

## Netflix
* _How we build code at Netflix ([blog](https://medium.com/netflix-techblog/how-we-build-code-at-netflix-c5d9bd727f15))_

## Review Papers
* _Rigby, Bird. 2013. ACM. Convergent Software Peer Review Practices ([Microsoft Research paper](https://www.microsoft.com/en-us/research/publication/convergent-software-peer-review-practices/))_
    * *"We examine two Google lead projects, Android and Chrome, three Microsoft projects, Bing, Office, and MS SQL, and one project internal to AMD. We contrast our findings with data taken from traditional software inspection conducted on a Lucent project, a compiler, and from open source software peer review on six projects, including Apache, Linux, and KDE"*

## Empiricial Studies
* _Bird, Bacchelli. 2013. IEEE. Expectation, Outcomes, and Challenges of Modern Code Review ([Microsoft Research paper](https://www.microsoft.com/en-us/research/publication/expectations-outcomes-and-challenges-of-modern-code-review/))_
  _  * *"We empirically explore the motivations, challenges, and outcomes of tool-based code reviews. We observed, interviewed, and surveyed developers and managers and manually classified hundreds of review comments across diverse teams at Microsoft"*_
* _Code Reviewing in the Trenches: Understanding_
* _Challenges, Best Practices and Tool Needs ([Microsoft Research paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/05/MS-Code-Review-Tech-Report-MSR-TR-2016-27.pdf))_
* _The Best Kept Secrects of Peer Code Review ([Palantir book](https://smartbear.com/resources/ebooks/best-kept-secrets-of-code-review/))_

## Resource resources
* _Software Craftmanship North America Conference ([talks](https://scna.softwarecraftsmanship.org/#7))_
