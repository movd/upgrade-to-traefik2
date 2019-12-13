# Upgrade from Traefik 1.7 to 2.x

This fall *containous* the company behind Traefik [released version 2.0](https://blog.containo.us/traefik-2-0-6531ec5196c2). This is a major release including cool stuff like reusable [middlewares](https://docs.traefik.io/middlewares/overview/), a new fun web dashboard and advanced stuff for production deployments like canary deployments. This changes come with a trade off. The new version has lots of breaking changes because of that I had to update my deployment and understand the new paradigms introduced. In my blog post over at [moritzvd.com](https://moritzvd.com) I want to help share my findings and show a path to upgrade from 1.7 to 2.1.

You can read my guide at <https://moritzvd.com/upgrade-traefik-2/>

## Generate acme.json

```sh
$ touch acme.json
$ chmod 600 acme.json
```