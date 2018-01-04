# react-time-limit

A React component to conditionally display elements based on date/time. Useful for displaying things like limited-time promotions so you don't have to redeploy or roll back your app on specific dates.

## Installation

With [Yarn](https://yarnpkg.com):

```bash
yarn add react-time-limit
```

With [npm](https://docs.npmjs.com/cli/npm):

```bash
npm install --save react-time-limit
```

## Usage

```jsx
import TimeLimit from 'react-time-limit'

...

<TimeLimit to='2018-01-20'>Show Before Target Date</TimeLimit>
<TimeLimit from='2018-01-20'>Show After Target Date</TimeLimit>
<TimeLimit from='2018-01-10' to='2018-01-15'>Show Between Two Target Dates</TimeLimit>
```

Dates can be supplied as any valid `new Date` value. ([Date docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date))