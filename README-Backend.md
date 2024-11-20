
# Conectando Huellas "BACKEND"

Es una aplicación sin fines de lucro que busca conectar a las mascotas en adopción con posibles dueños interesados, y también permite que los dueños que han extraviado sus mascotas puedan publicar un anuncio para poder encontrar a su respectiva mascota extraviada.

#### Mision 

Ser la primera opción para la publicación de mascotas en adopción, y de anuncios de mascotas perdidas.

#### Vision

Lograr aumentar el índice de adopción de mascotas, y la reducción de animales perdidos en el Perú.

## 🚀 Tecnologías
* ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
* ![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
* ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
* ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
* ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
* ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)
* ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=white)

## 📋 Requisitos Previos
* ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
* ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
* ![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)
* ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)


## Instalación

#### Bash

```
  git clone https://github.com/tu-usuario/MIR-conectando-huellas-backend.git

  cd MIR-conectando-huellas-backend

  npm install

  npm run dev
```


## 📁 Estructura del Proyecto
```
MIR-conectando-huellas-backend/
├── prisma/
   └── schema.prisma/
├── src/
   ├── config/         
   ├── controllers/    
   ├── middleware/     
   ├── models/         
   ├── routes/         
   ├── services/       
   ├── utils/          
   └── app.ts          
```

## ⚙️ Configuración
Variables de Entorno

#### .env
```
# Server
PORT=9090
NODE_ENV=development

# Database
DATABASE_URL="postgresql://usuario:contraseña@localhost:5432/mir_conectando_huellas?schema=public"

# JWT
JWT_SECRET_KEY=tu_clave_secreta
JWT_EXPIRES_IN=24h

# Email
GMAIL_USER=tu_email@gmail.com
GMAIL_PASS=tu_contraseña_app

# Cloudinary
CLOUDINARY_CLOUD_NAME=tu_cloud_name
CLOUDINARY_API_KEY=tu_api_key
CLOUDINARY_API_SECRET=tu_api_secret
```


## 🔗 API Endpoints

#### Obtener Mascotas Perdidas

```
  GET /api/pets/lost    
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `status` | `string` | Filtrar por estado (LOST, FOUND)  |
| `species` | `string` | Filtrar por especie (DOG, CAT)  |

#### Registrar usuario

```
  POST /api/user/register
```

| Parameter | Type | Description |
| :-------- | :------- | :-------------------------------- |
| name | string | Required. Nombre del usuario |
| email | string | Required. Email único |
| password | string | Required. Contraseña |
| phone | string | Required. Teléfono |
| address | string | Required. Dirección |

#### Actualizar Estado de Mascota

```
  PATCH /api/pets/${id}/status
```

| Parameter | Type | Description |
| :-------- | :------- | :------------------------- |
| id | string | Required. ID de la mascota |
| status | string | Required. Nuevo estado (LOST, FOUND) o (ADOPTION, ADOPTED) |

## 📤 Subida de Archivos
Las imágenes se suben a Cloudinary. Formatos soportados:
* JPG/JPEG
* PNG
* WebP


## 📝 Licencia
Este proyecto está bajo la Licencia MIT - ver el archivo LICENSE.md para detalles 

## 🙏 Agradecimientos
* A todos los participantes del proyecto.
* Profesores de Make It Real



## 🔗 Autores
#### Ana Albirena
[![github](https://img.shields.io/badge/github-000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/annalbirena)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ana-albirena/)

#### Anthony Antezanza
[![portfolio](https://img.shields.io/badge/github-000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Akuma2522)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
#### Alexander Puma
[![portfolio](https://img.shields.io/badge/github-000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AlexPumaPrado)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/alexander-puma-prado/)
