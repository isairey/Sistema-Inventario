# 📦 Sistema de Gestión de Inventarios de Activos Fijos

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Activo-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/Laravel-5.8-FF2D20?style=for-the-badge&logo=laravel&logoColor=white">
  <img src="https://img.shields.io/badge/PWA-Soportado-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/API-REST-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Licencia-MIT-yellow?style=for-the-badge">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PHP-Backend-777BB4?style=for-the-badge&logo=php&logoColor=white">
  <img src="https://img.shields.io/badge/Laravel-Framework-FF2D20?style=for-the-badge&logo=laravel&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-Frontend-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</p>

---

## 🏥 Descripción

Sistema de gestión de inventarios de **activos fijos** desarrollado con **Laravel 5.8**, diseñado para administrar equipos, usuarios y movimientos dentro de una organización.

El sistema está preparado para:
- 🌐 Arquitectura **RESTful**
- 📱 Uso como **Progressive Web App (PWA)**
- ⚡ Integración con tecnologías modernas

---

## 🚀 Características Principales

- Gestión completa de activos fijos  
- Sistema multiusuario con roles  
- API REST integrada  
- Soporte para PWA  
- Control de movimientos de inventario  
- Arquitectura escalable  

---

## 👥 Roles del Sistema

### 👤 Registrado
- Usuario sin permisos iniciales  

---

### 👨‍💻 Usuario
- Consulta de perfil  
- Visualización de reportes  

---

### 🔧 Administrador
- Control total del sistema  
- Gestión de usuarios e inventario  

---

### ⚙️ SYSTEM
- Configuración global del sistema  

---

## 📦 Módulos del Sistema

### 🧑‍💼 Usuarios
- Gestión de usuarios y roles  

---

### 💻 Equipos
- CRUD de activos  
- Control de inventario  

---

### 🏷️ Modelos
- Administración de modelos de equipos  

---

### 🔄 Movimientos
- Registro de entradas y salidas  
- Control de historial de activos  

---

## 🛠️ Tecnologías Utilizadas

- PHP  
- Laravel 5.8  
- MySQL  
- JavaScript  
- PWA  

---

## ⚙️ Instalación

```bash
cp .env.travis .env
cp .env.travis .env.testing

# Configurar base de datos

sleep 15

mysql -e 'create database inventarios_2;'

composer self-update
composer install --no-interaction

php artisan migrate
php artisan db:seed
