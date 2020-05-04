# Next.js + React Profiler

![npm badge](https://img.shields.io/npm/v/next-plugin-profiler)

Enable the [React Profiler](https://reactjs.org/blog/2018/09/10/introducing-the-react-profiler.html) during a production build in your [Next.js](https://nextjs.org/) project

## Installation

```bash
npm install --save next-plugin-profiler
```

or

```bash
yarn add next-plugin-profiler
```

### Usage with environment variables

Create a `next.config.js` file:

```js
// next.config.js
const withProfiler = require(`next-plugin-profiler`)({
  isEnabled: process.env.ENABLE_PROFILER === `true`
});

module.exports = withProfiler({});
```

Then you can run a build command with the environment variable:

```bash
ENABLE_PROFILER=true npm run build
```
