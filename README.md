# 📊 Snowflake Automated PDF Report Generator 📊

The **Snowflake Automated PDF Report Generator** is a **proof-of-concept project** designed to showcase the **functionality** and **power** of **Snowflake Notebooks**. This project demonstrates how to create a fully **automated reporting pipeline** for a fictional company, **WidgetCo**, using only **Snowflake Notebook features**.

The result? A **dynamic, daily PDF report** of **sales performance** for three product lines (**A, B, and C**), personalized for three different managers. These reports are sent automatically via **email** with **failure altering** and **archived for future reference**.


https://github.com/user-attachments/assets/82e1c99c-a5b8-4a6c-967f-9b8965a58f10

## 🔧 Key Features

- **Dynamic PDF Report Generation:**
  - Generate PDF reports for product lines A, B, and C.
  - Custom data tailored for each manager.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d4057c0c-a6c4-4d00-be3a-9c079fcf37f9" alt="a-report" width="250"/>
  <img src="https://github.com/user-attachments/assets/a7840e76-a568-4b48-864d-8c8e0e0de551" alt="b-report" width="250"/>
  <img src="https://github.com/user-attachments/assets/7d0ddca8-c6da-41bb-8e83-3558f9815dd8" alt="c-report" width="250"/>
</p>

- **Email Failure Alerts:**
  - Automatic email notifications in case of report generation or delivery failures.
 
    ![email-warning](https://github.com/user-attachments/assets/d7b3bab4-b21f-4787-9da6-1bbc8ddf0301)

- **Customizable Dynamic Emails:**
  - Each manager receives a personalized email with their respective report.

  ![email-inbox](https://github.com/user-attachments/assets/147dc1f2-707e-4a83-8515-367768585c8e)

- **Visualize Reports During Development:**
  - View the report directly within the notebook environment without needing to save it to a stage.

  ![dark-report-in-nb](https://github.com/user-attachments/assets/5b776e32-e7ce-40d3-9fab-1dc803497914)

- **Archive Management:**
  - All PDF reports are securely archived to an internal stage for easy future reference.

  ![stage-main](https://github.com/user-attachments/assets/497eead9-d850-4355-88cb-ce82eebead3d)
  ![stage-a](https://github.com/user-attachments/assets/8e054d94-2a86-4fe7-942a-e112f38dd753)

- **Simplified Workflow Management:**
  - A single orchestration notebook handles the entire process, supporting both ad-hoc runs and scheduled automation.

---

## 🏗️ Requirements

- A Snowflake account with access to Snowflake Notebooks.

---

## ⚖️ Step-by-Step Walkthrough

### 1. Setup
1. Copy all the notebooks provided into your Snowflake environment.

### 2. Data Engineering
- Run the `_00_REPORT_GEN__ENG` notebook to prepare the data for the project.
  - This notebook generates a sales fact table with randomized sales data for three fictional widgets.
  - It also creates a stage to store the generated PDF reports.

### 3. Report Development
- Run the `01_REPORT_GEN__REPORT` notebook to view and test the demo report.
  - Customize the report as needed.
  - Preview the report as a JPG directly within the notebook.

### 4. Email Integration Setup
- Run the `_02_REPORT_GEN__EMAIL_CONFIG` notebook to configure email integration.
  - Update the notebook with your email addresses.

### 5. Email Development
- Run the `_03_REPORT_GEN__SEND_EMAIL` notebook to preview email content.
  - Note: Email formatting preview may have limitations due to Streamlit.

### 6. Automate Report Generation and Delivery
- Run the `_04_REPORT_GEN__PIPELINE` notebook to generate and send the reports.
  - Schedule this notebook for daily execution to automate the reporting process.

---

## 🚀 Reach out if you have any questions or want to chat about the project. I'd love to hear your thoughts!
