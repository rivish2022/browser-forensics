rowser Forensic Artifact Analysis
📌 About This Project
This project demonstrates basic digital forensics skills by analyzing Google Chrome browser artifacts. The goal was to extract and examine browsing history, downloads, search queries, and other artifacts to reconstruct user activity. It showcases foundational DFIR (Digital Forensics and Incident Response) techniques using both manual and automated tools.

🛠️ Tools Used
DB Browser for SQLite – Manual inspection of Chrome's History database.

Hindsight (GUI version) – Automated extraction of browser artifacts and timeline generation.

Google Chrome – Source of browser artifacts.

Windows 10 – Analysis environment.

📂 What I Did
Evidence Acquisition

Closed Chrome completely to unlock database files.

Located Chrome profile folder:
%LOCALAPPDATA%\Google\Chrome\User Data\Default

Copied History file to preserve original evidence.

Manual Analysis (DB Browser for SQLite)

Opened History file in DB Browser.

Examined urls table for URLs, titles, visit counts, and timestamps.

Automated Analysis (Hindsight GUI)

Ran hindsight-gui.exe and accessed web interface at http://localhost:8080.

Entered Chrome profile path and ran analysis.

Reviewed summary of extracted artifacts.

Timeline Reconstruction

Compared manual and automated findings.

Identified browsing patterns and frequently visited sites (e.g., YouTube, Netflix, university portals).

📊 Key Findings
Artifact Type	Count
URL records	18,182
Download records	650
Google search queries	6,790
Bookmarks	182
Autofill entries	578
Saved login credentials	82
Installed extensions	3
Note: Some artifacts (cookies, cache) showed as "Failed" in Hindsight – this is normal due to file locks and does not affect overall analysis.

📁 Files in This Repository
Browser_Forensics_Report.pdf – Full forensic analysis report.

db browser/ – Folder containing evidence screenshots


💡 Skills Demonstrated
Digital evidence acquisition

Browser artifact analysis (history, downloads, searches, bookmarks)

Use of forensic tools (DB Browser, Hindsight)

Forensic reporting and documentation

📬 Contact
Author: S.M.A.D.R.Pabasarani
Date: 08 March 2026
Connect: https://www.linkedin.com/in/rivishka-pabasarani/
