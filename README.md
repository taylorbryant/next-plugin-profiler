# Next.js + React Profiler

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

Create a next.config.js:

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
