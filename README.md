# My Node.js Website
A simple Node.js website built with Express.js for demonstrating a basic web application.

## 🖥️ Install Web Server and Packages

# Install Apache, Node.js, npm, and unzip
yum install -y httpd unzip nodejs npm

# Navigate to your project directory
cd /project

# Install Node.js dependencies
npm install
npm run build

# Enable and start Apache web server
systemctl enable --now httpd

# Copy built files to Apache web root
cp -r /project/dist/* /var/www/html/

# Restart the service and access them
Systemctl restrt httpd
