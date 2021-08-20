# XState Redux

Incrementally adopt XState in your redux app with some simple middleware.

## Getting Started

1. See [`lib/counterSlice.ts`](./lib/counterSlice.ts) to see how to create an 'XState' slice
2. See [`lib/store.ts`](./lib/store.ts) to see how to configure your Redux store to use XState.
3. Try creating your own slice! You can use any XState feature.

## Features

**Use statecharts as reducers**: Call `createMachine`, then pass it into `createXStateSlice`, and you're good to go. You can use 100% of XState's features right alongside Redux.

**Use sendParent to send events to Redux**: The Redux store is your machine's 'parent', meaning you can call `sendParent` to send actions to Redux.

**Colocate side effects with your Redux logic**: No more splitting out side effects from your app logic. Use `invoke`, `actions` and even spawn actors in your XState machines.
