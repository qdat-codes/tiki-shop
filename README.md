# 🛒 Tiki Shop — MERN Stack E-commerce Platform

<div align="center">

![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Mongoose-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white)

A full-stack e-commerce web application inspired by Tiki, built with the MERN stack. Features JWT authentication, role-based access control, and a complete shopping experience from product browsing to order management.

**Ứng dụng thương mại điện tử full-stack lấy cảm hứng từ Tiki, xây dựng trên nền tảng MERN Stack với xác thực JWT, phân quyền người dùng và trải nghiệm mua sắm hoàn chỉnh.**

[Demo](#) · [Report Bug](https://github.com/qdat-codes/tiki-shop/issues) · [Request Feature](https://github.com/qdat-codes/tiki-shop/issues)

</div>

---

## 📁 Project Structure / Cấu trúc dự án

```
tiki-shop/
├── mern-ecommerce/        # Frontend (React + TypeScript)
└── ecommerce-backend/     # Backend (Node.js + Express)
```

---

## ✨ Features / Tính năng

### 👤 Authentication & Authorization / Xác thực & Phân quyền
- User registration & login with JWT — *Đăng ký & đăng nhập với JWT*
- Role-based access control (Admin / User) — *Phân quyền theo vai trò*
- Protected routes for authenticated users — *Bảo vệ route cho người dùng đã đăng nhập*

### 🛍️ Shopping Experience / Trải nghiệm mua sắm
- Product listing with search & filter — *Danh sách sản phẩm, tìm kiếm & lọc*
- Product detail page — *Trang chi tiết sản phẩm*
- Shopping cart (add, remove, update quantity) — *Giỏ hàng*
- Order placement & order history — *Đặt hàng & lịch sử đơn hàng*

### 🛠️ Admin Dashboard / Trang quản trị
- Product CRUD (Create, Read, Update, Delete) — *Quản lý sản phẩm*
- Order management — *Quản lý đơn hàng*
- User management — *Quản lý người dùng*

---

## 🧰 Tech Stack / Công nghệ sử dụng

### Frontend
| Technology | Purpose |
|---|---|
| React 18 + TypeScript | UI framework |
| Redux Toolkit | Global state management |
| React Query (TanStack) | Server state & data fetching |
| React Router v6 | Client-side routing |
| Ant Design | UI component library |
| Axios | HTTP client |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express | REST API server |
| MongoDB + Mongoose | Database & ODM |
| JSON Web Token (JWT) | Authentication |
| bcryptjs | Password hashing |
| dotenv | Environment configuration |

---

## 🚀 Getting Started / Hướng dẫn cài đặt

### Prerequisites / Yêu cầu

- Node.js >= 18.x
- MongoDB (local or [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))
- npm hoặc yarn

---

### 🖥️ Backend Setup

```bash
# 1. Navigate to backend folder
cd ecommerce-backend

# 2. Install dependencies
npm install

# 3. Create environment file
cp .env.example .env
```

Configure your `.env` file:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRES_IN=7d
```

```bash
# 4. Start the server
npm run dev
```

Backend runs on: `http://localhost:5000`

---

### 💻 Frontend Setup

```bash
# 1. Navigate to frontend folder
cd mern-ecommerce

# 2. Install dependencies
npm install

# 3. Create environment file
cp .env.example .env
```

Configure your `.env` file:

```env
VITE_API_URL=http://localhost:5000/api
```

```bash
# 4. Start the development server
npm run dev
```

Frontend runs on: `http://localhost:5173`

---

## 📡 API Endpoints / Các endpoint API

### Auth
| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/auth/register` | Register new user |
| `POST` | `/api/auth/login` | Login & get JWT token |

### Products
| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/products` | Get all products |
| `GET` | `/api/products/:id` | Get product by ID |
| `POST` | `/api/products` | Create product *(Admin)* |
| `PUT` | `/api/products/:id` | Update product *(Admin)* |
| `DELETE` | `/api/products/:id` | Delete product *(Admin)* |

### Orders
| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/orders` | Create new order |
| `GET` | `/api/orders/my-orders` | Get current user's orders |
| `GET` | `/api/orders` | Get all orders *(Admin)* |
| `PUT` | `/api/orders/:id` | Update order status *(Admin)* |

---

## 📸 Screenshots / Ảnh chụp màn hình

> *Coming soon — Add screenshots of your app here*
>
> *Sắp có — Thêm ảnh chụp màn hình ứng dụng của bạn vào đây*

---

## 🔮 Future Improvements / Hướng phát triển

- [ ] Payment integration (VNPay / Stripe) — *Tích hợp thanh toán*
- [ ] Product reviews & ratings — *Đánh giá sản phẩm*
- [ ] Real-time notifications — *Thông báo thời gian thực*
- [ ] Pagination & infinite scroll — *Phân trang*
- [ ] Deploy to cloud (Vercel + Railway/Render) — *Triển khai lên cloud*

---

## 👨‍💻 Author / Tác giả

**Pham Quoc Dat**

- GitHub: [@qdat-codes](https://github.com/qdat-codes)
- Email: pqdatIT2304@gmail.com

---

## 📄 License

This project is for learning and portfolio purposes.

*Dự án này được xây dựng cho mục đích học tập và portfolio cá nhân.*
