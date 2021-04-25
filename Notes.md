# Outline

* intro
* trends risks
* characteristics of frameworks 
  * why frameworks - remove choice - freedom is slavery - constraints liberate
* Functional programming and haskell
* 2 executables 
  * automation framework
  * quickstep
* Support structures

# Detail
* time intro
  * business systems
  
* trends risks
  * risk intro - pyramid 

  * MYOB - Huxley
    *  https://digitalfirst.com/opinion-cloud-brings-hard-questions-for-myob-and-reckon/
    *  https://www.itnews.com.au/news/myob-a-lesson-in-how-to-bungle-a-beta-284370
    *  Big bangs end in big bangs
    *  John Mitch - Barry

  * packages - scope reduction - open sourced / outsourced / orchestrated
 
  * microservices
    * conways law
    * problems / tooling 
    * risk - innovation - heterogeneous
    * evolution - Barrak Obarma
    * modularity - testing types A/B
      * https://blog.optimizely.com/2010/11/29/how-obama-raised-60-million-by-running-a-simple-experiment/
    * amazon podcast example
    * cqrs / persistent message question
    * testing in production
    * the rise and rise of monitoring
    * meta-level WFH Covid - services - plug in 
  * devops 
  * devops culture

  * the strongly typed functional paradigm 
    * more later - more powerful compiler - risk elimination

Key Principles
    * risk elimination
    * decrease impact
    * decrease scope
    * time compression
    * decrease contexualise risk

Future
    * there is still going to be manual testing but less
    * there will still be automation but less
    * high risk domains
    * laggards large complex domain specific systems
      * more effective manual testing
      * different types of testing
      * manual testers -> domain experts
    * more effective automation 
    * better integration between automation

Why Frameworks
  * Consistent
  * Reusable
  * Concrete Implementation of an Opinionated Solution
  * Most importantly It Eliminates Choice - Constraints Liberate, Liberties Constrain — Runar Bjarnason

Automation Framework Principles 
  * How is end to end automation different to unit testing 
    * application stack
    * people stack
      * https://www.youtube.com/watch?v=U0tpjs8zflQ
    * type 2 errors
    * logging reporting
    * magnitudes slower
    * will be worked on by lower skilled devs
    * 
  * its not a unit test
  * it will always be wrong - refactor early, hard and often
  * semantic layers
    * test layer    - Tests
    * domain layer  - Helpers
    * utils layer   - Domain Independent Functions (time, web interactions, REST calls)
    * further specific layering 
      * Browser / Appium Based
        * read
        * write
        * navigate
        * seek and set functions
        * setForm
        * auto-generate set form
        * cache session
      * REST Based
        * specific seek and set functions JSON 
  * execution separated into layers 
    * data generation                     - pure
    * aut interaction                     - impure
    * parsing aut data -> domain object   - pure
    * validation of domain object         - pure
  * highly focussed on data driven testing
    * object lists
    * generative testing
  * multiple asserts in one test
  * big emphasis on logging reporting
  * utilise existing packages and libraries such as Selenium / Appium / C# rest ?? 
  * heavy use of types and functional programming concepts
  * must be OSS

2 Projects
  * DRY
    * I'm a hypocrite
    * I can see a day coming when it will be feasable 
    * pick and stick
    * paradigm and language which:
      * has a type system which eliminates a huge amount of risk
      * separates purity from state
      * highly expressive  
      * is highly re-factorable
      * paradigm is functional programming and the language is the canonical FP language which is haskell 

What is FP
  * history
    * Alonzo Church 
    * Alan Turing
  * Simon Peyton Jones - describes Functional programming
  * https://youtu.be/zLMN34DB5Ms?t=200
  * higher order functions
  * declarative statelessness is pervasive
    * Devops - gitops
    * Dhall
    * Nix
  * split languages
    * C#
  * other languages
  * https://www.youtube.com/watch?v=9_cUNM0H8QU&t=21s
  * Haskell moving

What is Haskell - Why Haskell
  * history
  * no variables
  * no loops
  * only values and functions
  * functions can only take one parameter
  * higher kinded types
  * parse don't validate
  * pattern matching
  * pioneered property based testing

Problem with haskell
  * overwhelming 
  * thesisware
  * language extensions
  * Haskell from first principles - 1196
  * What I Wish I Knew When Learning Haskell - 482 pages
  * language extensions
  * Lens / effects system
  * Tooling

Response 
  * Framework
  * HLS
  * Updates
  * Haskell Foundation
  * Haskell - crossing the Chasm

# Describe Projects
  * Pyrethrum
  * Quickstep 
    * Similarly eliminate duplication
    * Dhall - LiveSpec
    * generate data
    * demo outcomes
    * import into automation
    * integrated with VSCode
  * integration between 
    * same log protocol
    * coverage parsing machinery

# Support 
  * available all the time constantly monitoring
  * escalation points
  * further developments

# Wrap Up
  * its really happening
  * John Mitch
    * REA
    * MYOB
    * AfterPay
  * Sydney Slides

# Everything

  * key principles
    * orchestration
    * shift left - where does it end
    * declarative
    * time compression
    * more powerful compiler
    * https://docs.google.com/presentation/d/1UOBjsyutb41sJywa1vksvMqFuCIAwt4JtTFX7S8QxsM/edit#slide=id.g3bd06b3138_0_44
    

* photo
  * https://www.youtube.com/watch?v=FpVqUOCQjlY - Time
  * https://soundcloud.com/infoq-channel/clare-liguori-on-automating-safe-and-hands-off-deployments-at-aws - integration tests 34 mins - canary deployments 
  
* declarative / deterministic 
* remote control 
* https://www.gitpod.io/features
* https://nixos.org/
* https://www.weave.works/technologies/gitops/

* separate data from control
* components as services (eg logging and presentation)

* vscode and LSP
* https://www.youtube.com/watch?v=JWM4J2TLGNQ
* lambda man

* property based testing - algebra driven design
* https://youtu.be/2SAQNO46V3U?t=157

* https://docs.google.com/presentation/d/1a4GvI0dbL8sfAlnTUwVxhq4_j-QiDlz02_t0XZJXnzY/edit#slide=id.ga932d2c2b_1292
* https://yowconference.com/talks/josh-godsiff/yow-lambda-jam-2018/the-human-side-of-haskell-6115/ - bread example - higher kinded types - context


* https://github.com/dhall-lang/dhall-lang - Dhall 
* Crossing the Chasm - https://corecursive.com/040-tech-evangelism-with-gabriel-gonzalez/
  * https://www.ignitionframework.com/crossing-the-chasm-theory-how-to-market-sell-and-improve-your-new-invention/

* marketing 
  * remember your priors
  * not always - when not
    * components - work flow, data generation, reporting
    * concepts
  * seen it fail - AFL
  * share the narrative
  * demonstrate the artifacts 
  * have a strategy and capacity to back it up
  * instill confidence

* Simon Peyton Jones - describes Functional programming
  * https://youtu.be/zLMN34DB5Ms?t=200

* risk % 
  * Obama killing Binladen - risk %
