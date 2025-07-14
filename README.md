# 📝 Serverless Todo App

This is a simple **Serverless TODO App** built with:

- AWS Lambda (backend logic)
- API Gateway (REST API)
- DynamoDB (storage)
- Serverless Framework (deployment)
- Vanilla HTML + JS (frontend)

---

## 🚀 Features

- Add new tasks
- Get all tasks
- Deployed fully on AWS using Serverless Framework
- Backend is fully serverless (no EC2, no traditional servers)

---

## 🗂️ Project Structure

```
serverless-todo-app/
│
├── frontend/
│   ├── index.html        # UI
│   └── app.js            # Calls API
│
├── lambdas/
│   ├── createTask.js     # Lambda to insert task into DynamoDB
│   └── getTasks.js       # Lambda to fetch tasks
│
└── serverless.yml        # Deployment config
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/yourname/serverless-todo-app.git
cd serverless-todo-app
```

### 2. Install Serverless CLI

```bash
npm install -g serverless
```

### 3. Configure AWS Credentials

```bash
aws configure
```

> Enter your **Access Key**, **Secret Key**, region (like `ap-south-1`), and output format (`json`)

---

## 📦 Deploy to AWS

```bash
serverless deploy
```

After a successful deploy, the terminal will show:

- POST endpoint to add tasks
- GET endpoint to fetch tasks

---

## 🔗 Example API Endpoints

```http
POST https://your-api-id.execute-api.ap-south-1.amazonaws.com/dev/tasks
GET  https://your-api-id.execute-api.ap-south-1.amazonaws.com/dev/tasks
```

---

## 🧪 Test API (Using Hoppscotch/Postman)

### POST Body Example (JSON)

```json
{
  "task": "Complete AWS serverless app"
}
```

---

## 💻 Frontend Setup

1. Go to `frontend/index.html`
2. Update the API endpoint URLs in `app.js` if needed
3. Open the HTML file in your browser

---

## 🛠 Technologies Used

- AWS Lambda
- API Gateway
- DynamoDB
- Serverless Framework
- JavaScript (Node.js runtime)
- HTML/CSS/JS (Frontend)

---

## 🙌 Author

Made by Janani
📧 Contact: jananijane03@gmail.com

---

## 📝 License

MIT License
