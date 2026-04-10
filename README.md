# Student Project Portfolio Platform (Backend)

A robust Spring Boot backend API for students to manage and showcase projects, now optimized for seamless cloud deployment.

## Stack
- **Backend**: Spring Boot 3 + Java 17
- **Database**: MySQL
- **Authentication**: JWT (JSON Web Tokens)

## Run Locally

```bash
cd backend
./mvnw spring-boot:run
```
*(Or use your IDE to run `StudentPortfolioApplication.java`)*

## Deployment (Railway)

This backend is fully optimized for Railway deployments:
1. **Root Directory**: Make sure to configure the `Root Directory` setting to `/backend` in your Railway Service settings.
2. **Database Auto-Connect**: Add a MySQL database in Railway; this project automatically binds to Railway's `${MYSQLHOST}`, `${MYSQLPORT}`, and `${MYSQLDATABASE}` environment variables.
3. **Optimized limits**: Container RAM is capped at 300MB to prevent `OOM` crashes on free tiers.

## Features
- JWT Authentication (Student / Admin roles)
- Project CRUD with milestone tracking
- Media uploads: Images, PDFs, Videos
- Admin feedback & ratings
- Cross-Origin Resource Sharing (CORS) configured for multi-environment deployed frontend.
