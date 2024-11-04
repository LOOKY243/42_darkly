This vulnerability is called "Directory Traversal" which allows the attacker to access restricted directories and files inside the host machine, it is caused by an inproper input validation, it can be exploited by using a series of "../" (dot dot slash) inside the url accesing a file or a page, attackers will often target files like /etc/passwd with this method, for example: http://<URL>/index.html?page=../../../../../etc/passwd

Solution

Proper input validation
Check and restrict the use of special characters/patterns
implement an allowlist for certain paths