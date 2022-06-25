- Secure Gaming Platform .

> Built with React, Redux, and Node.js.
---

## Setup

1. Clone the repo.
2. Generate SSH keys.
   From app folder:
   ```
   mkdir -p backend/keys
   ssh-keygen -t rsa -b 2048 -m PEM -f backend/keys/jwt
   ```
3. Install npm packages.
   From app folder:
   ```
   cd frontend
   npm i
   cd ../backend
   npm i
   ```
4. Configure `backend/.env.example` and rename it to `.env`

---

## Features

- **Server Channels**
  - Create channels
  - Delete channels
- **Message Management**
  - Server owners can delete any message
  - Message author can delete and edit their own messages
- **Member Management**
  - Kick members as the server owner
  - Easily leave the server by right clicking the server
  - Join servers with an invite code
- **Server Management**
  - Create servers as you would in Discord
  - Edit server name, and icon URL in the server settings
  - Delete your server in the server settings
- **User Management**
  - Manage your account by clicking the settings icon
  - Change your username, and avatar
  - Delete your user and prevent it from being used to login
- **and more** (of course)
---

`backend/.env`
(dev with Docker)

```
EMAIL_ADDRESS="...@gmail.com"
EMAIL_PASSWORD="..."
MONGO_URI="mongodb://database/accord"
NODE_ENV="dev"
PORT=3000
WEBSITE_URL="http://localhost:4200"
```

`backend/test/.env`
(test without Docker)

```
API_URL="http://localhost:3001/api"
EMAIL_ADDRESS="...@gmail.com"
EMAIL_PASSWORD="..."
MONGO_URI="mongodb://localhost/accord-test"
NODE_ENV="dev"
PORT=3001
ROOT_ENDPOINT="http://localhost:3001"
WEBSITE_URL="http://localhost:4200"
```
