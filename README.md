# Discovery Cloud Server

This was made as a stop-gap replacement for [discovery-swarm](https://github.com/mafintosh/discovery-swarm).

We were developing on a platform (Chrome App) that had some serious network
bugs and platform limitations and while waiting for the issues surrounding
discovery swarm to get fixed built this as a replacement.

This is the server portion of the project. It allows peers to find each
other via discovery keys and get piped websockets to each other created.

For usage, see the client portion at [discovery-cloud-client](https://github.com/orionz/discovery-cloud-client).

## Setup

### Heroku

This app is intended to be deployable to heroku out of the box and require no
configuration. By its design it should only ever run with a single dyno as
there's no backplane for processes to communicate with each other.

```
  $ heroku create
  Creating app... done, ⬢ fish-monger-9999
  https://fish-monger-9999.herokuapp.com/ | https://git.heroku.com/fish-monger-9999.git
  $ git push heroku master
```

### Glitch

This server can run on [Glitch](https://glitch.com); just remix the [**discovery-cloud**](https://glitch.com/edit/#!/remix/discovery-cloud) project.

## LICENSE

MIT
