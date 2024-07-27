# Caddy with Docker

## Environment .env

```
CADDY_VERSION=latest
CADDY_FILE_PATH=./Caddyfile
```

### Example Caddyfile

```
monitorpgw.multired.com.bo {
  reverse_proxy localhost:3000
  tls {
    on_demand
  }
}
```
