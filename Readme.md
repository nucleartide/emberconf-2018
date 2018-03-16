![oh no](https://user-images.githubusercontent.com/914228/37348426-431dcaa6-2691-11e8-9e41-91fb5a5f0e5c.png)

# EmberConf 2018

A collection of links (and notes) that summarize the events of EmberConf 2018. Please submit a PR if you'd like!

Inspired by [**@poteto**](https://github.com/poteto)'s past EmberConf repos. See [2017](https://github.com/poteto/emberconf-2017), [2016](https://github.com/poteto/emberconf-2016), and [2015](https://github.com/poteto/emberconf-2015) for previous years!

## Livestream

> <img alt="" src="https://user-images.githubusercontent.com/914228/34072730-9d2d0bcc-e25a-11e7-9ab5-405ddce05303.gif" width="25"> <img alt="" src="https://user-images.githubusercontent.com/914228/34072749-07a8ab50-e25b-11e7-80ba-d0f6250aad11.png" width="20.5">

- Official live stream
  - [Day 1](https://www.youtube.com/watch?v=qfnkDyHVJzs&feature=youtu.be)
  - [Day 2](https://youtu.be/bt9MRkf5Mus?t=1080)

## Other Blogs & Highlights
- [Alex's Talk Highlights](https://alexdiliberto.com/posts/emberconf-2018-notes/)

## Job board

See photos [here](https://github.com/nucleartide/emberconf-2018/tree/master/job-board). Pictures were taken around 1 PM PST on Wednesday March 14.

## Day 1

### Talks

#### Keynote by [Tom Dale](https://twitter.com/tomdale) and [Yehuda Katz](https://twitter.com/wycats)

_Overall, lots of API improvements, as well as exciting advances in Glimmer.js._

- [Video](https://youtu.be/qfnkDyHVJzs?t=1h2m25s)
- [Slides](https://speakerdeck.com/tomdale/emberconf-2018-keynote)
- New filesystem layout
- Optional jQuery
- Codemods
  - `async`/`await` in tests
  - JS module api
  - Computed properties, use es5 getters
  - ES6 classes
    - TypeScript
  - Decorators
- Editor integration
  - [VSCode](https://code.visualstudio.com/docs/languages/typescript)
- Fragment components, empty tagName
- `@tracked` properties, autotracking dependencies
- `@args` syntax in templates
- Experimental
  - Angle bracket syntax
  - Single word component names
  - Named blocks RFC
- [LinkedIn feed in Preact and Glimmer](https://engineering.linkedin.com/blog/2018/03/how-we-built-the-same-app-twice-with-preact-and-glimmerjs)
- https://schedule.emberconf.com - uses rehydration
- https://schedule-wasm.emberconf.com - uses WASM
  - [Glimmer written in Rust](https://github.com/glimmerjs/glimmer-vm/pull/752)

#### Brief interlude from sponsor [Percy.io](https://percy.io) by [Mike Fotinakis](https://twitter.com/mikefotinakis?lang=en)

Percy.io is "Solving visual testing across design, development, and deployment." "Stop doing QA in the dark. See every pixel changed on every pull request."

- [percy.io](https://percy.io/)
- [percy-web](https://github.com/percy/percy-web), open source front-end
- [Example of PR integration](https://github.com/percy/percy-web/pull/459)

#### Ambitious for All: Accessibility in Ember by [Melanie Sumner](https://twitter.com/melaniersumner)

> Be magnanimous.

- [Video](https://youtu.be/qfnkDyHVJzs?t=8286)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- WAI-ARIA
- WCAG 2.0
- [Color-blind glasses](https://www.google.com/search?q=color+blind+glasses)
- https://include.ai
  - Add alt text to images on the web
- [ember-a11y](https://github.com/ember-a11y)
- Problems
  - Route transitions
  - Modal focus
  - `aria-*` support
  - Clicks
  - Passwords
- Easy wins
  - Use HTML5 elements
  - Link for routing, button for everything else
  - Keyboard nav, arrow keys
  - [Color contrast](https://a11ywins.tumblr.com/post/167324368213/google-chromes-color-contrast-debugger)
  - Image alt text
    - `<img src="elmo.png" alt="" role="presentation" />`
- [`ember-component-attributes`](https://github.com/mmun/ember-component-attributes)
- [\#topic-a11y](https://embercommunity.slack.com/messages/C06MC4CG6/)

#### Everything they didn't tell you about the Ember Community by [Jessica Jordan](https://twitter.com/jjordan_dev)

_Jessica provides an exhaustive overview of the Ember.js ecosystem and Emberista subculture._

- [Video](https://youtu.be/qfnkDyHVJzs?t=10835)
- [Slides](https://speakerdeck.com/jessicajordanjs/everything-they-didnt-tell-you-about-the-ember-community-jessica-jordan)
- Subculture
  - Emberistas, subset/subculture of JavaScript community
- [Growth in `@angular/cli` download counts](https://npm-stat.com/charts.html?package=%40angular%2Fcli&from=2017-03-01&to=2018-03-13)
- Top addons on [Ember Observer](https://emberobserver.com/lists/top-addons)
- [`ember-rickroll`](https://github.com/nucleartide/ember-rickroll) :troll:
- [Ember Request For Comments (RFC) process](https://github.com/ember-cli/rfcs)
- Quest issues concept
  - Example: [Ember Data](https://github.com/emberjs/data/issues/5292)
- [Ember.js status board](https://www.emberjs.com/statusboard/)
- [Adoption of RFC process by React](https://reactjs.org/blog/2017/12/07/introducing-the-react-rfc-process.html)
- [Ember.js Slack Community](https://embercommunity.slack.com)
  - [`#give-wrjblue-a-beer`](https://embercommunity.slack.com/messages/C05599BQX/)
- [Rapidly growing `ember-cli-typescript` adoption](https://github.com/typed-ember/ember-cli-typescript)
- Email newsletters
  - [Ember Weekly](http://www.emberweekly.com/)
  - [Ember.js Times](https://the-emberjs-times.ongoodbits.com/)
- Offline
  - EmberConf
  - EmberFest
  - EmberCamp
  - Meetups
- [Ember Women Helping Women program](http://emberwomen.com/)
- (not part of talk, related essay) [Melancholy of Subculture Society](https://www.gwern.net/The%20Melancholy%20of%20Subculture%20Society)

#### The Next Generation of Testing by [Tobias Bieniek](https://twitter.com/tobiasbieniek?lang=en)

_Tobias introduces new, elegant testing APIs in Ember._

- [Video](https://youtu.be/qfnkDyHVJzs?t=17882)
- [Slides](https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js)
- `.andThen()` vs `async`/`await`
- [`ember-native-dom-helpers`](https://github.com/cibernox/ember-native-dom-helpers)
- [`@ember/test-helpers`](https://github.com/emberjs/ember-test-helpers)
- [Grand Testing Unification RFC](https://github.com/rwjblue/rfcs/blob/42/text/0000-grand-testing-unification.md)
- Codemods
  - [`ember-native-dom-helpers-codemod`](https://github.com/simonihmig/ember-native-dom-helpers-codemod)
  - [`ember-qunit-codemod`](https://github.com/rwjblue/ember-qunit-codemod)
  - [`ember-test-helpers-codemod`](https://github.com/simonihmig/ember-test-helpers-codemod)
- Test loading states: `await waitFor('.loading-spinner');`
- [`ember-test-selectors`](https://github.com/simplabs/ember-test-selectors)
- DOM assertion library: [`qunit-dom`](https://github.com/simplabs/qunit-dom)

#### Say More by [Jamie White](https://twitter.com/jgwhite)

_Jamie examines test abstractions, and how one might hide details and edge cases behind a less powerful test language._

- [Video](https://youtu.be/qfnkDyHVJzs?t=20356)
- Slides - [https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js](https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js)
- Access via accessibility
- [Rule of Least Power](https://www.w3.org/2001/tag/doc/leastPower.html)
- [Babel plugin](https://babeljs.io/docs/plugins/) for generating `keyboardClick` test
- [`say-more`](https://github.com/jgwhite/say-more) app demonstrating concepts from talk

#### Who Moved My Cheese? Ember's New Filesystem Layout by [Matthew Beale](https://twitter.com/mixonic)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/qfnkDyHVJzs?t=22950)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [Ember.js Community Survey](https://emberjs.com/ember-community-survey-2018/)
- [Module Unification RFC](https://github.com/emberjs/rfcs/blob/master/text/0143-module-unification.md)
- Codemods
  - [ember-cli/ember-modules-codemod](https://github.com/ember-cli/ember-modules-codemod)
- [ember-optional-features](https://github.com/emberjs/ember-optional-features)
- Concepts
  - Colocation
  - Local lookup / isolation
  - Addon namespaces
    - `{{gadget-tools::list}}`
  - Compatibility between Module Unification layout and classic layout
- [schedule.emberconf.com](https://schedule.emberconf.com) module unification app
- [Quest issue, module unification: final cut](https://github.com/emberjs/ember.js/issues/16373)

#### Mastering the Art of Forms by [Danielle Adams](https://twitter.com/adamzdanielle)

_Danielle dives into component and data design for use in form UI and UX._

- [Video](https://youtu.be/qfnkDyHVJzs?t=26963)
- Slides - https://slides.com/danielleadams/art-of-forms-ec18
- Design questions
  - Field type
  - Required
  - Dependency between inputs
- Data-loading component using `willRender`
  - Retries with [`ember-concurrency`](https://github.com/machty/ember-concurrency)
- [`ember-cp-validations`](https://github.com/offirgolan/ember-cp-validations)
- Concerns
  - Built-in validation in HTML5 inputs
  - Tab navigation order that makes sense
- [Blue Apron](https://www.blueapron.com/) - form examples on the site

#### How To Build A Bonfire: On Training and Hiring New Devs by [Taylor Jones](https://twitter.com/hiimtaylorjones)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/qfnkDyHVJzs?t=29267)
- [Slides](https://www.slideshare.net/TaylorJones89/how-to-build-a-bonfire-on-hiring-and-training-ember-developers)
- [Mythical Man Month](https://en.wikipedia.org/wiki/The_Mythical_Man-Month)
  - Can't throw people at a problem... or can you :shipit:
- Help your team become _skilled_ at Ember
- "...context of a developer's past affects how they understand the future..."
  - Example: React vs. Angular background
- Have a style guide
  - Not just syntax, but how to do things

#### Living Animation by [Edward Faulkner](https://twitter.com/eaf4)

_mind blown_

- [Video](https://youtu.be/qfnkDyHVJzs?t=31861)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Animation approaches
  - Tweening
  - Procedural animation: rules and physics models in games
- [liquid-fire](https://github.com/ember-animation/liquid-fire)
  - Separation between app logic and animation
  - Establish rules (like in games) and let motions emerge
- [`ember-animated`](https://github.com/ember-animation/ember-animated), "Glimmer"-ization of `liquid-fire`
- [ef4/living-animation](https://github.com/ef4/living-animation)

## Day 2

### Talks

#### The Future of Data in Ember by [Dan Gebhardt](https://twitter.com/dgeb)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/bt9MRkf5Mus?t=1082)
- [Slides](https://speakerdeck.com/dgeb/the-future-of-data-in-ember)
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Smartphone Symphony by [Gavin Joyce](https://twitter.com/gavinjoyce)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/bt9MRkf5Mus?t=4601)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [ember-present](https://github.com/GavinJoyce/ember-present)

#### Reuse, Recycle: One Team's Journey From Projects to Products by [Sarah Bostwick](https://twitter.com/FajitaFresca)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/bt9MRkf5Mus?t=7327)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- http://www.animalancestry.com/
- [Write the Docs](http://www.writethedocs.org/)
- Sarah Mei's "refactor without permission" talk

#### Deep Dive on Ember Events by [Marie Chatfield](https://twitter.com/mariechatfield)

_Marie offers a lucid explanation of the subtle differences between DOM event and Ember event handling._

- [Video](https://youtu.be/bt9MRkf5Mus?t=14450)
- [Slides](https://drive.google.com/file/d/1tI4_GJesVIiH1QXsHtjyT6NAyt0kip47/view)
- Distinguish between DOM event listeners and Ember event listeners
  - DOM event listener (notice `on*` event syntax): `<div onclick={{action 'handleClick'}}>click me</div>`
  - Ember event listener: `<div {{action 'handleClick'}}>click me</div>`
    - Ember event listeners don't receive the native DOM event
- [Deep Dive on Ember Events blog post from Marie](https://medium.com/square-corner-blog/deep-dive-on-ember-events-cf684fd3b808)
- [`event_dispatcher.js`](https://github.com/emberjs/ember.js/blob/5a59eef5e6eb34001f8d002e1f8bc146d8d3f86f/packages/ember-views/lib/system/event_dispatcher.js#L205)
- Pick one and stick with it
- DOM event listeners fire before Ember event listeners

#### Building a Memex in Ember by [Andrew Louis](https://twitter.com/hyfen)

_Andrew demos his impressive life events database and graph query language and UI. Also his history of eclectic burrito consumption._

- [Video](https://youtu.be/bt9MRkf5Mus?t=17189)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [Vannevar Bush](https://en.wikipedia.org/wiki/Vannevar_Bush)
- [As We May Think essay](http://web.mit.edu/STS.035/www/PDFs/think.pdf)
- [Memex](https://en.wikipedia.org/wiki/Memex)
  - Human brain creates associations, memex creates associations mechanically
- "...brain gets the same stack that you had when you were solving this problem..."
- [Quantified Self](https://en.wikipedia.org/wiki/Quantified_self)
- [`ember-d3`](https://www.npmjs.com/package/ember-d3)
- [Mapbox GL JS](https://www.mapbox.com/mapbox-gl-js/api/)
- Addons used
  - ember-in-viewport
  - ember-electron
- Douglas Engelbert
- [@darkpatterns](https://twitter.com/darkpatterns) for inefficient time usage
- "Keep your side projects weird"
- https://hyfen.net/memex/

#### Brief interlude from sponsor LinkedIn

...

#### Prying Open the Black Box by [Godfrey Chan](https://twitter.com/chancancode)

_Godfrey explains debugging techniques by making analogies to the Hawaii missile false alarm and Columbia disaster. He also gives an overview of Chrome Devtools tricks for debugging Ember apps._

- [Video](https://youtu.be/bt9MRkf5Mus?t=19915)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Read stack traces from top to bottom
- Use debugger to freeze time, then go up and down stack
- [Blackboxing stack frames to hide frames you don't want](https://developer.chrome.com/devtools/docs/blackboxing)
- Chrome DevTools tricks
  - Conditional breakpoints in chrome devtools
  - Breakpoint on Ajax request
  - Right click & continue to here
  - `import { assert, debug } from '@ember/debug';`
  - "Continue to end" to escape breakpoints in for loop
  - [Ember Inspector](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi?hl=en)
  - Right click -> Show function definition
  - Break on DOM subtree modifications

#### Minitalk: Contributor Rally by [Sean Massa](https://twitter.com/endangeredmassa)

_Sean rallies the crowd and lists the various ways people contribute to the Ember.js community._

- [Video](https://youtu.be/bt9MRkf5Mus?t=6h35m46s)
- [Slides](https://docs.google.com/presentation/d/1Mwpp403LFUxM79eyXavI-Broh7tRWn_fbHxOdQYI0i4/edit?usp=sharing)
- [all-contributors](https://github.com/kentcdodds/all-contributors)
- [Let's All Build a Hat Rack](https://labhr.github.io/)
- [12 Reasons I Still Choose Ember.js by Ryan Tablada (rtablada)](https://www.youtube.com/watch?v=nOCMppWZ0Qs)

#### Minitalk: Toyota's Shared Component Library by [Tony Ward](https://twitter.com/_ynotdraw)

_Tony presents Toyota's shared component library, named "Loom"._

- [Video](https://youtu.be/bt9MRkf5Mus?t=24237)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [Toyota Production System](https://en.wikipedia.org/wiki/Toyota_Production_System)

#### Minitalk: Lightning Thoughts on Lightning Deploy by [Christina Kung](https://twitter.com/logtailer)

_Christine presents on how `ember-cli-deploy` helps with deployment on Conde Nast's built-in-Ember CMS "Copilot"._

- [Video](https://youtu.be/bt9MRkf5Mus?t=24595)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Addons
  - `ember-cli-deploy`
  - `ember-cli-deploy-lightning-pack`

#### Minitalk: Ember CLI Addon Docs by [Sam Selikoff](https://twitter.com/samselikoff)

_Sam Selikoff presents ember-cli-addon-docs, a standard documentation solution for Ember addons._

- [Video](https://youtu.be/bt9MRkf5Mus?t=24900)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Similar documentation sites
  - ember-cli-mirage (original)
  - ember-power-select
  - ember-cli-deploy
- Docs sites that are more animated
  - liquid-fire
  - ember-concurrency
- Examples of ember-cli-addon-docs sites
  - ember-data-storefront

#### Minitalk: Let Me Ember This for You by [Serena Fritsch](https://twitter.com/serifritsch)

_Serena presents on her experience rewriting the Ember.js deprecation page in Ember._

- [Video](https://youtu.be/bt9MRkf5Mus?t=25329)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [broccoli-static-site-json](https://github.com/stonecircle/broccoli-static-site-json)
- [ember-learn/deprecation-app](https://github.com/ember-learn/deprecation-app)

#### Creating Fluid App-Like Experiences With Ember by [Nick Schot](https://twitter.com/nickschot)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- [Video](https://youtu.be/bt9MRkf5Mus?t=7h14m50s)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Addons
  - [ember-mobile-core](https://github.com/nickschot/ember-mobile-core)
  - [ember-mobile-menu](https://github.com/nickschot/ember-mobile-menu)
  - [ember-mobile-bar](https://github.com/nickschot/ember-mobile-bar)
  - [ember-mobile-pane](https://github.com/nickschot/ember-mobile-pane)
- Mobile approaches
  - PWA
  - Corber/Cordova: hybrid approach, load Ember app into WebView
- [Demo app](https://github.com/nickschot/emberconf2018)

#### Shining a Light (closing keynote) by [Saron Yitbarek](https://twitter.com/saronyitbarek) and [Vaidehi Joshi](https://twitter.com/vaidehijoshi)

_Saron and Vaidehi discuss community building, and how to build inclusive commmunities (without the jerks). More pink, 3 exclamation points minimum!!!_

- [Video](https://youtu.be/bt9MRkf5Mus?t=8h3m35s)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Weekly #codenewbie Twitter chats
- [basecs Medium publication](https://medium.com/basecs)
- "No community is truly inclusive"
- [Codeland conference](http://codelandconf.com/)
- [Code Newbie podcast](https://www.codenewbie.org/podcast)
- [basecs podcast](https://www.codenewbie.org/basecs)
- [Lending Privilege talk by @anjuan at RubyConf](https://www.youtube.com/watch?v=zd4PsSk_0iQ)
  - [@anjuan](https://twitter.com/anjuan)
- "If I don't see them, ~they must not exist~"
