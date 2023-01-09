# Steps to reproduce

1. Disable traefik in ddev
2. Check out the repo and run `ddev start`
3. `http http://reproduce-traefik-virtualhost.ddev.site` will show you "hello world from php"
4. `http http://nginx.reproduce-traefik-virtualhost.ddev.site` will show you nginx welcome page stating "Thank you for using nginx."
5. Enable traefik in ddev
6. `ddev poweroff && ddev start`
7. Run the above two `http`-commands. In my testings I got always the "hello world from php", regardless of the host in the url

