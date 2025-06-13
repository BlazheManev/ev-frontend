# ⚡ SmartCharge EV Frontend

A responsive web interface for SmartCharge AI — an intelligent system for predicting electric vehicle (EV) charging station availability. This frontend enables both EV users and infrastructure administrators to interact with prediction data, map views, and station metrics.

---

## 🚀 Features

* 📍 **Map View**: Real-time display of EV stations with occupancy info
* 🧠 **Admin Panel**: Track model performance (RMSE, MAE, run IDs)
* 📊 **Drift Reports**: Visual diagnostics for data and model drift
* 🗂 **Dynamic filtering**: By station and date
* 💡 **Smart UX**: Responsive design for desktops and tablets

---

## 🧱 Tech Stack

* ⚙️ **Vite** + **React** + **TypeScript**
* 🗽 **React-Leaflet** for interactive maps
* 🎨 CSS modules
* 📡 Integrated with backend via REST API
* 🔐 Deployed on Vercel

---

## 🗜️ Project Structure

```
src/
├── api/              # API fetch functions (stations, models)
├── assets/           # Static assets (icons, SVGs)
├── components/       # Reusable UI components
├── pages/            # Views: map, reports, admin panel
├── types/            # TypeScript interfaces for models and stations
├── App.tsx           # Root component
├── main.tsx          # Entry point
```

---

## 🛠️ Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/your-username/smartcharge-frontend.git
cd smartcharge-frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start local development server

```bash
npm run dev
```

Vite will serve the app at [http://localhost:5173](http://localhost:5173)

---

## 🐳 Docker

### Build image

```bash
docker build -t blazhe/smartcharge-frontend:latest .
```

### Run container

```bash
docker run -p 3000:80 blazhe/smartcharge-frontend:latest
```

---

## 🔗 API Endpoints

Make sure the backend is running and accessible at:

```bash
https://smartcharge-backend.onrender.com
```
or localy clone backend(https://github.com/BlazheManev/smartCharge-backend)
```bash
http://localhost:3000/
```
Endpoints used:

* `/api/ev-data` → Fetch station info
* `/api/ml-models` → Fetch model metadata
* `/reports/view/:id` → Fetch HTML reports

---

## 🌐 Live Deployment

Frontend is deployed on **Vercel**:

🔗 [https://smart-charge-frontend.vercel.app](https://smart-charge-frontend.vercel.app)

---

## 👨‍💻 Author

Blazhe Manev

---

