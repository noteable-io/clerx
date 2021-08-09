# clerx 💁

RxJS Operators and Observables for the administrative busybodies inside us.

## Operators

### `rateLimiter`

Defer sending events if `count` events occur within `slidingWindowTime`. Optionally,
stop deferring if the wait time goes past `timeoutDue`.

## Observables

### `postDelay`

Creates an observable that emits the `event` then waits `dueTime` before
closing the observable, like so:

```
event--{ dueTime }--|
```