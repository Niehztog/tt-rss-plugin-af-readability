# Fork of af-readability plugin for tt-rss

While the original plugin relies on the [Fivefilters Readability.php library](https://github.com/fivefilters/readability.php), this fork uses [Graby](https://github.com/j0k3r/graby) for fetching full article contents. [Graby](https://github.com/j0k3r/graby) is based on [full-text-rss by fivefilters](https://bitbucket.org/fivefilters/full-text-rss). This leads to a lot better results, as `full-text-rss` comes with a large collection of site specific extraction rules and processes Open Graph HTML tags of articles to extract article images.

## Adding site-specific configs

Graby uses [full-text-rss site patterns](https://help.fivefilters.org/full-text-rss/site-patterns.html) to extract content for specific sites. If a site is not supported or produces poor results, you can add a custom config file to `vendor/j0k3r/graby-site-config/` following the format described in the link above. To share your config with the community, submit a pull request to the [ftr-site-config repository](https://github.com/fivefilters/ftr-site-config).
