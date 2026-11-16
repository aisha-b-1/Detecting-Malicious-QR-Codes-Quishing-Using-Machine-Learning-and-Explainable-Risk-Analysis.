QRGuard Project Log
12/11/2026
Reviewed brief, project definition feedback and supervisor email
Plan: basic web app by December, ML and organisation verification from January

14/11/2026
Installed Python 3.14.2, Git, VS Code; cloned repo
Created venv; installed Flask, OpenCV, tldextract, RapidFuzz, pytest
Problem: venv blocked by PowerShell → fixed with Set-ExecutionPolicy
Decisions: Python 3.14, Flask instead of FastAPI

15/11/2026
Wrote requirements draft v0.1; created docs folder

16/11/2026
Requirements v0.2 and entity list completed
Problem: git push rejected → fixed with git pull --rebase
Decision: scans never stored, only reference data (privacy)
Next: Flask skeleton