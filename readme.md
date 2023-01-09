# Steps to reproduce

1. Disable traefik in ddev
2. `http http://reproduce-traefik-virtualhost.ddev.site` will show you "hello world from php"
3. `http http://nginx.reproduce-traefik-virtualhost.ddev.site` will show you nginx welcome page stating "Thank you for using nginx."
4. Enable traefik in ddev
5. `ddev poweroff && ddev start`
6. Run the above two `http`-commands. In my testings I got always the "hello world from php", regardless of the host in the url

