# Requirements

## Problem Statement

Pelaku usaha perlu mengetahui omzet, modal, biaya operasional, dan perkiraan keuntungan agar dapat memahami kondisi keuangan usahanya dengan lebih mudah.

Profitly dirancang sebagai aplikasi web untuk membantu pelaku usaha memantau informasi keuangan dan keuntungan penjualan.

## Target Users

- Pemilik usaha online.
- Pelaku UMKM.
- Pengelola usaha kecil.

## Functional Requirements

- FR-01 Aplikasi menampilkan halaman utama Profitly.
- FR-02 Aplikasi menyediakan endpoint `/health` untuk memeriksa status aplikasi.
- FR-03 Aplikasi menyediakan endpoint `/api/info` untuk menampilkan informasi proyek.
- FR-04 Aplikasi dirancang untuk mendukung pengembangan fitur pencatatan dan analisis keuntungan usaha pada tahap berikutnya.

## Non-Functional Requirements

- NFR-01 backend loopback-only
- NFR-02 application managed by systemd
- NFR-03 public request through reverse proxy
- NFR-04 no secret in repository

## Constraints

- 1 vCPU
- 1 GB RAM
- 20 GB disk
- Ubuntu Server 24.04
- public IPv4

## Acceptance Criteria M03

- [x] first deployment accessible
- [x] health endpoint works
