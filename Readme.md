# Architecture Resources

**Becoming A Software Architect:**

1. **Software Fundamentals** - I look at this section as general core knowledge - for people who have a more traditional CS background some of these things may be unnecessary but for someone like me a consolidated core knowledge about different aspects of software development has been crucial to progressing my skills.
    1. **Books** - read at will - they're not all necessary up front but go a long way in establishing codebase best practices for extending an initial architecture to dev teams
        1. [Clean Code](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882/ref=pd_lpo_14_img_0/147-4229037-8838224?_encoding=UTF8&pd_rd_i=0132350882&pd_rd_r=42536dd8-e88d-412c-9043-4eceaa1ca9f2&pd_rd_w=dNnDQ&pd_rd_wg=VJBlx&pf_rd_p=7b36d496-f366-4631-94d3-61b87b52511b&pf_rd_r=R94925AJQJ3TTPRH2Z3S&psc=1&refRID=R94925AJQJ3TTPRH2Z3S)
        2. [The Clean Coder](https://www.amazon.com/Clean-Coder-Conduct-Professional-Programmers/dp/0137081073/ref=pd_lpo_14_t_1/147-4229037-8838224?_encoding=UTF8&pd_rd_i=0137081073&pd_rd_r=42536dd8-e88d-412c-9043-4eceaa1ca9f2&pd_rd_w=dNnDQ&pd_rd_wg=VJBlx&pf_rd_p=7b36d496-f366-4631-94d3-61b87b52511b&pf_rd_r=R94925AJQJ3TTPRH2Z3S&psc=1&refRID=R94925AJQJ3TTPRH2Z3S)
        3. [The 12 Factor App](https://12factor.net/)
        4. [Clean Architecture](Jay's%20Ultimate%20Architecture%20Toolkit%201fad9efec97d4013a82ae024a0784762/https%20www%20amazon%20com%20Clean-Architecture-Craftsmans%2059062d9a7ff548349b597a35e2d2af65.md)
            - [https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
        5. [Architecture For Devs](https://leanpub.com/software-architecture-for-developers)

    2. **Core Skills** - specialize in 1, at least be familiar with the pieces in each
        1. **Backend**
            - backend developer roadmap - [https://roadmap.sh/backend](https://roadmap.sh/backend)
        2. **Frontend**
            - frontend developer roadmap - [https://roadmap.sh/frontend](https://roadmap.sh/frontend)
            - frontend concepts - [https://developers.google.com/web/ilt/pwa](https://developers.google.com/web/ilt/pwa)
        3. **Devops**
            - roadmap - [https://roadmap.sh/devops](https://roadmap.sh/devops)
            - Docker docker docker - learn to be able to dockerize all the things - "works on my machine" problems become extremely diminished and local development productivity is increased exponentially across the board
            - no matter what you do, learn enough devops to at least be able to deploy basic webservers and API's quickly as well as connect to different SaaS from different cloud providers quickly and efficiently as well as setup CI/CD pipelines for a **dev** environment
            - this will go a long way in getting a project up and running efficiently.  Also focus on dev/prod parity concepts from the 12 factor app - [https://12factor.net/](https://12factor.net/)
            - I can't honestly recommend learning the entirety of Kubernetes yet if you're going to be an architect - I have found that it's extremely helpful to know basic **kubectl** commands, how to port forward and exec to containers and how to view running container logs. I've also found it's helpful to understand the pieces and how they work - knowing that Kubernetes is handling SSL termination or Load Balancing can help identify where problems are.  Overall though, being able to Dockerize an app and lean on a Devops specialist has always gotten me where I need to go - ***WARNING* -** this is just my opinion and is subject to change based on my own personal journey / experience.  Overall I think I'm in the "camp" of people that think Kubernetes will be abstracted away to the point where I don't really need to know it

    3. **Core Tech - my ideal stack to be able to build *most* things** - this stack can be replicated in many ways, whether you know NodeJS + React or Java and VueJS doesn't really matter, the larger point is that you are **very** skilled in a backend tech, very skilled in a frontend tech, and you know how to quickly stand up a basic deployment pipeline for a dev environment. These technologies are not a one size fits all, but instead what I've found that I can "cover" most use cases with.  These have allowed me to learn less different language nuances and still build complex architectures that let me get exposure to real world examples of these concepts in action, those concepts being things like backend apis, frontend SPA's, basic deployments, CI/CD, Test Driven Development, Caching, Object Store, Document Store, NoSQL data modeling, SQL data modeling, rate limiting, messages, events, queues, eventual consistency, etc. (I could go on here but I think this gives the picture, knowing an end to end stack that lets you build what you need quickly is paramount)
        1. **NodeJS** (Javascript)
            1. The NodeJS Cookbook - [https://github.com/PacktPublishing/Node-Cookbook-3rd-Ed](https://github.com/PacktPublishing/Node-Cookbook-3rd-Ed)
            2. Speaking Javascript - [http://speakingjs.com/es5/](http://speakingjs.com/es5/)
            3. Javascript Design Patterns - [https://addyosmani.com/resources/essentialjsdesignpatterns/book/](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)
            4. Learn Typescript - [https://basarat.gitbook.io/typescript/](https://basarat.gitbook.io/typescript/)
            5. Learn how to write tests really well - [Jest](https://jestjs.io/)
            6. Know differences between Express, Fastify, NestJS, and Koa - all solve the same problem in different ways and expose a lot of NodeJS core knowledge
            7. all the awesome repos - [https://github.com/sindresorhus/awesome](https://github.com/sindresorhus/awesome)
        2. **Devops / Docker**
            1. Learn Docker really well
            2. [http://www.devopsbliss.com/webinar-registration-24143816](http://www.devopsbliss.com/webinar-registration-24143816) - do the free email course - it's awesome with hands on examples - do them!
        3. **React** - works as a nice "catchall" frontend "framework" to use although I'm investigating easier to use workflows
        4. **PostgresDB** - [https://wiki.postgresql.org/wiki/Main_Page](https://wiki.postgresql.org/wiki/Main_Page)
        5. **MongoDB**
            1. University - [https://university.mongodb.com/](https://university.mongodb.com/) - I took them all and didn't regret it
            2. [https://learnmongodbthehardway.com/](https://learnmongodbthehardway.com/)
            3. [https://thecodebarbarian.com/](https://thecodebarbarian.com/)
            4. At some point read most if not all the manual - [https://docs.mongodb.com/manual/](https://docs.mongodb.com/manual/)
        6. **Redis**
            1. University - [https://university.redislabs.com/](https://university.redislabs.com/)
            2. docs - [https://redis.io/documentation](https://redis.io/documentation)
        7. **RabbitMQ** - [https://www.rabbitmq.com/getstarted.html](https://www.rabbitmq.com/getstarted.html)
        8. **REST API** - [https://jsonapi.org/](https://jsonapi.org/) - I've found that specifications typically "outlive" frameworks and specific tech
        9. **JSON Schema** - [https://json-schema.org/](https://json-schema.org/) - another spec - allows validation and documentation with same code
        10. **Cloud Provider** - learn enough to do basic things - POC's, basic CI/CD for dev level environments, SSL, custom domains, stand up SaaS and connect live apps to them quickly
            1. **Azure** - you could swap azure for anything else but really the concepts of learning a lot of the pieces will transfer to any provider
                1. learn how to make a CI/CD environment that auto deploys to a develop environment
                2. Container apps
                3. databases
                4. azure functions - beware of pitfalls but they are super useful for some things
                5. blob storage
                6. Service Bus Queues and triggers
                7. Learning Path - [https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWtQqM](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWtQqM)
            2. **Heroku -**  so fast to deploy something you can't skip this one - for a one off app that requires a backend app this is great
            3. **Glitch -**  [https://glitch.me](https://glitch.me) - even faster but less useful - still good for quick sharing of code snippets
        11. **Test Driven Development**
            - [https://martinfowler.com/bliki/TestDrivenDevelopment.html](https://martinfowler.com/bliki/TestDrivenDevelopment.html)
            - [https://jaywolfe.dev/tdd-a-mongo-node-app/](https://jaywolfe.dev/tdd-a-mongo-node-app/)
            - [https://www.youtube.com/watch?v=l_UvUYUGRLg](https://www.youtube.com/watch?v=l_UvUYUGRLg)
            - 
2. **Architecture Fundamentals**
    1. **Building Microservices** - Sam Newman - [https://www.amazon.com/Building-Microservices-Designing-Fine-Grained-Systems/dp/1491950358](https://www.amazon.com/Building-Microservices-Designing-Fine-Grained-Systems/dp/1491950358)
    2. **Seven DBs in 7 weeks** - [https://www.amazon.com/Seven-Databases-Weeks-Modern-Movement-ebook/dp/B07CYLX6FD/ref=sr_1_3?crid=3DX6DX19HMHWH&dchild=1&keywords=seven+databases+in+seven+weeks&qid=1603401546&s=books&sprefix=seven+databases%2Cstripbooks%2C156&sr=1-3](https://www.amazon.com/Seven-Databases-Weeks-Modern-Movement-ebook/dp/B07CYLX6FD/ref=sr_1_3?crid=3DX6DX19HMHWH&dchild=1&keywords=seven+databases+in+seven+weeks&qid=1603401546&s=books&sprefix=seven+databases%2Cstripbooks%2C156&sr=1-3)
    3. **Effective Software Development** - [https://leanpub.com/effective-software-development-4-enterprise](https://leanpub.com/effective-software-development-4-enterprise)
    4. **Architect Training** - [https://www.developertoarchitect.com/](https://www.developertoarchitect.com/)
    5. **DB Changes** - [https://martinfowler.com/articles/evodb.html](https://martinfowler.com/articles/evodb.html)
    6. **Agile** - [https://martinfowler.com/agile.html](https://martinfowler.com/agile.html)
    7. Basically everything on these two sites: (Even if you're not building microservices it will teach you tons of ways to look at technology)
        1. [https://martinfowler.com/](https://martinfowler.com/)
        2. [https://microservices.io/](https://microservices.io/)
    8. **Design Patterns**
        - Event Sourcing, Repository Pattern, Singleton, Factory, CQRS, Circuit Breakers, POJOs
        - [https://c4model.com/](https://c4model.com/)
        - [https://www.dofactory.com/javascript/design-patterns](https://www.dofactory.com/javascript/design-patterns)
        - Examples In JS Code - [https://github.com/fbeline/design-patterns-JS](https://github.com/fbeline/design-patterns-JS)
        - [Design Patterns Gang of 4 Book](https://www.amazon.com/gp/product/0201633612/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)
    9. **Domain Driven Design**
        - [https://martinfowler.com/tags/domain driven design.html](https://martinfowler.com/tags/domain%20driven%20design.html)
        - [Tough Book but awesome - will change the way you think on DDD](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215)
    10. **Blog Series**
        1. [https://medium.com/@nvashanin/the-path-to-becoming-a-software-architect-de53f1cb310a](https://medium.com/@nvashanin/the-path-to-becoming-a-software-architect-de53f1cb310a)
        2. [https://medium.com/@patrickleet](https://medium.com/@patrickleet) - pretty much everything from this guy
    11. **Breaking down a use case**
        1. Who are the users?
        2. What is the business?
        3. What is expected traffic?
            1. Load testing
        4. Who is the subject matter expert?
        5. What is the main problem to solve?
        6. What are my constraints?
            1. Team (team knowledge and experience level, specialties, etc)
            2. Env (what cloud env, cost concerns, deployability)
            3. Is this existing application?
            4. Language Constraints?
            5. Who will maintain it?
            6. Logging requirements?
            7. KPI's - identifying these early and often is mega important
            8. Do I have Devops? If not then keep deployment as simple as possible - this is a good rule of thumb anyways but can be relaxed for speed if dedicated devops is available
        7. Prioritize iteration speed - productive developer workflow is paramount and will pay dividends
3. **Weekly Tech Subscriptions (\* Beside the ones I NEVER skip reading)**
    1. Serverless Weekly* - [https://serverless.email/](https://serverless.email/)
    2. NodeJS Weekly* - [https://nodeweekly.com/](https://nodeweekly.com/)
    3. Javascript Weekly - [https://javascriptweekly.com/](https://javascriptweekly.com/)
    4. Kubernetes Weekly - [https://kubeweekly.io/](https://kubeweekly.io/)
    5. Frontend Focus - [https://frontendfoc.us/](https://frontendfoc.us/)
    6. React Weekly - [https://react.statuscode.com/](https://react.statuscode.com/)
    7. Postgres Weekly - [https://postgresweekly.com/](https://postgresweekly.com/)
    8. DB weekly* - [https://dbweekly.com/](https://dbweekly.com/)
    9. MongoDB Memo - [https://mongodb.email/](https://mongodb.email/)
    10. Hacker News Weekly  - [https://hackernewsletter.com/](https://hackernewsletter.com/)
    11. Deno Weekly - [https://denoweekly.com/](https://denoweekly.com/)
    12. Architect lessons - [https://www.developertoarchitect.com/lessons/](https://www.developertoarchitect.com/lessons/)
4. **Smart People's Blogs I Follow**
    1. [https://www.tutisani.com/software-architecture/](https://www.tutisani.com/software-architecture/)
    2. [https://thecodebarbarian.com/](https://thecodebarbarian.com/)
    3. [https://blog.cleancoder.com/](https://blog.cleancoder.com/)
5. **Major Architecture Patterns To Study**
    1. CRUD Monolith
    2. SOA
    3. Microservices
    4. Event Sourced and Event Driven / CQRS

        [Joys Of Event Sourcing NodeJS](event-sourcing.md)

6. **Sample Apps That Can Help You Learn Anything**
    1. Todo List
    2. Url shortener
    3. Chatbot
    4. Live Chat App
    5. Webhook Inspection Tool
    6. anything you can come up with!
7. **Product Mindset - Everything Is A Product**
    - [https://apievangelist.com/2012/01/12/the-secret-to-amazons-success-internal-apis/](https://apievangelist.com/2012/01/12/the-secret-to-amazons-success-internal-apis/)
    - [The Lean Startup](https://www.amazon.com/Lean-Startup-Entrepreneurs-Continuous-Innovation/dp/0307887898)
8. **Podcasts**
    - [https://6figuredev.com/](https://6figuredev.com/)
    - [https://syntax.fm/](https://syntax.fm/)
    - [https://www.indiehackers.com/podcast](https://www.indiehackers.com/podcast)
    - [https://anchor.fm/profitablepythonfm](https://anchor.fm/profitablepythonfm)
9. **Systems Design**
    - https://github.com/donnemartin/system-design-primer/blob/master/README.md#system-design-topics-start-here
