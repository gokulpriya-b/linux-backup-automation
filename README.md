# Linux Backup Automation

## 📌 Project Overview

This project is a Linux Bash shell script that automates the process of backing up a directory. It compresses the selected directory into a `.tar.gz` archive, appends the current date to the backup filename, and stores the backup in a dedicated `backup/` folder.

This project demonstrates basic Linux automation skills commonly used by DevOps Engineers and Linux System Administrators.

---

## 🚀 Features

* Automates directory backup
* Compresses files using `tar` and `gzip`
* Appends the current date to the backup filename
* Stores backups in a `backup/` directory
* Can be scheduled using `cron` for automatic daily backups

---

## 📁 Project Structure

```text
linux-backup-automation/
│
├── backup.sh
├── README.md
├── .gitignore
├── backup/
│   └── .gitkeep
└── project_data/
    ├── file1.txt
    ├── file2.txt
    └── file3.txt
```

---

## 🛠️ Technologies Used

* Linux (Ubuntu)
* Bash Shell Scripting
* tar
* gzip
* Cron

---

## ▶️ How to Run

### Give execute permission

```bash
chmod +x backup.sh
```

### Run the script

```bash
./backup.sh
```

---

## 📦 Example Output

```text
Backup Completed Successfully!
```

Generated backup file:

```text
backup/project_backup_YYYY-MM-DD.tar.gz
```

---

## 📅 Automate Using Cron

Open the cron editor:

```bash
crontab -e
```

Run the backup every day at 2:00 AM:

```text
0 2 * * * /path/to/linux-backup-automation/backup.sh
```

Replace `/path/to/` with the actual location of your project.

---

## 🎯 Learning Outcomes

* Linux file and directory management
* Bash scripting
* Variables in Shell Script
* Date formatting
* File compression using tar
* Linux automation
* Cron job scheduling

---

## 🔮 Future Improvements

* Accept the source directory as a command-line argument
* Create timestamp-based backups
* Automatically delete backups older than 7 days
* Generate backup logs
* Add email notifications for backup status

---

## 👩‍💻 Author

**B. Gokulpriya**

GitHub: https://github.com/gokulpriya-b
