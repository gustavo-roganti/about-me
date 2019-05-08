## Amatori Web Ticketing System

###### Setting:
Amatori [[amatori.com](https://www.amatori.com)] is a maritime agency, its previous ticketing system relied on a SOAP service that was to be decommissioned. We had to rebuild the whole system, and we took advantage to refactor their website and to improve the usability of the ticketing process, leveraging on years of booking data to optimize the UX.

###### Challenges:
- The setup of a multilingual CMS
- The consumption of new external APIs providing ticketing services.
- The UX design and optimization of the ticketing system.  
- The implementation of the ticketing system with HTML5 and JavaScript.
- The creation of APIs to be used by third parties.

###### Process:

We adopted an Agile approach, splitting all the development in a series of iterations, that lasted two weeks. We were in constant communication with the client via Basecamp and via telephone calls.

###### Development:

Based on Pimcore, an enterprise CMS, I used Symfony to create the modules I needed:
- I wrote a module that consumed the external JSON API, relying on Redis to cache the results, and abstracting the more complicated calls.
- I designed and refined the UX of the ticketing system with our client, simplifying the process, and breaking the limits of the API through a layer of abstraction. We tuned the default settings based on previous bookings, and we pruned some options that were historically underused.
- I built the ticketing web app in JavaScript, with Symfony and PHP on the back-end. The various steps allow the user to choose voyage dates, passengers, accommodations and more, automatically applying discounts, and managing the payments using Stripe.
- I built an API server that offer a REST API to third parties to buy tickets. I documented the APIs using Swagger and I assisted the first few companies that started using our APIs.

###### Team:
I worked on this project with a sysadmin, a programmer that implemented all things CMS-related, a graphic designer and a frontend developer that built most of the HTML5 and SCSS.

###### Tools:
- Frameworks, documentation and build tools: Pimcore, Symfony, PHPDocs, Swagger, Grunt, SCSS, and more
- Tools to test, track and deploy: Vagrant, Git, Git Flow, Git Hooks, GitLab, XDebug, and others.
- To design and develop: Photoshop, Sketch, Balsamiq, PHPStorm, Sublime, and others.
