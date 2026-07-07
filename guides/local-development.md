# Local development

## Contracts

```bash
git clone https://github.com/blink-protocol/blink-contracts
cd blink-contracts
cargo test -p link-registry
stellar contract build
```

## Frontend

```bash
git clone https://github.com/blink-protocol/blink-frontend
cd blink-frontend
npm install
cp .env.example .env.local
npm run dev
```

## Backend

```bash
git clone https://github.com/blink-protocol/blink-backend
cd blink-backend
npm install
cp .env.example .env
npm run dev
```

