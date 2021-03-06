# 🔗 URL Shortener Database

**Hosted by Github Pages**

This is a minimal URL shortener database that can be entirely hosted on GitHub pages. All link issues are kept here.

## Usage

To add a new link:

- Open an issue with the title being the link you want to shorten, including the `http(s)://` to [/sdb/issues](https://github.com/fluteds/sdb/issues).
- There is no need to put the pound symbol as the URLs look like this: `website.xyz/s/1` instead of this: `website.xyz/s/#1`.

## Terms

By submitting a link you agree to the following:

- Your URL will be publically available and cannot be deleted unless the repo is deleted.
- GitHub has a rate limit of 60 searches without auth which affects how many times you can use the service. Check your rate limit by using CURL. `curl -I https://api.github.com/user`
- Links that go against [GitHub's TOS](https://docs.github.com/en/github/site-policy/github-community-guidelines) are not allowed.

## ShareX Config

This URL shortener can also be used with [ShareX.](https://getsharex.com/)

To add the config to ShareX:

- [Visit this gist](https://gist.github.com/avedromeda/44b59ed363fee1b1a1e4fb74946f023e)
- Follow the Gist's instructions

The ShareX config was created by [avedromeda](https://github.com/avedromeda)
