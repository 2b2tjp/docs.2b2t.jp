# Selfhosting the status page

## Requirements
- [Node.js](https://nodejs.org/)

## Optional
- Apache2, nginx, or similar things for reverse proxy if you want
- [yarn](https://yarnpkg.com/) (optional, but recommended. you can install via `npm i -g yarn`)

## Run status page

First, clone or download [this repository](https://github.com/acrylic-style/status.2b2t.jp). ([Download ZIP](https://github.com/acrylic-style/status.2b2t.jp/archive/master.zip))

Now, your repository folder should look like this:

![](/assets/ls.png)

Copy `.env.example` to `.env`, and set `AUTHORIZATION` to some random long string.

Set `PORT` to valid tcp port you want to use. The web server will be accessible from that port.

If you don't know what is `TEBEX_SECRET`, put some random string and save it.

!> **Never** share your `.env` file!

Run one of those commands:
- `npm install`
- `yarn` (if you have yarn installed)

![](/assets/yarn.png)

And finally, run the application with `node index.js`.

?> You can daemonize your application with [pm2](https://www.npmjs.com/package/pm2)

Your screen should be similar to this:

![](/assets/running_app.png)

Now you can visit the website with your browser!

![](/assets/page.png)

To make show the data, you have to put data.

The easiest way to put the data is to use the plugin.

See: [Installing Metric Poster Plugin](/self-hosting/installing-metric-poster-plugin)

