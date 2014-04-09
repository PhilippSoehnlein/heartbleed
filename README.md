# Heartbleed

List of sites that have fixed there infrastructure against heartbleed.

The idea of this repository came from two tweets from [janl](https://twitter.com/janl/status/453874289528549376) and [rem](https://twitter.com/rem/status/453874447305687040).
We should have some central place where site owner can "notify" everyone that they hardend their infrastructure aginst [The Heartbleed Bug](http://heartbleed.com).

## Contribute
You can contribute your site to this repository via pull requests. To get the name of the file use the following rules:

- reverse the domain name
- create a directory for each part (if it does not exist already) **except for the last part)
- add a filename of the last part you just omitted and add the `.json` extension

If guides.github.com wanted contribute their update, they would create a file with the name `guides.json` inside the directory path `com/github`.

The content is a plain JSON object and can contain the following keys:

- **`domain`** - The name of the domain in a human readable form
- **`time`** – The time after which communications are assumed to be save again (if unknown use `null`)
- **`includeSubdomain`** - If also all subdomains have been secured (`true` or `false`)
- **`source`** - Where this information comes from (e.g. a blogpost)

An example for guides.github.com would look like this:

```
{
    "domain": "guides.github.com",
    "time": null,
    "includeSubdomain": false,
    "source": "https:\/\/github.com\/blog\/1818-security-heartbleed-vulnerability"
}
```

## Feedback
If you want to provide feedback to this repository: please just create an [new issue](https://github.com/tobiastom/heartbleed/issues/new).