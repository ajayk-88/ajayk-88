# HRMS & Automation Suite

This repository contains a collection of three integrated Python-based projects:

1. **HRMS (Human Resource Management System)** – A Django web application for managing employee data, attendance (including shift-based and GPS-based), and leave tracking.
2. **Selenium Automation + SMTP Mailing** – A Python automation script for browser-based tasks (like data scraping or form submissions) and email notifications using SMTP.
3. **Invoice Detection using YOLOv5** – A deep learning model implementation to detect invoice fields and extract structured data from invoice images.

---

## 🔧 Tech Stack

- **Backend:** Python, Django
- **Frontend:** HTML, Tailwind CSS (in HRMS)
- **Automation:** Selenium, SMTP, ChromeDriver
- **Object Detection:** YOLOv5, OpenCV, PyTorch
- **Database:** SQLite / PostgreSQL (optional)
- **Others:** WSL (Ubuntu), virtualenv, Git

---

## 🚀 Features

### HRMS Module
- Employee management (Add/Edit/Delete)
- Shift-based and GPS-based attendance
- QR code and form-based attendance
- Leave tracking and approval
- Attendance reports with short-hours & late detection

### Selenium + SMTP Script
- Browser automation using Selenium WebDriver
- ChromeDriver path auto-setup using environment config
- Email reports sent automatically via SMTP (Gmail or company mail)

### Invoice Detection (YOLOv5)
- Detects invoice fields like invoice number, date, total amount, etc.
- Pre-trained YOLOv5 model integration
- Outputs bounding boxes with extracted text

---

## 📷 Screenshots / Demos

*(Add images or links here if available)*

---

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# For Django app
cd hrms_project
python manage.py migrate
python manage.py runserver

# For Selenium Script
cd automation_script
python automation.py

# For YOLOv5
cd invoice_detection
# Follow YOLOv5 setup instructions (weights, requirements etc.)
