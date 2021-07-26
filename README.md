# microfrontend-react-vue

A microfrontend application using react and vue. This application is for an imaginary SAAS product where the features are divided into three micro frontend applications.

| Apps      |                                                    |
| --------- | -------------------------------------------------- |
| Marketing | Contains information about the SAAS product        |
| Auth      | Basic signin/signup flow                           |
| Dashboard | A staic dashboard for authenticated users          |
| Container | Works as container for above three microfrontend's |

## Features

- Loosely coupled code for each microfrontend
- Framework agnostic, I have used react/vue but can be used with any FE framework or even vanilla JS.
- Each microfrontend can be used as a standalone app
- Each microfrontend can handle routing as it's own or can pass this responsibility to the container application.

## Tech

- React / vue
- react-router-dom
- Webpack with Module Federation Plugin
- material-ui for some quick staic markup

## Installation

```sh
cd packages/marketing
npm install
npm start

cd packages/auth
npm install
npm start

cd packages/dashboard
npm install
npm start

cd packages/container
npm install
npm start
```

Marketing app will run at http://localhost:8081
Auth app will run at http://localhost:8082
Dashboard app will run at http://localhost:8083
Container app will run at http://localhost:8080
