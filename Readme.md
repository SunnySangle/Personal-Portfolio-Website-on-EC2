# **Personal Portfolio Website on AWS EC2**

### **Project Overview**
This project demonstrates the deployment of a static personal portfolio website on an AWS EC2 instance. The project highlights essential cloud computing skills, including launching and configuring an EC2 instance, setting up a web server, and deploying a website.

---

## **Features**
- Hosted on an AWS EC2 instance.
- Lightweight and responsive HTML/CSS design.
- Secure configuration with AWS Security Groups.
- Demonstrates proficiency in setting up and managing cloud infrastructure.

---

## **Tech Stack**
- **Cloud Platform:** Amazon Web Services (AWS)
- **Service Used:** EC2 (Elastic Compute Cloud)
- **Web Server:** Apache HTTP Server
- **Frontend Technologies:** HTML, CSS
- **Operating System:** Amazon Linux 2

---

## **Setup Steps**

### **1. Launch an EC2 Instance**
1. Go to the AWS Management Console and navigate to the EC2 service.
2. Create an instance with the following configurations:
   - **AMI:** Amazon Linux 2.
   - **Instance Type:** t2.micro (Free Tier eligible).
   - Configure security groups to allow:
     - **HTTP** (port 80) for website access.
     - **SSH** (port 22) for administrative access.

### **2. Connect to the Instance**
1. Use the provided key pair to SSH into the instance:
   ```bash
   ssh -i "your-key.pem" ec2-user@<public-ip>
   ```

### **3. Install Apache Web Server**
1. Update packages and install Apache:
   ```bash
   sudo yum update -y
   sudo yum install httpd -y
   sudo systemctl start httpd
   sudo systemctl enable httpd
   ```

### **4. Deploy the Portfolio Website**
1. Navigate to the web server's root directory:
   ```bash
   cd /var/www/html
   ```
2. Create and upload the `index.html` file:
   ```bash
   sudo nano index.html
   ```
3. Paste the portfolio content and save the file.

### **5. Access the Website**
1. Open a browser and navigate to:
   ```
   http://54.226.63.51
   ```

---

## **Skills Demonstrated**
- Deploying and managing AWS EC2 instances.
- Setting up and configuring a Linux-based web server.
- Hosting and testing a static website in the cloud.
- Applying basic network security principles using AWS Security Groups.

---

## **Future Enhancements**
- Add SSL/TLS encryption using AWS Certificate Manager.
- Use CloudFront for better performance and content delivery.
- Implement a backend to handle user input (e.g., contact forms).
- Link the EC2 instance to a custom domain name using Route 53.

---

## **Project Screenshot**


---

## **Author**
- **Name:** Sunny Sangle 
- **Email:** [sunnysangle681@gmail.com]  
- **LinkedIn:** [https://www.linkedin.com/in/sunny-sangle-a6172929a/](#)

