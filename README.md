# 🔐 Windows File Integrity Monitoring (FIM) + Hash Detection

This project is a lightweight **File Integrity Monitoring (FIM)** tool built using **PowerShell** on Windows. It monitors sensitive files or directories for unauthorized changes by calculating and comparing file **SHA256 hashes**. If a tampering event is detected, it logs the incident and sends a **real-time email alert** to the administrator.

---

## 📌 Features

- ✅ Monitors specified files for unauthorized modifications
- 🔐 Verifies file integrity using SHA256 hashing
- 📝 Logs every scan to a CSV file (`fim_log.csv`)
- 📩 Sends email alerts for hash mismatches
- ⚙️ Can be fully automated with Task Scheduler

---

## 🧰 Technologies Used

- PowerShell (Scripting)
- Send-MailMessage (SMTP Email Alert)
- SHA256 Hashing
- CSV Logging
- Task Scheduler (Automation)

---

## 💡 Use Case

This script is useful for:

- System administrators who need lightweight file change detection
- Cybersecurity students creating blue team tools
- Home lab defenders interested in detection engineering
- Internship and SOP portfolios (shows knowledge of EDR concepts)

---

## 🚀 How It Works

1. Script generates the initial SHA256 hash of the target file(s)
2. On every run, the hash is recalculated and compared
3. If the hash differs, the system:
   - Logs the change to `fim_log.csv`
   - Sends an alert email with a timestamp

---

## ⚠️ Limitations

- Real-time monitoring is not included (uses scheduled scanning)
- Email alerts require app-specific password (for Gmail SMTP)
- Currently supports single files; directory-level scanning can be added

---

## 🔮 Future Improvements

- Add real-time monitoring with `FileSystemWatcher`
- Build a GUI interface (WinForms/WPF or Python Tkinter)
- Extend for directory monitoring and multiple files
- Add webhook integration (e.g., Discord/Slack alerts)

---

## 📄 License

This project is intended for educational and non-commercial use only.

---




