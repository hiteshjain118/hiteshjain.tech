# hiteshjain.tech

Personal site for Hitesh Jain. One page, plus a couple of long-form pieces.

Static HTML and CSS — no build step, no dependencies. Served by GitHub Pages
from the `main` branch.

```
index.html                          the page
style.css                           shared styles (light + dark)
writing/embedding-inference.html    Domain-Specific Embedding Inference with Sub-20ms Tail Latency
writing/embedding-performance.html  Embedding Performance for Real-Time Retrieval Systems
images/                             article figures
CNAME                               custom domain
```

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages rebuilds automatically.

## DNS

The apex domain needs four A records pointing at GitHub Pages:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

And, for the `www` subdomain, a CNAME to `hiteshjain118.github.io`.
