# 🎓 School Suite - Complete School Management System

A comprehensive, modern school management system built with NestJS (backend) and Next.js (frontend).

## 📁 Project Structure

```
school-suite/
├── backend/               # NestJS API Server
│   ├── src/              # Source code
│   ├── dist/             # Compiled code
│   ├── test/             # Tests
│   └── package.json      # Backend dependencies
│
├── frontend/             # Next.js Web Application
│   ├── app/              # Next.js app directory
│   ├── components/       # React components
│   ├── lib/              # Utilities
│   └── package.json      # Frontend dependencies
│
├── docker-compose.yml    # Docker services (PostgreSQL, Redis)
└── README.md            # This file
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ installed
- Docker Desktop running (for PostgreSQL)
- npm or yarn package manager

### 1. Start Database Services
```bash
docker-compose up -d
```

### 2. Start Backend (Terminal 1)
```bash
cd backend
npm install
npm run start:dev
```

Backend will run on: `http://localhost:3000`

### 3. Start Frontend (Terminal 2)
```bash
cd frontend
npm install
npm run dev
```

Frontend will run on: `http://localhost:3001`

## 🎯 Features

### ✅ Implemented Modules (Backend)
- **Tenancy Module** - Multi-tenant management, schools, subscriptions
- **Auth Module** - JWT authentication, user management
- **Academics Module** - Academic years, classes, sections, subjects
- **Finance Module** - Fee structures, payments, receipts, installments

### 🎨 Frontend Features
- **Onboarding Flow** - Step-by-step school setup
- **Dashboard** - Overview and analytics
- **Modern UI** - Beautiful, responsive design with Tailwind CSS
- **Authentication** - Login/Register pages

## 📊 API Endpoints

- **100+ REST API Endpoints**
- **JWT Authentication**
- **Role-Based Access Control**
- **Multi-tenant Architecture**

See `backend/src/tenancy/README.md` for detailed API documentation.

## 📚 Documentation

- `APP_RUNNING_SUCCESSFULLY.md` - Quick start guide
- `IMPLEMENTATION_COMPLETE.md` - Implementation details
- `FINAL_STATUS.md` - Complete status overview
- `DATABASE_SETUP.md` - Database setup guide
- `backend/src/tenancy/README.md` - Tenancy API docs
- `backend/src/tenancy/QUICKSTART.md` - API quick start
- `postman_collection.json` - Postman collection

## 🧪 Testing

### Backend Tests
```bash
cd backend
npm run test
npm run test:e2e
```

### Import Postman Collection
Import `postman_collection.json` into Postman for complete API testing.

## 🐳 Docker Services

The `docker-compose.yml` provides:
- **PostgreSQL 17** - Main database (port 5432)
- **Redis 7** - Caching and queues (port 6379)

```bash
# Start services
docker-compose up -d

# View logs
docker-compose logs -f

# Stop services
docker-compose down
```

## 🔒 Default Credentials

After seeding data:
- **Email**: admin@schoolsuite.com
- **Password**: admin123

⚠️ Change these in production!

## 🛠️ Development

### Backend Development
```bash
cd backend
npm run start:dev      # Start with watch mode
npm run build          # Build for production
npm run lint           # Run linter
```

### Frontend Development
```bash
cd frontend
npm run dev            # Start development server
npm run build          # Build for production
npm run start          # Start production server
```

## 📈 Project Progress

- ✅ Backend: 4/15 modules complete (27%)
- ✅ Frontend: Onboarding flow + Authentication
- ✅ Database: PostgreSQL with 29 tables
- ✅ API: 100+ endpoints operational

## 🎓 Tech Stack

### Backend
- NestJS 11
- TypeORM
- PostgreSQL 17
- JWT Authentication
- Class Validator
- Passport.js

### Frontend
- Next.js 15
- React 19
- TypeScript
- Tailwind CSS
- React Hook Form
- Axios

## 📝 Environment Variables

### Backend (.env in backend folder)
```env
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=postgres123
DB_NAME=school_suite
JWT_SECRET=your-secret-key
NODE_ENV=development
PORT=3000
```

### Frontend (.env.local in frontend folder)
```env
NEXT_PUBLIC_API_URL=http://localhost:3000
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the UNLICENSED License.

## 🙏 Support

For issues or questions:
1. Check the documentation files
2. Review the API documentation
3. Check the backend logs
4. Verify Docker services are running

---

**Built with ❤️ for modern school management**

