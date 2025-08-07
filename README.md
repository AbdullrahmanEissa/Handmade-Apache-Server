# 🌐 Full Apache2 Built From Scratch With Docker


![collage](https://github.com/user-attachments/assets/fdc7716e-21fa-4113-b910-068cd41e545b)



Welcome to a Docker-powered Apache setup running on AWS EC2! This project sets up a lightweight HTTP server inside a Docker container, all deployed on an EC2 instance.

---

## 🚀 Project Overview

- 🔧 Provisioned an EC2 instance from AWS Console
- 🔐 Connected via SSH
- 📦 Installed Docker and Git
- 🛠️ Cloned and built the `httpd` (Apache) Docker image
- 🔥 Exposed Apache server on port `80`
- ✅ Verified successful launch in browser

---

## 📸 Preview

> Apache Server running at: `http://<your-ec2-public-ip>/`

---

## 📦 Installation Steps

```bash
# 1️⃣ Update and install dependencies
sudo apt update
sudo apt install docker.io git -y

# 2️⃣ Clone the project (example)
https://github.com/docker-library/httpd.git

# 3️⃣ Build and run Apache container
docker build -t apache .
docker run -dit --name my-apache -p 80:80 apache
```

---

## 🐳 Docker Details

- Image used: `httpd` (Apache official)
- Container name: `my-apache`
- Port mapping: `80:80`
- Persistent logs: `docker logs my-apache`

---

## 🛡️ Security Notes

Be sure to:
- Configure security groups on EC2 to allow inbound traffic on port `80`
- Restrict access via IP if necessary

---

## 🎯 Future Ideas

- Add SSL via Let's Encrypt
- Automate deployment with Terraform or Ansible
- Add basic web content to `/usr/local/apache2/htdocs/`

---

## 📚 Resources

- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
- [Docker Apache Image](https://hub.docker.com/_/httpd)
- [Your GitHub Repo](https://github.com/eissa-stack/CLOUD-)

---

> _“Built for speed, deployed with style.”_ 🛸

---

## 👨‍💻 Author

**AbdullrahmanEissa**  
🔗 GitHub: https://github.com/AbdullrahmanEissa/

---
```
