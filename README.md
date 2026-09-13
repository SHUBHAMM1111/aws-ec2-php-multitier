# Deploying Multi-Tier Website Using AWS EC2 & Amazon RDS

## Project Overview
A scalable multi-tier web application architecture deployed on AWS Elastic Beanstalk (PHP runtime), featuring a user data collection frontend securely connected to an Amazon RDS MySQL backend database.

---

## Architecture & Key Features

* **Website Development:** Developed a PHP-based web application interface (`Upload Employee Data`) designed for user input and interaction.
* **Data Gathering:** Implemented form handlers to capture data points including Employee ID, Name, Date of Birth, and Department.
* **Data Security:** Deployed the application within a secure AWS environment with managed network access controls.
* **Database Integration:** Configured and integrated the application with an Amazon RDS MySQL database (`ebdb`) to store and query the submitted records persistently.

---

## Project Screenshots

### 1. Elastic Beanstalk Environment Overview
*Shows the active AWS Elastic Beanstalk environment running PHP 8.2 on Amazon Linux 2023 with the generated public endpoint domain.*
![Elastic Beanstalk Environment](https://github.com/SHUBHAMM1111/aws-ec2-php-multitier/blob/ede214a9c102322ededfafe466b41d3f4a8f4ecc/Project-2-%E2%80%93-Website-Orchestration-2/Environment%20overview%20-%20events%20_%20Elastic%20Beanstalk%20_%20us-east-1%20-%20Google%20Chrome%2021-May-24%206_32_30%20PM.png)

### 2. Website User Interface & Data Entry
*The live PHP web interface successfully capturing employee details (ID, Name, DOB, Department) and returning a success message.*
![Website UI Form](https://github.com/SHUBHAMM1111/aws-ec2-php-multitier/blob/ede214a9c102322ededfafe466b41d3f4a8f4ecc/Project-2-%E2%80%93-Website-Orchestration-2/Environment%20overview%20-%20events%20_%20Elastic%20Beanstalk%20_%20us-east-1%20-%20Google%20Chrome%2021-May-24%206_32_43%20PM.png)

### 3. Amazon RDS Database Storage Verification
*MySQL terminal session confirming successful connection to the `ebdb` database and displaying records stored in the `employees` table from the web form.*
![RDS Database Backend]([Project-2-–-Website-Orchestration-2/Screenshot 21-May-24 6_32_05 PM.png](https://github.com/SHUBHAMM1111/aws-ec2-php-multitier/blob/650c03b4cdf47706eafceff6062aa42e51693541/Project-2-%E2%80%93-Website-Orchestration-2/Screenshot%2021-May-24%206_32_05%20PM.png))

---

## How to Deploy
1. Clone the repository: `git clone https://github.com/Mane46680/your-repo-name.git`
2. Bundle your PHP source files into a ZIP archive.
3. Deploy the application package via the AWS Elastic Beanstalk console.
4. Ensure your security groups allow your application instances to communicate with your Amazon RDS MySQL instance.
