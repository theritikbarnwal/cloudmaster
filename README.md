# 🔐 Flask Login System with MongoDB & Sessions

A clean and minimalistic authentication system built using **Flask** and **MongoDB**, implementing:

- 💼 **User registration**
- 🔑 **Session-based login**
- 🔄 **Password reset flow**
- 🔐 **Secure password hashing**
- 🔓 **Logout functionality**

All powered by a simple Flask backend and organized with modular routes and secure practices.

---

## 🧰 Technology Stack

- **Flask** – Lightweight Python web framework  
- **MongoDB** – NoSQL database accessed via `pymongo`  
- **bcrypt** – Secure password hashing  
- **Flask sessions** – Manages authentication state  
- **dotenv** – Secure environment variable configuration  
- **Jinja2 + HTML** – Server-side templates for UI

---

## 🗂️ Project Structure

```

login\_db/
├── app.py                    # Main Flask application
├── .env                      # Environment variables (e.g., MONGO\_URI, SECRET\_KEY)
├── requirements.txt          # Dependencies
└── templates/                # HTML templates
├── register.html
├── login.html
├── forgot.html
├── reset.html
└── dashboard.html
└── test_app.py

````

---

## 🚀 Features Overview

### 1. **Registration**
- Stores user credentials in MongoDB with bcrypt-hashed passwords.

### 2. **Login**
- Validates credentials and initiates a session on success.

### 3. **Forgot + Reset Password**
- Allows users to reset their password using username-based identification ➡️ hashed update.

### 4. **Logout**
- Clears the session and redirects back to login page.

---

## 🛠️ Why I Built This

I wanted a **clean, modular login backend** to use as a foundation for other projects or CI/CD pipelines. This is a learning exercise to:

- Learn Flask session management
- Securely handle authentication workflows
- Structure backend routes cleanly and maintainably :contentReference[oaicite:1]{index=1}

---

## ⚙️ How to Run Locally

```bash
git clone https://github.com/theritikbarnwal/DevOps.git
cd DevOps/login_db

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Create a .env file with MONGO_URI and SECRET_KEY

python app.py
````

Then visit **[http://127.0.0.1:5000/](http://127.0.0.1:5000/)**

---

## ✅ What I Learned

* 🛡️ Secure password storage with bcrypt
* 🔗 Flask sessions to maintain login state
* 🗂️ Route structure for login, registration, and password reset
* 🔐 Using environment variables responsibly with `dotenv`
* 🗃️ Basic MongoDB interactions using `pymongo`

---

## 🚀 Next Steps

* Integrate an **email-based password reset** flow
* Package and **Dockerize** the app
* Add **CI/CD pipeline** (e.g., GitHub Actions)
* Deploy to a cloud platform (Railway or Render)

---

## 📚 References

* Original Dev.to article: *Building a Clean Flask Login System with MongoDB, Sessions, and Password Reset* ([dev.to][1])

---

### 🤝 Feedback & Collaboration

If you have suggestions—whether for the password reset flow, route structure, or Dockerization—feel free to open an issue or pull request. Always open to learning and improving!

```

---

### ✅ Why This Works:
- 🎯 **Clarity**: Highlights what the project does, why it matters, and how to run it.
- 🛠 **Tech Stack**: Lists all tools and frameworks used.
- 🧩 **Modular Structure**: Shows readers how the project is organized.
- 🔄 **Future Improvements**: Indicates your roadmap and ambition.

Feel free to adjust any section or add images, screenshots, or badges.
::contentReference[oaicite:13]{index=13}
```

[1]: https://dev.to/theritikbarnwal/building-a-clean-flask-login-system-with-mongodb-sessions-and-password-reset-5f03?utm_source=chatgpt.com "Building a Clean Flask Login System with MongoDB, Sessions, and ..."


