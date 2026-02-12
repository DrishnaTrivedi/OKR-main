# OKR Backend — NestJS API

This is the backend service for the **OKR (Objectives and Key Results)** application.  
It is built using **NestJS**, **Prisma ORM**, and **PostgreSQL**.

The API provides endpoints to manage objectives and key results following a modular and scalable architecture.

---

## 🧠 Tech Stack

- **Backend Framework:** NestJS (TypeScript)
- **ORM:** Prisma
- **Database:** PostgreSQL
- **Validation:** class-validator
- **Testing:** Jest, 

---


## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Avani-prajapati/OKR-main.git
cd OKR-main/nest-backend
```

---

### 2️⃣ Install Dependencies

```bash
npm install
```

---

### 3️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

Update the `DATABASE_URL` inside `.env`:

```
DATABASE_URL="postgresql://username:password@localhost:5432/okr_db?schema=public"
```

Example:

```
DATABASE_URL="postgresql://postgres:postgres@localhost:5432/okr_db"
```

---

### 4️⃣ Setup Database

No need to install postgres as we have docker-compose.yml

Create the database:

### 5️⃣ Run Prisma Migrations

Generate Prisma Client:

```bash
pnpx prisma generate
```

Run migrations:

```bash
pnpx prisma migrate dev
```

If migrations are not present, push schema:

```bash
npx prisma db push
```

---

### 6️⃣ Run the Application

Development mode:

```bash
pnpm run start:dev
```

The server will start at:

```
http://localhost:3000
```

---
