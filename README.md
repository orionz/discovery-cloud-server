### Discovery Cloud

This was made as a stop-gap replaceent for discovery swarm.

https://github.com/mafintosh/discovery-swarm

We were developing on a platform (Chrome App) that had some serious network
bugs and platform limitations and while waiting for the issues surriounding
discovery swarm to get fixed built this as a replacement.  This is the server
portion of the project that will allow peers to find each other via disvoery
keys and get piped websockets to each other created.

This app is intended to be deployable to heroku out of the box and require no
configuration.  By its design it should only ever run with a single dyno as
there's no backplane for processes to communicate with each other.

### Client code 

https://github.com/orionz/discovery-cloud-client

### Setup

The code should work as a heroku app out of the box with no extra setup.

```
  $ heroku create
  Creating app... done, ⬢ fish-monger-9999
  https://fish-monger-9999.herokuapp.com/ | https://git.heroku.com/fish-monger-9999.git
  $ git push heroku master
```

### LICENSE 

MIT

