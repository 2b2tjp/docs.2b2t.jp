# Installing MetricPoster Plugin

## Requirements
- Spigot or Paper server (Either NMS or `Bukkit#getTPS()` is required.)
- Selfhosted status page (See: [Selfhosting the status page](/self-hosting/selfhosting-the-status-page))

See: https://github.com/acrylic-style/MetricPosterPlugin

Installing Metric Poster Plugin is simple, all you need is to just install the plugin and edit config.yml a bit.

Download the plugin from [here](https://github.com/acrylic-style/MetricPosterPlugin/releases/download/v1.0/MetricPoster.jar), then put the plugin into your `plugins` folder. (Can be put into both main and queue server)

Now you need to configure the plugin.

First, create the **folder** named `MetricPoster` **inside** your `plugins` folder.

Create the config.yml inside the created `MetricPoster` folder, with those contents:
```yaml
queueServer: false # turn it on only if the plugin is in queue server, don't use this if you have 2+ queue servers.
authorization: # set same value as AUTHORIZATION in https://github.com/acrylic-style/status.2b2t.jp/blob/master/.env.example
endPoint: # example: https://status.2b2t.jp/api/data.json
```

For example, if you have `AUTHORIZATION=abcdef` defined in .env from acrylic-style/status.2b2t.jp, and the end point is `https://status.example.com/api/data.json`, the config.yml will look like this:
```yaml
authorization: abcdef
endPoint: "https://status.example.com/api/data.json"
```

The end point must return valid json and must be accessible from User-Agent `Java/your_jvm_version`
