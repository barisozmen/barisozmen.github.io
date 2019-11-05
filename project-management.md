## References
* What We Actually Know About Software Development, and Why We Believe It’s True ([talk](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/))
* Have Agile Techniques been the Silver Bullet for Software Development at Microsoft? ([2016. Murphy et al. Microsoft Research](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Agile20Trends20ESEM20Master.pdf))
* Agile at scale ([HBR article](https://hbr.org/2018/05/agile-at-scale))
* [Microsoft Research blog: Exploding Software Engineering Myths](https://www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/)
  * Code coverage doesn't predict code quality
  * Test-driven development leads to 60-90% fewer bugs, but takes 15% tp 35% more time
  * Assertions are very useful ([Kudrjavets et al, 2016. Microsoft Research](https://www.microsoft.com/en-us/research/publication/assessing-the-relationship-between-software-assertions-and-code-qualityan-empirical-investigation/))
  * How developers in the team are distant by hierarchy is more important than geographical distance ([Nagappan et al., 2008, Microsoft Research](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/))
  * Similar papers referenced by [this talk](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/)
* [www.linkedin.com/learning/agile-software-development](https://www.linkedin.com/learning/agile-software-development)


## Agile Software Development - LI Learning course and other resources
[www.linkedin.com/learning/agile-software-development](https://www.linkedin.com/learning/agile-software-development)
 * Extreme programming (XP)
   * developed by Kent Beck in 90s
   * weekly cycle, quarterly cycle
   * stories, tasks
   * XP team includes customers
   * team members sit together, minimal barriers to information (informative workspace)
 * XP execution
   * test-driven development (TDD)
     * method: 1) write a test that fails, 2) make only enough code for it to pass, 3) improve code quality
     * According to [Nagappan et al., 2016, Microsoft Research](https://www.microsoft.com/en-us/research/wp-content/uploads/2009/10/Realizing-Quality-Improvement-Through-Test-Driven-Development-Results-and-Experiences-of-Four-Industrial-Teams-nagappan_tdd.pdf), TDD teams makes 60% to 90% better in terms of defect density, while they spend 15% to 35% longer time to complete same project.
     * as a result, spend good time on refactoring
     * Automated unit testing
   * build process should be less than 10 minutes
   * pair programming
     * one writes code, other reviews code
     * From an empricial study on pair programming ([Microsoft Research paper](https://www.microsoft.com/en-us/research/publication/pair-programming-whats-in-it-for-me/)): 
       * "The biggest perceived benefits of pair programming were the introduction of fewer bugs, spreading code understanding, and producing overall higher quality code. The top problems were cost-efficiency, (work time) scheduling problems, and personality conflicts. Most engineers preferred a partner who had complementary skills to their own, who was flexible and had good communication skills"
     
     * [Pros and Cons](https://www.freecodecamp.org/news/the-benefits-and-pitfalls-of-pair-programming-in-the-workplace-e68c3ed3c81f/)
   * continuous integration (CI)
   * [Slack](https://explainagile.com/agile/xp-extreme-programming/practices/slack/): low priority tasks that can be postponed without worry
     * Examples Slacks: Adding tests to a legacy code, Paying off a technical debt such as improving a build system, Architectural refactoring, Improvements to testing strategies such as a mocking a database
 * Many Agile teams combine XP practices with Scrum
   * XP prescriptive and implementation centric as opposed to Scrum which is non-prescriptive and abstract in nature
 * Story (User story)
   * who wants + what is wanted + why wanted
   * e.g. As a fitness club member [user], I should be able to view my payment history [what is wanted] so I know how I am being billed [motivation]
   * Success criteria
     * e.g. User should be able to view payments made in the last two years."
   * Lack of specific details which is intentional
     * not aiming to meet contractual obligations
     * promise for a conversation between product owner and development teams
   * 3Cs: card, conversation, confirmations
 * Epic
   * A large user story
   * Represents a business work low or process and is too large to be estimated
   * Think epic as workflow diagrams
   * e.g. "As a fitness club manager, I should be able to set up a new club member account. Setting up a customer account includes setting up their name, address, phone number, and their payment information. Many clubs store a picture of the member. The process may include processing the sign-up fee and the first month's fee. It would likely include setting up payment information so the club could automatically process monthly"
 * Theme
   * a way of grouping user stories
   * e.g security, mobile, web etc.
 * If you cannot write a user story on a card, it is probably an epic
 * Agile Estimation
   * estimates provided by team members, not managers
   * Absolute unit estimation vs. Relative unit estimation
     * as work become more complex, variation in time increase
   * Fibonacci scale, vs. Exponential scale
   * item time can be estimated as infinity (too big, complicated), or as question mark (not enough information to estimate)
 * Planning Poker
   * 
   
## Empricial evaluation of Agile and Critics
* Have Agile Techniques been the Silver Bullet for Software Development at Microsoft? ([2016. Murphy et al. Microsoft Research](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Agile20Trends20ESEM20Master.pdf))
  * **Results:** *"The survey results reveal that despite intense market
pressure, the growth of agile adoption at Microsoft is slower than
would be expected. Additionally, no individual agile practice
exhibited strong growth trends. We also found that while
development practices of teams may be similar, some perceive
and declare themselves to be following an agile methodology
while others do not. Both agile and non-agile practitioners agree
on the relative benefits and problem areas of agile techniques."*
  * **Conclusions:** *"We found no clear trends in practice adoption.
Non-agile practitioners are less enamored of the benefits and
more strongly in agreement with the problem areas. The ability
for agile practices to be used by large-scale teams generally
concerned all respondents, which may limit its future adoption."* 

   
   


