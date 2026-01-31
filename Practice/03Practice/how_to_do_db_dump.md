### DB dump

**A DB dump** (_database dump_) is a full exported copy of a database’s structure and/or data, saved to a file — usually as SQL statements or a binary archive — so it can be restored later.
Think of it as a database backup in portable form.

Let's practice with [Employees Sample Database](https://dev.mysql.com/doc/employee/en/).

General Installation [instructions](https://dev.mysql.com/doc/employee/en/).

``````
# 1. Install git (if not already installed)
sudo apt update
sudo apt install git -y

# 2. Clone the repository from GitHub
git clone https://github.com/datacharmer/test_db.git

# 3. Change into the dataset directory
cd test_db

# Load the main employees database into MySQL
mysql -u root -p < employees.sql
``````

#### Windows
https://dev.mysql.com/downloads/mysql/

Do dump
``````
# PowerShell


setx PATH "$env:PATH;C:\Program Files\MySQL\MySQL Server 8.0\bin"

# Restart PowerShell, then verify:

mysql --version

https://git-scm.com/download/win

git clone https://github.com/datacharmer/test_db.git
cd test_db

mysql -u root -p < employees.sql

# PowerShell sometimes blocks input redirection. Use this instead:

`cmd /c "mysql -u root -p < employees.sql"`
``````