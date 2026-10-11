# ADR-0001: Initial Architecture

## Status
Accepted

## Context
Profitly membutuhkan deployment awal yang dapat diakses melalui public IPv4 dengan sumber daya VPS terbatas, yaitu 1 vCPU, 1 GB RAM, dan 20 GB disk.

## Decision
Arsitektur awal Profitly menggunakan:
- Ubuntu Server 24.04 sebagai sistem operasi server.
- Flask sebagai aplikasi web.
- Gunicorn sebagai application server pada `127.0.0.1:8000`.
- Caddy sebagai reverse proxy pada port 80.
- systemd untuk mengelola layanan aplikasi `cc-m03`.
- UFW sebagai firewall server.
- SSH key authentication dengan login root dan autentikasi password dinonaktifkan.

## Consequences
- Aplikasi dapat diakses melalui public IPv4 menggunakan HTTP.
- Backend hanya menerima koneksi langsung melalui loopback.
- Layanan aplikasi dapat dikelola menggunakan systemd.
- HTTPS dan domain belum diterapkan pada M03.
