# Graphana-Visualization-Banking-Project

![Project Badge](https://img.shields.io/badge/Project-Banking%20Dashboard-brightgreen)  
Welcome to the **Banking Transactions Dashboard** project! This repository demonstrates how to process transaction data, visualize patterns, and detect anomalies using **PostgreSQL**, **Grafana**, and **AWS RDS**. 🚀

## Features 🎯
- Process banking transactions with custom rules.
- Store and manage data using PostgreSQL.
- Visualize transaction patterns in **Grafana**.
- Detect anomalies and high-risk transactions.

---

## Prerequisites 🛠️

1. **AWS Account**
   - Create an AWS account [here](https://aws.amazon.com/).
2. **AWS CLI**
   - Download and install the AWS CLI [here](https://aws.amazon.com/cli/).
   - Run `aws configure` to set up access keys.

---

## Setup Instructions 📦

### 1. Clone the Repository 🖥️
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

### 2. Install Required Packages 📚
```bash
pip install -r requirements.txt
```

### 3. Create AWS RDS Instance 🌐
1. Log in to the AWS Management Console.
2. Navigate to **RDS** > **Create Database**.
3. Select PostgreSQL as the database engine.
4. Configure the database:
   - **Instance Name**: Choose a unique name.
   - **Username**: `admin`
   - **Password**: `securepassword`
5. Copy the **RDS Instance ARN** for later use.

### 4. Set Up IAM Roles 🔐
1. Navigate to the **IAM** section in AWS.
2. Create a role with `AmazonRDSFullAccess` permissions.
3. Attach the role to your RDS instance.

### 5. Configure AWS CLI ⚙️
```bash
aws configure
```
- Input your access key, secret key, region, and output format.

### 6. Update the Script ✏️
Replace the placeholder `***` with your RDS **Instance ARN** in the script.

### 7. Connect to RDS Using DBeaver 🌐
1. Download and install **DBeaver** [here](https://dbeaver.io/).
2. Create a new PostgreSQL connection:
   - Host: `<RDS Endpoint>`
   - Port: `5432`
   - Database: `postgres`
   - Username: `postgres`
   - Password: `postgres`
3. Verify the connection.

### 8. Run the Script 🚀
1. Open the `app.ipynb` notebook.
2. Execute the cells to process and store transaction data.

### 9. Set Up Grafana for Visualization 📊
1. Sign up for a **Grafana** account [here](https://grafana.com/).
2. Add your PostgreSQL data source:
   - Host: `<RDS Endpoint>`
   - Database: `postgres`
   - User: `admin`
   - Password: `securepassword`
3. Create visualizations:
   - Use queries from `app.ipynb` or pre-defined SQL scripts.
   - Explore dashboards with pie charts, bar graphs, and heatmaps.

### 10. View Dashboards and Monitor 🌟
- Access Grafana to explore transaction trends and anomalies.

---

## Folder Structure 📂
```plaintext
.
│── .git/
├── .gitignore
├── app.ipynb
├── requirements.txt
├── Visualization_images/
│   ├── chart1.png
│   ├── chart2.png
│   └── chart2.png

```

---

## Visualizations 🖼️
Check out some of the amazing visualizations:

![Sample Chart](https://github.com/ArpitKadam/graphana-visualization-banking-project/blob/main/Visualization_images/screencapture-arpitkadam-grafana-net-d-de8s5bcvp7saod-banking-data-visualization-2025-01-02-19_34_22.png)

---

## Contributing 🤝
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Open a pull request.

---

## License 📜
This project is licensed under the MIT License.

---

## Contact ✉️
For any queries, feel free to reach out to [arpitkadam922@gmail.com](arpitkadam922@gmail.com).

Enjoy building your dashboard! 🎉

