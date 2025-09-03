# Golang_Template

Template project Golang dengan struktur modular dan siap pakai untuk pengembangan aplikasi web menggunakan Echo Framework.

## Fitur Utama
- Struktur folder yang rapi (app, cmd, docs, pkg)
- Contoh implementasi controller, repository, usecase
- File Dockerfile untuk kontainerisasi
- Skema database (docs/postgres_schema.sql)
- Manajemen konfigurasi & environment
- Contoh error handling dan custom error

## Struktur Folder

```
├── app/            # Business logic (controller, model, repository, usecase)
├── cmd/            # Entry point aplikasi & command line tools
├── docs/           # Dokumentasi & skema database
├── pkg/            # Package utilitas (config, database, customerror)
├── Dockerfile      # Build image Docker
├── go.mod          # Modul Go
├── go.sum          # Dependency checksum
```

## Cara Memulai

### 1. Clone repository
```bash
git clone https://github.com/TambunanMagdalena/Golang_Template.git
cd Golang_Template
```

### 2. Copy file environment contoh
```bash
cp cmd/.env.example .env
```
Lalu sesuaikan konfigurasi database dan environment sesuai kebutuhan.

### 3. Install dependency
```bash
go mod tidy
```

### 4. Jalankan aplikasi
```bash
go run cmd/main.go
```

### 5. Build menggunakan Docker (opsional)
```bash
docker build -t golang_template .
docker run -p 8080:8080 golang_template
```

## Kontribusi

Pull request dan issue sangat diterima!  
Silakan gunakan branch terpisah untuk pengembangan fitur atau bugfix.

## Lisensi

MIT License

---

**By [TambunanMagdalena](https://github.com/TambunanMagdalena)**
