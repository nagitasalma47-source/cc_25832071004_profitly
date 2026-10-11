# Profitly

Cloud Computing — PTI 2802  
Pertemuan 3 — Project Inception

## Author
Nama: Neng Nagita Salma  
NIM: 25832071004  
Kelas: 2A

## Problem
Pelaku usaha perlu mengetahui omzet, modal, biaya operasional, dan perkiraan keuntungan agar dapat memahami kondisi keuangan usahanya dengan lebih mudah.

Profitly dirancang sebagai aplikasi web untuk membantu pelaku usaha memantau informasi keuangan dan keuntungan penjualan.

## Target Users
- Pemilik usaha online.
- Pelaku UMKM.
- Pengelola usaha kecil.

## Features M03
- Baseline application.
- Health endpoint.
- VPS deployment.

## Architecture

```mermaid
flowchart LR
    U[User] --> C[Caddy]
    C --> G[Gunicorn]
    G --> F[Flask]
```

## Infrastructure
- Ubuntu Server 24.04
- 1 vCPU
- 1 GB RAM
- 20 GB disk
- Caddy
- Gunicorn

## Public Endpoint
`http://27.112.79.135/`

## Health Check
`GET /health`

## Deployment
See `docs/deployment.md`.

## Security
- Key-only SSH.
- Root SSH disabled.
- UFW enabled.
- Backend loopback-only.

## Current Limitations
- HTTP only.
- No persistent database.
- No container.
- Manual deployment.

## Roadmap
- M04 DNS/HTTPS.
- M05 Data.
- M06 Container.
- M07 IaC.
- M09 CI/CD.
