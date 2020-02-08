# Next.js + React Profiler

Enable the [React Profiler](https://reactjs.org/blog/2018/09/10/introducing-the-react-profiler.html) during a production build in your [Next.js](https://nextjs.org/) project

## Installation

```bash
npm install --save next-plugin-react-profiler
```

or

```bash
yarn add next-plugin-react-profiler
```

### Usage with environment variables

Create a next.config.js:

```js
// next.config.js
const withReactProfiler = require(`next-plugin-react-profiler`)({
  isEnabled: process.env.ENABLE_REACT_PROFILER === `true`
});

module.exports = withReactProfiler({});
```

Then you can run a build command with environment variable and the condition you've set:

```bash
ENABLE_REACT_PROFILER=true npm run build
```
