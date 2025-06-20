## **LAMP (linux,apache,mysql,php) Stack on amazon linux OS**

### **Step 1:  Update System**

  ```
      sudo yum update -y
  ```

### **Step 2: Install apache(https)**

  ```
    sudo yum install httpd -y
    sudo systemctl start httpd
    sudo systemctl enable httpd
  ```

### **Step 3: Install mariaDB (MYSQL-compatible)**

  ```
    sudo dnf install mariadb105-server -y
    sudo systemctl start mariadb
    sudo systemctl enable mariadb
  ```

### **Step 4: Install PHP and Required Modules**
  
  ```
    sudo dnf install php php-mysqlnd php-cli php-gd php-xml php-mbstring -y
  ```

### **Step 6: Restart Apache**

  ```
    sudo systemctl restart httpd
  ```


