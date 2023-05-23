# CodiMD for railway.app

Deploy CodiMD on railway

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/YcOXBV?referralCode=2_sIT9)
## ✨ Features

* CodiMD with automated setup
* CodiMD settings as environment variables

## 🐍 How to Deploy

1. Click Deploy on Railway and setup your credentials in the environment variables

```json
 {
        "NPM_CONFIG_PRODUCTION": {
            "description": "Let npm also install development build tool",
            "value": "false"
        },
        "CMD_SESSION_SECRET": {
            "description": "Secret used to secure session cookies.",
            "required": false
        },
        "CMD_HSTS_ENABLE": {
            "description": "whether to also use HSTS if HTTPS is enabled",
            "required": false
        },
        "CMD_HSTS_MAX_AGE": {
            "description": "max duration, in seconds, to tell clients to keep HSTS status",
            "required": false
        },
        "CMD_HSTS_INCLUDE_SUBDOMAINS": {
            "description": "whether to tell clients to also regard subdomains as HSTS hosts",
            "required": false
        },
        "CMD_HSTS_PRELOAD": {
            "description": "whether to allow at all adding of the site to HSTS preloads (e.g. in browsers)",
            "required": false
        },
        "CMD_DOMAIN": {
            "description": "domain name",
            "required": false
        },
        "CMD_URL_PATH": {
            "description": "sub url path, like `www.example.com/<URL_PATH>`",
            "required": false
        },
        "CMD_ALLOW_ORIGIN": {
            "description": "domain name whitelist (use comma to separate)",
            "required": false,
            "value": "localhost"
        },
        "CMD_PROTOCOL_USESSL": {
            "description": "set to use ssl protocol for resources path (only applied when domain is set)",
            "required": false
        },
        "CMD_URL_ADDPORT": {
            "description": "set to add port on callback url (port 80 or 443 won't applied) (only applied when domain is set)",
            "required": false
        },
        "CMD_FACEBOOK_CLIENTID": {
            "description": "Facebook API client id",
            "required": false
        },
        "CMD_FACEBOOK_CLIENTSECRET": {
            "description": "Facebook API client secret",
            "required": false
        },
        "CMD_TWITTER_CONSUMERKEY": {
            "description": "Twitter API consumer key",
            "required": false
        },
        "CMD_TWITTER_CONSUMERSECRET": {
            "description": "Twitter API consumer secret",
            "required": false
        },
        "CMD_GITHUB_CLIENTID": {
            "description": "GitHub API client id",
            "required": false
        },
        "CMD_GITHUB_CLIENTSECRET": {
            "description": "GitHub API client secret",
            "required": false
        },
        "CMD_BITBUCKET_CLIENTID": {
            "description": "Bitbucket API client id",
            "required": false
        },
        "CMD_BITBUCKET_CLIENTSECRET": {
            "description": "Bitbucket API client secret",
            "required": false
        },
        "CMD_GITLAB_BASEURL": {
            "description": "GitLab authentication endpoint, set to use other endpoint than GitLab.com (optional)",
            "required": false
        },
        "CMD_GITLAB_CLIENTID": {
            "description": "GitLab API client id",
            "required": false
        },
        "CMD_GITLAB_CLIENTSECRET": {
            "description": "GitLab API client secret",
            "required": false
        },
        "CMD_GITLAB_SCOPE": {
            "description": "GitLab API client scope (optional)",
            "required": false
        },
        "CMD_MATTERMOST_BASEURL": {
            "description": "Mattermost authentication endpoint",
            "required": false
        },
        "CMD_MATTERMOST_CLIENTID": {
            "description": "Mattermost API client id",
            "required": false
        },
        "CMD_MATTERMOST_CLIENTSECRET": {
            "description": "Mattermost API client secret",
            "required": false
        },
        "CMD_DROPBOX_CLIENTID": {
            "description": "Dropbox API client id",
            "required": false
        },
        "CMD_DROPBOX_CLIENTSECRET": {
            "description": "Dropbox API client secret",
            "required": false
        },
        "CMD_DROPBOX_APP_KEY": {
            "description": "Dropbox app key (for import/export)",
            "required": false
        },
        "CMD_GOOGLE_CLIENTID": {
            "description": "Google API client id",
            "required": false
        },
        "CMD_GOOGLE_CLIENTSECRET": {
            "description": "Google API client secret",
            "required": false
        },
        "CMD_IMGUR_CLIENTID": {
            "description": "Imgur API client id",
            "required": false
        },
        "CMD_ALLOW_PDF_EXPORT": {
            "description": "Enable or disable PDF exports",
            "required": false
        },
        "PGSSLMODE": {
          "description": "Enforce PG SSL mode",
          "value": "require"
        }
 }
 ```

```bash
CMD_USECDN=false
CMD_DOMAIN=${{RAILWAY_STATIC_URL}}
CMD_URL_ADDPORT=false
CMD_PROTOCOL_USESSL=true
```

### Essentials

 ```bash
PORT=3000 # Don't change this
```

2. Wait for Build & Deployment to Finish
3. Open the custom URL an enter your credentials

## 👩‍💻 How to Use

1. Setup your credentials in the environment variables

## 🪲 Bug Reporting

If you find a bug in the template for railway, you can [submit an issue](https://github.com/vergissberlin/railwayapp-codimd/issues/new) to the GitHub Repository. Even better you can submit a Pull Request with a fix.

## 🐳  Local Development

```bash
docker compose up -d
```

Connect to http://localhost:3000 use setup username & password from docker-compose file to login to codimd.
