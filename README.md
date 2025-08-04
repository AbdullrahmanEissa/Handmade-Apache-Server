# 🌐 Full Apache2 Built From Scratch With Docker


<img width="1858" height="781" alt="Aws Ec2" src="https://github.com/user-attachments/assets/13aea80a-c743-4242-b7ae-e8f79d00f0e2" />
<img width="1482" height="870" alt="EC2 SSH" src="https://github.com/user-attachments/assets/d34e2727-09ec-4e26-9e28-7e6aef0a10e3" />
<img width="1401" height="984" alt="Docker Installation" src="https://github.com/user-attachments/assets/0c4e6387-cac0-4eaa-b321-95d34eb2d911" />
<img width="999" height="385" alt="Git Clone HTTPD REPO" src="https://github.com/user-attachments/assets/9e2308bf-8def-4cb8-8a53-e99bb31fb118" />
<img width="1908" height="817" alt="itworks" src="https://github.com/user-attachments/assets/58c03ebc-2cdf-4aed-99c8-ab51a37ee108" />
<img width="674" height="384" alt="docker build 2" src="https://github.com/user-attachments/assets/5c93550f-be62-4cc9-8097-4ede58747c73" />


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
