# Software Engineering Career Ideas


## Most important skills

### Knowing how to solve problems
- Have grit
- Know how to ask questions. Questions should include:
    - a summary of problem
    - error message
    - what did you do
    - what happened
    - any situational cases other person should know
- Know who to ask questions (Google, stackoverflow, Slack, Jira, Wiki, Teammate)
- Keep track of your teammates strengths, use their brains
- Debugging techniques ([1](https://courses.cs.washington.edu/courses/cse331/17wi/lec15/lec15-debugging-4up.pdf))
  - reproduce error
  - Binary search (use with Git versioning) (can try git bisect)
  - think like a scientist
     - Rule out possibilities
     - Test assumptions
  - put prints/logs in the code
  - use assertions for edge cases
  - Use best Editors (PyCharm, IntellIJ): breakpoints, step into, step over, step out
  - Some bugs are different in nature, and too rigid rules may not be best to find it. Be creative at these times. Examples are bugs happen depending on external condition like temperature of system, data load etc. Other examples are Machine Learning software bugs (technically they may not be bugs at all)
  - If solving a particular bug takes time, just switch to another task, or take a walk, rest. A solution may come to your mind instantly, your brain will be going over it on the back log. If not, at least you will be better at solving after you refresh.
- After solving a problem, bug
  - retrospect on why it happened, understand the cause
  - add a unit test
- Have sense on where bugs would be hiding mostly.
- Be well literate of info/warning/error loggings. try understand coming error types (exceptions) for language.
- Think on causes of bugs, think on internals of language.

### Fast code reading skill
- Understand API's you are using from reading the source code. It's more reliable than documentation.
- Practice fast code reading, at first it's hard, but later it can be easier to read from code than the documentation

### Adaptability to new tech
Software engineering stack is rapidly changing. Learning any tool very well would lose its value in 5-10 years. What is important is learning how to learn a new tool/tech faster. Which involves:
    - Knowing where to find resources, 
    - who to get insights from. 
    - Know how to do experiments with code, do perturbation for understand how its internals are working.
    
 Always follow blogs, observe others about best practices on X. Pitfalls for Y.
    
### Sense for where to invest next
Should know learning what would provide highest return of investment (ROI). Always prioritize your learning by that.

### Learning tools best for maximum productivity
Learn productivity tools and how to orchestrate them together extremely well. These tools will be changing by time and are ever improving. Therefore always be searching for better productivity tools. Upgrade/change them if a change would make you more productivity. For today (2019), most important ones are:
 - Profile yourself. Where do you spend most time? Which tool? Whic process? Optimize processes, tools taking the most time. Have an eye on pain points!! (analoguos to [code profiling](https://en.wikipedia.org/wiki/Profiling_(computer_programming)))
    - idea: profile yourself like a statistical code profiler. Set alarm to random times, and note what you are doing at each exact time.
 - Editor (Intellij, Pycharm)
    - use best editors always, affects productivity a lot
    - master code navigation (e.g. jump to function definition (command+B), jump back to previous place (command+<-))
    - master code completion (e.g. change all usages of one variable at same time (ctrl+R))
 - Code review
    - write your code, and prepare descriptions, having in mind others will read over and over
    - write for others
    - be very structured between different CRs
 - Git
    - master code versioning. you can control it over IntellIJ as well. Very important during debugging. keep points in time, so you can return back, or do **binary search** on changes for finding bug sources. It is log faster than searching bugs one change at a time.
 - Jira
    - how to plan all work. be able to note anything coming to your mind. have a light structure
    
### Read classical books, Follow best people, learn best practices and common pitfalls
Classical books:
 - Pragmatic programmer
 - Design patterns
 - Clean Code / Architecture
 - Coders at work
 - Code Complete
 - Hackers & Painters
 - Zero bugs
 - Google resume and green book
 
 
### Avoiding bugs
 - simple coding
 - assertions for edge cases
 - unit testing
 - CI/CD
 - Murphy law applies as if things may go wrong, they will
 - Book: [Zero Bugs and Program Faster](https://www.amazon.com/Zero-Bugs-Program-Faster-Thompson/dp/0996193308/ref=asc_df_0996193308/?tag=hyprod-20&linkCode=df0&hvadid=312091457223&hvpos=1o1&hvnetw=g&hvrand=2253535076960508376&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1014221&hvtargid=aud-829758849484:pla-521736069013&psc=1&tag=&ref=&adgrpid=62820903995&hvpone=&hvptwo=&hvadid=312091457223&hvpos=1o1&hvnetw=g&hvrand=2253535076960508376&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1014221&hvtargid=aud-829758849484:pla-521736069013)

    
 ## References
 ### Debugging
 1. [Debugging lecture](https://courses.cs.washington.edu/courses/cse331/17wi/lec15/lec15-debugging-4up.pdf) by Professor Norm Matlof, UC Davis, 
  
 
