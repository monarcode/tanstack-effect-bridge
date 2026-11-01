# tanstack-effect-bridge

**Use [Effect](https://effect.website) with [TanStack Query](https://tanstack.com/query), without writing the glue yourself.**

> 🚧 **Coming soon.** This project is in the works. Star or watch the repo
> to hear when the first release lands.

## What it's for

TanStack Query is the industry standard for data fetching. Effect is a great
way to write the code behind it, with typed errors, services and retries.
Using the two together usually means a hand-written bridge: run each Effect
into a promise, hand the promise to TanStack Query, and turn its errors back
into something your UI can match on.

tanstack-effect-bridge will be that bridge, done once and done well. Keep
TanStack Query, its devtools and its ecosystem, and write your queries and
mutations as Effects.

## What's planned

- **Effects as queries and mutations:** `queryFn` and `mutationFn` from an
  Effect, run with your app's layer or `ManagedRuntime`.
- **Typed errors** that reach your components as Effect errors, not `unknown`.
- **Cancellation:** TanStack Query's abort signal interrupts the Effect.
- **Works with [effetch](https://github.com/monarcode/effetch):** turn its
  endpoints straight into query options.

## Want it Effect-native all the way?

If you're ready to move your server state into Effect itself, see
[effetch-query](https://github.com/monarcode/effetch-query): TanStack-Query-style
caching built on Effect.

## License

[MIT](LICENSE)
