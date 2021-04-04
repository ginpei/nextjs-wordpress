# Next.js + WordPress

- [next.js/README.md at canary · vercel/next.js](https://github.com/vercel/next.js/blob/canary/examples/cms-wordpress/README.md)

## Set up

You need Node.js and Docker.

### WordPress

```console
$ docker-compose up
```

Set up WordPress with default values but specify `db` to database name.

Log in to the WordPress site and go to Plugins > Add New > search by "WP GraphQL":

- http://localhost:8080/wp-admin/plugin-install.php?s=WP+GraphQL&tab=search&type=term

Then install and activate it.

### Next.js

```console
$ cd nextjs
$ npm ci
```

## Start

```console
$ cd wordpress
$ docker-compose up
```

Then

```console
$ cd nextjs
$ npm run dev
```

### Stop

Press `Ctrl+C`.
