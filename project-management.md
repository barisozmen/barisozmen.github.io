

Agile Software Development - LI Learning course and other resources
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
 * Story
   * e.g. As a fitness club member [user], I should be able to view my payment history [what is wanted] so I know how I am being billed [motivation]
   * who wants + what is wanted + why wanted
   
   
Empricial evaluation of Agile and Critics
  * 
   
   

[Exploding Software Engineering Myths](https://www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/)
  * Code coverage doesn't predict code quality
  * Test-driven development leads to 60-90% fewer bugs, but takes 15% tp 35% more time
  * Assertions are very useful ([Kudrjavets et al, 2016. Microsoft Research](https://www.microsoft.com/en-us/research/publication/assessing-the-relationship-between-software-assertions-and-code-qualityan-empirical-investigation/))
  * How developers in the team are distant by hierarchy is more important than geographical distance ([Nagappan et al., 2008, Microsoft Research](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/))
  * Similar papers referenced by [this talk](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/)

## References
[www.linkedin.com/learning/agile-software-development](https://www.linkedin.com/learning/agile-software-development)
[www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/](https://www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/)
What We Actually Know About Software Development, and Why We Believe It’s True ([talk](https://www.microsoft.com/en-us/research/publication/the-influence-of-organizational-structure-on-software-quality-an-empirical-case-study/))
Have Agile Techniques been the Silver Bullet for Software Development at Microsoft? ([2016. Murphy et al. Microsoft Research](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Agile20Trends20ESEM20Master.pdf))
