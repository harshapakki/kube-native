# kube-native

A small Vue.js events bulletin board used as a target for containerising and
deploying a Node application, rather than as a front end exercise.

The application code comes from a public Vue.js tutorial. What is mine here is
the packaging: the `Dockerfile` and the work of getting an Express server and a
built front end to run the same way on a laptop and in a cluster.

## What is here

- `server.js` is the Express host for the API and the built assets
- `src/` is the Vue application, with `src/backend/` holding the API and the
  event store
- `Dockerfile` builds the runnable image

## Running it

```
npm install
node server.js
```

Or build the image and run that instead, which is the point of the repo.

## Credit

The bulletin board application follows the Scotch.io Vue.js time tracking
tutorial. The container and deployment work is mine.
