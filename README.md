<style>
  body {
    background: black;
    color: black;
    font-size: 14px;
    font-family: Arial, Helvetica, sans-serif;
  }

  .container-lg {
    max-width: 1012px;
    margin-right: auto;
    margin-left: auto;
    margin-top: 0 !important;
  }

  .container-lg h1 {
    display: none;
  }

  .mobile-demo {
    margin: 1.5rem 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-between;
    text-align: center;
    color: white;
  }

  .mobile-demo .title {
    font-size: 1.5rem;
    margin-bottom: 10px;
    width: 100%;
    color:gray;
  }

  .web-demo {
    /* transform: scale(0.95); */
    transform-origin: top center;
    text-align: center;
  }

  .web-header {
    border-right: 1px solid #545456;
    border-top: 1px solid #545456;
    border-left: 1px solid #545456;
    /* box-shadow: rgb(235, 235, 235) 0px 2px 4px; */
  }

  .web-demo .title {
    font-size: 1.3rem !important;
    clear: both;
    margin-top: 1rem;
  }

  .web-wrapper {
    margin: 0 auto;
    border: 1px solid #575757;
    border-radius: 30px;
    padding: 25px 15px
  }

  .web-wrapper iframe {
    width: 320px;
    height: 67%;
    border: 0;
  }

  .web-header {
    background: -webkit-linear-gradient(rgba(55, 55, 55, .98), #545456);
    background: linear-gradient(rgba(55, 55, 55, .98), #545456);
    text-align: center;
  }

  .web-statbar {
    height: 20px;
    margin-bottom: 4px;
  }

  .web-statbar img {
    border-style: none;
    margin: 7px 2px;
    background-color: transparent;
    width: 300px;
  }

  .url-box {
    width: 300px;
    height: 28px;
    line-height: 28px;
    color: #fff;
    background-color: #a2a2a2;
    margin: 0 auto;
    border-radius: 4px;
    white-space: nowrap;
    overflow-x: scroll;
    text-align: left;
    font-size: 14px;
  }

  .url-box span {
    padding: 0 10px;
  }

  .browserstack {
    font-family: Arial;
    text-decoration: none;
  }

  .browserstack img {
    background: #ececec;
    position: relative;
    top: 7px;
    width: 25px;
  }

  .appetize {
    font-family: Arial;
    text-decoration: none;
  }

  .appetize img {
    background: #ececec;
    position: relative;
    top: 7px;
    width: 25px;
  }
</style>

<div>
  <div class="mobile-demo">
    <!-- WEB demo -->
    <div class="web-demo">
      <div class="title">Mobile WEB</div>
      <div class="web-wrapper">
        <div class="web-header">
          <div class="web-statbar">
            <img width="250" alt="presentation" src="https://os.alipayobjects.com/rmsportal/VfVHYcSUxreetec.png" />
          </div>
          <div style="height: 40px">
            <div class="url-box"><span>https://shop.serga.name/</span></div>
          </div>
        </div>
        <section>
          <iframe src="https://shop.serga.name">
            Iframe isn't supported
          </iframe>
        </section>
      </div>
    </div>
    <div>
      <!-- About -->
      <div style="height: 100px; margin: 0.5rem 0; color: white">
        <div style="font-size: 2.9rem; text-shadow: 1px 1px 1px gray; font-family: monospace">React Cross-Platform</div>
        <div style="font-size: 1.2rem; color: gray">1 project with shared JS code + single GraphQL API = 3 platforms</div>
      </div>
      <div style="display: flex; justify-content: space-evenly; width: 800">
        <!-- Adnroid demo -->
        <div>
          <div class="title">Android</div>
          <iframe src="https://appetize.io/embed/edrtcxb7wqu1cgny78wu9av4dc?device=nexus5&scale=60&autoplay=false&orientation=portrait&deviceColor=black&language=en"
            width="240px" height="477px" frameborder="0" scrolling="no">
            Iframe isn't supported
          </iframe>
        </div>
        <!-- iOS demo -->
        <div>
            <div class="title">iOS</div>
            <iframe src="https://appetize.io/embed/c0au0jv9uhgut98zqm9t8zhn40?device=iphone5s&scale=61&autoplay=false&orientation=portrait&deviceColor=white&language=en"
              width="240px" height="477px" frameborder="0" scrolling="no">Iframe isn't supported</iframe>
          </div>
      </div>
    </div>
  </div>
</div>

<iframe src="https://shop.serga.name/graphiql?query=query%20%7B%0A%20%20categories%20%7B%0A%20%20%20%20id%0A%20%20%20%20alias%0A%20%20%7D%0A%7D%0A&variables=%7B%7D" width="100%" height="400">
  Iframe isn't supported
</iframe>

## How React solves Cross-Platform?

* WEB — [React](https://facebook.github.io/react/)
* Mobile apps — React + [React Native](https://facebook.github.io/react-native/)
* Desktop apps — React + [Electron](https://electron.atom.io/)

you can even reuse platform's common JS code in single monorepo using

* ready solutions like [ReactXP](https://microsoft.github.io/reactxp/) ([Skype story](https://microsoft.github.io/reactxp/blog/2017/04/06/introducing-reactxp.html))
* or find your own solution using [Lerna](https://lernajs.io/)

Smells like future front-end!
<iframe width="560" height="315" src="https://www.youtube.com/embed/-5VkI0dpHek" frameborder="0" allowfullscreen></iframe>

`Note: if you write games - it's not your story, sorry`

## Why React? Mature matters!

Is React mature enough for WEB? Yes, the most.

Is Electron mature enough for Desktop? If you like VSCode, Atom, Slack or some of [385 apps](https://electron.atom.io/apps/) and believe in GitHub - Yes.

Is React Native mature enough for Mobile? Instagram, Skype, Airbnb, Walmart and [other](https://facebook.github.io/react-native/showcase.html) already use it and you can read how they did it. And if you believe in Facebook - I believe Yes.

## What is the Tech Stack in this demo?

* Front-End - react, react-native, redux, apollo-client, ant-design-mobile. Written using TypeScript.
* Back-End - django, graphene, postgresql. Written using Python.

## Ready to fork?

* Mobile WEB - [https://github.com/react-cross-platform/react-shop](https://github.com/react-cross-platform/react-shop)
* iOS and Android - [https://github.com/react-cross-platform/react-native-shop](https://github.com/react-cross-platform/react-native-shop)
* Cross-platform monorepo with shared JS code - sure some sunny day!

## Sponsorship

<div style="margin-bottom: 2rem">
  <div>
    <a class="browserstack" href="https://www.browserstack.com/">
      <img src="./browserstack-logo.png"/>
      BrowserStack
    </a> - live, web-based browser testing
  </div>
  <div>
    <a class="appetize" href="https://appetize.io/">
      <img src="./appetize-logo.png"/>
      Appetize
    </a> - run native mobile apps in your browser
  </div>
</div>

> To Be Continued...