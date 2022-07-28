# pin-hugo

Experimenting with Hugo on [Cloudflare Pages](https://pages.cloudflare.com). 

## Prerequisites
- hugo, available via `brew install hugo` 
- Clouflare Pages account, for publishing

## Installation

1. Clone the repo
2. cd to/the/folder/
3. `hugo server`

## Notes
This is a pretty vanilla instance of a Hugo site. 

It follows the instructions laid out on the Cloudflare Pages docs, [Deploy a Hugo Site](https://developers.cloudflare.com/pages/framework-guides/deploy-a-hugo-site/).

### Known Issue, HUGO_VERSION
As of Jul 28 2022, `ERROR` is generated on build due to incompatible version of Hugo. 

```
ERROR 2022/07/28 18:51:26 TERMINAL theme does not support Hugo version 0.54.0. Minimum version required is 0.74
```

To fix, go to the Project > Settings > Environment Variables > Production and specify the variable `HUGO_VERSION` to 0.80.0

h/t https://sysrant.com/posts/setting-up-a-hugo-website-with-cloudflare-pages/
