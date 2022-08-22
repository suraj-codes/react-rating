# React Ratings

React Ratings is a [React](https://github.com/facebook/react) rating component built with [StyledComponents](https://github.com/styled-components/styled-components) 💅

## Installation

You can install `rc-ratings` component using the **yarn** or **npm** package manager:

```bash
yarn add rc-ratings
npm install rc-ratings
```

### Dependencies

The `rc-ratings` component [peer depends](https://docs.npmjs.com/files/package.json#peerdependencies) on the [React](http://facebook.github.io/react/) library.

You can install React using _yarn_:

```bash
yarn add --save react react-dom
```

## Usage

Import Rating Component

```javascript
import Rating from "rc-ratings";
```

Start using it:

```jsx
<Rating />
```

Pass some config props:

```jsx
<Rating animateOnHover disableAnimation initialRate={3} stop={10} />
```

## Properties

| Property           | Type            | Default    | Description                                          |
| ------------------ | --------------- | ---------- | ---------------------------------------------------- |
| `animateOnHover`   | _Boolean_       | false      | Whether to animate rate hovering or not.             |
| `disableAnimation` | _Boolean_       | false      | Disable stars animation onClick or onHover.          |
| `emptyRate`        | _React Element_ | Empty Star | React Element                                        |
| `fractions`        | _Number_        | 1          | Number of equal parts that make up a whole symbol.   |
| `fullRate`         | _React Element_ | Full Star  | React element                                        |
| `initialRate`      | _Number_        | 0          | Initial rate value.                                  |
| `readonly`         | _Boolean_       | false      | Whether the rating can be modified or not.           |
| `start`            | _Number_        | 0          | Range starting value.                                |
| `step`             | _Number_        | 1          | Step increment (must be between _start_ and _stop_). |
| `stop`             | _Number_        | 5          | Range stop value.                                    |

## Callbacks

| Callback   | Type       | Parameters                       | Description                                                                               |
| ---------- | ---------- | -------------------------------- | ----------------------------------------------------------------------------------------- |
| `onChange` | _Function_ | rate: _Number_                   | Called when the selected rate is changed.                                                 |
| `onClick`  | _Function_ | (rate: _Number_, event: _Event_) | Called when a rate is clicked.                                                            |
| `onRate`   | _Function_ | rate: _Number_ or _undefined_    | Called when a rate is entered or left. When a rate is left it is called with `undefined`. |

## License

[MIT License](https://github.com/surajcodes/react-rating/blob/master/LICENSE.md)
