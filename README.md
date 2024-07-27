# Caddy with Docker

## Environment .env

```properties
CADDY_VERSION=latest
CADDY_FILE_PATH=./Caddyfile
```

### Example Caddyfile

First create Caddyfile

```bash
touch Caddyfile
```

```
monitorpgw.multired.com.bo {
  reverse_proxy localhost:3000
  tls {
    on_demand
  }
}
```
