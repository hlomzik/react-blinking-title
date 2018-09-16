# React Blinking Title

Simple component to draw user's attention with the blinking page title.
There are no start/stop triggers, just mount it by condition and provide it
with your `title` and optional blinking `interval`. Component will carefully
store your current title and restore it after every blink, even if you
change it during this short time.

## Installation

```sh
npm install --save git+https://git@github.com/hlomzik/react-blinking-title.git
```

React 15+, ES6+ with [class fields](https://github.com/tc39/proposal-class-fields)

## Example

```jsx
/* somewhere in the App component */
{newMessages.count > 0 && (
  <BlinkingTitle title={`${newMessages.count} new messages`} interval={300} />
)}
```

