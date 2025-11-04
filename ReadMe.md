### Installation guide 
- SSH into your Amazon Linux 2023 EC2 Instance.
- Download the MySQL Community Yum Repository RPM:

```sudo wget https://dev.mysql.com/get/mysql84-community-release-el9-1.noarch.rpm```

# Install the MySQL Community Yum Repository.
```sudo dnf install mysql84-community-release-el9-1.noarch.rpm -y```

# Import the MySQL GPG Key.
```sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2023```

# Install the MySQL Server.
```sudo dnf install mysql-community-server -y```

# Start the MySQL Service.
```sudo systemctl start mysqld```

# Enable the MySQL Service to start on boot:
```sudo systemctl enable mysqld```

# Verify the MySQL Service Status.
```sudo systemctl status mysqld```

