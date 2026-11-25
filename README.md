# Vishal Ojha — static preview

Personal real estate brokerage website for Vishal Ojha, Mumbai. This is a static, preview-only build; it does not deploy or modify DNS.

## Preview

```bash
python3 -m http.server 4173 --directory site
```

Open <http://localhost:4173>.

## Build

```bash
npm run build
```

The build copies the static site into `dist/`.

## Docker

```bash
docker build -t vishalojha-site .
docker run --rm -p 8080:80 vishalojha-site
```

Coolify can use the repository root, the `main` branch, base directory `/`, and the Dockerfile build pack. The container serves the site on port `80`.
