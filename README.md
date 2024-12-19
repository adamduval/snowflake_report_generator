# 📊 Snowflake Automated PDF Report Generator 📊

The **Snowflake Automated PDF Report Generator** is a proof-of-concept project designed to showcase the functionality and power of Snowflake Notebooks. This project demonstrates how to create a fully automated reporting pipeline for a fictional company, WidgetCo, using only Snowflake Notebook features.

The result? A dynamic, daily PDF report of sales performance for three product lines (A, B, and C), personalized for three different managers. These reports are sent automatically via email and archived for future reference.

{{placeholder for demo video}}

## 🔧 Key Features

- **Dynamic PDF Report Generation:**
  - Generate PDF reports for product lines A, B, and C.
  - Custom data tailored for each manager.

- **Email Failure Alerts:**
  - Automatic email notifications in case of report generation or delivery failures.
 
    {{placeholder for alert image}}

- **Customizable Dynamic Emails:**
  - Each manager receives a personalized email with their respective report.

  {{placeholder for report images}}

- **Visualize Reports During Development:**
  - View the report directly within the notebook environment without needing to save it to a stage.

  {{placeholder for notebook image with report}}

- **Archive Management:**
  - All PDF reports are securely archived to an internal stage for easy future reference.

  {{placeholder for stage folders image}}

- **Simplified Workflow Management:**
  - A single orchestrating notebook handles the entire process, supporting both ad-hoc runs and scheduled automation.

  {{placeholder for failure image}}

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
