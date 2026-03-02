# THY Transportation & Route Management System ✈️🚌

Bu proje, lokasyonlar arası ulaşım ağlarını yöneten, BFS (Breadth-First Search) algoritması ile rotaları hesaplayan ve Dockerize edilmiş bir Full Stack web uygulamasıdır. 

## 🚀 Proje Hakkında Genel Bakış
Uygulama; hava ve kara yolu ulaşım araçlarını kullanarak, belirli kurallar (aktarma sayısı, ulaşım tipi önceliği vb.) çerçevesinde en uygun rotaları listeler.

### Temel Özellikler:
- **Dinamik Rota Arama:** BFS algoritması ile başlangıç ve varış noktası arasındaki tüm yolları hesaplar.
- **Rol Tabanlı Yetkilendirme:** Spring Security ve JWT kullanılarak `ADMIN` ve `AGENCY` rolleri için farklı erişim seviyeleri.
- **Performans Optimizasyonu:** Redis Cache entegrasyonu ile sık sorgulanan rotaların hızlı getirilmesi.
- **Dockerize Altyapı:** Frontend, Backend ve Redis servislerinin izole ve uyumlu çalışması.

## 🛠️ Kullanılan Teknolojiler

### Backend
- **Java 17 & Spring Boot 3**
- **Spring Security & JWT** (Güvenlik)
- **Redis** (Caching)
- **H2 Database** (In-memory veri saklama)
- **Liquibase** (Veritabanı versiyon yönetimi)

### Frontend
- **React & Vite**
- **Ant design** (Modern UI tasarımı)
- **Axios** (API iletişimi)
- **Nginx** (Production-ready serving & Reverse Proxy)

### DevOps & Altyapı
- **Docker & Docker Compose**

## 📦 Kurulum ve Çalıştırma

Sistemi çalıştırmak için bilgisayarınızda **Docker Desktop** yüklü olmalı

Uygulamaya Erişin:

Frontend: http://localhost:3000

Backend API: http://localhost:8080/api

H2 Console: http://localhost:8080/h2-console (JDBC URL: jdbc:h2:mem:testdb)
