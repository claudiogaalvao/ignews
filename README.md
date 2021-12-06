# Ignews
That's a project of content subscription about React News, that I started with the objective to apply NextJs concepts. In that project I worked with Sass, CSS Modules, TypeScript, FaunaDB, Authentication with Next Auth and explore concepts like CSR (Client-side Rendering), SSR (Server-side Rendering) and SSG (Static Site Generation). There's a possibility to subscribe to access the articles, so I integrated with an external payment API (Stripe).

# What is NextJs (Simple description)
NextJs is a framework for ReactJs. The NextJs work with SSR concept that add more performance to our application and indexing of page content by search engines.

# How to run the project
- First, garantee that you have installed NodeJs and npm on your machine. 

  - You can check with this command ``` npx --version ```

    <img src="https://treehouse.github.io/installation-guides/mac/imgs/node-install1.png" style="width: 100%; height: auto;" />

  - You can download the last release in this link https://nodejs.org/pt-br/download/. The installer of NodeJs include npm.
  
- The second step is download the dependencies. To do that, open the project in some terminal on the root path, and execute ``` npm install ```

- After finish the dependencies download, execute ``` npm run dev ```, then you should be able to identify the link to open on your browser, like that:

  <img src="https://github.com/claudiogaalvao/ignews/raw/master/public/images/Screenshot_1.png" style="width: 100%; height: auto;" />

- To local test features like subscription canceled and subcription saving on database, it's necessary listen the stripe events. To listen that, download Stripe CLI (https://stripe.com/docs/stripe-cli). For Windows, unzip the file and open the file on cmd. Run the command ``` stripe login ```. After that, to let listening locally, execute the command ``` stripe listen --forward-to localhost:3000/api/webhooks ```

# Future features plan
- List posts
- Connect Front-end to a CMS to manage posts
