# 🔗 URL Shortener Database

This is a minimal URL shortener database that can be entirely hosted on GitHub pages. All link issues are kept here.

## Usage

Note: Non authenticated submissions are turned off and will not work.

To add a new link:

- Open an issue with the title being the link you want to shorten, including the `http(s)://` to [/sdb/issues](https://github.com/fluteds/sdb/issues).

## Terms

While the repo will currently only work with URLs submitted by myself, the usage terms still apply if you attempt to submit a link.

If you to submit a link you agree to the following:

- Your URL will be publically available and cannot be deleted unless the repo is deleted.
- GitHub has a rate limit of 60 searches without auth which affects how many times you can use the service. Check your rate limit by using CURL. `curl -I https://api.github.com/user`
- Links that go against [GitHub's TOS](https://docs.github.com/en/github/site-policy/github-community-guidelines) are not allowed.

## ShareX Config

This URL shortener can also be used with [ShareX.](https://getsharex.com/)

```json
{
  "Version": "13.3.0",
  "Name": "GitHub Short URL",
  "DestinationType": "URLShortener",
  "RequestMethod": "POST",
  "RequestURL": "https://api.github.com/repos/{repo}/issues",
  "Headers": {
    "Authorization": "token {github token}",
    "Accept": "application/vnd.github.v3+json"
  },
  "Body": "JSON",
  "Data": "{\"title\":\"$input$\",\"body\":\"$prompt:Alias?$\"}",
  "URL": "{URL of shortener}/$json:number$"
}
```

To add the config to ShareX:

- [Visit this gist](https://gist.github.com/jacobmacweb/44b59ed363fee1b1a1e4fb74946f023e)
- Follow the Gist's instructions
