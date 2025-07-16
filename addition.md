There are two types of version control system 

🔸 Centralized Version Control System (CVCS)
📌 Definition:
In a centralized system, there is one central server that stores all the versioned files, and all developers connect to that server to get or push their changes.

🧠 Think of it like:
👉 A shared Google Drive where everyone works on the same documents directly.

✅ Features:
There's only one central repository

Everyone pulls from and pushes to that central server

Internet connection is usually required to do version control operations

Example: Subversion (SVN), Perforce

❌ Problems:
If the server crashes, everyone loses access

You can't commit changes offline

Risk of bottlenecks

🔹 Distributed Version Control System (DVCS)
📌 Definition:
In a distributed system, every developer has a full copy of the entire repository (including history). They can work offline, commit locally, and later push to a central remote like GitHub.

🧠 Think of it like:
👉 Everyone has their own personal Google Drive clone, and they sync it with the team whenever needed.

✅ Features:
Every user has a local repo + full history

You can commit, view logs, branch even offline

Much safer: if the main server is lost, you can restore from any team member’s copy

Faster operations

Examples: Git, Mercurial