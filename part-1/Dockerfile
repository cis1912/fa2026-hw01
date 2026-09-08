FROM node:20-slim AS builder

# Build the frontend

FROM caddy:alpine

# Copy the build output from the builder image

EXPOSE 80

CMD ["caddy", "run", "--config", "/etc/caddy/Caddyfile", "--adapter", "caddyfile"]
