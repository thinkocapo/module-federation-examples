# Create React App Example

This example demos a basic host application loading remote component.

- `host` is the host application (cra-based).
- `remote` standalone application (cra-based) which exposes `Button` component.

# Running Demo

Run `yarn start`. This will build and serve both `host` and `remote` on ports 3001 and 3002 respectively.

- [localhost:3001](http://localhost:3001/) (HOST)
- [localhost:3002](http://localhost:3002/) (STANDALONE REMOTE)


## Troubleshooting
Your node version might be off. I switched to:
```
nvm use 14.17.0
```

On first yarn install it might say 'port 3000 already in use'
```
lsof -i tcp:3000 
kill <pid>

or

npx kill-port 3000
```