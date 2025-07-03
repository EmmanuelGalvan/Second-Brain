Links: [[0000 Index|0000 Index]] [[0100 Git and Console]]
Tags: #Code

Creation date: 2025-06-29 02:46
Last update: 2025-06-29 02:46

---
# 0104 Basic Workflow

Files manipulation and stage/commit status

| Comand                         | Explanation                               |
| ------------------------------ | ----------------------------------------- |
| git status                     | Show info about stage status              |
| git add .                      | Add all files to stage status             |
| git add file_name.ext          | Add specified file to stage status        |
| git rm file_name               | Delete specified file from system and git |
| git restore --staged file_name | Removes file from staged status           |
| git restore file_name          | Removes changes in a file                 |
| git mv file_name new_file_name | Changes name                              |
| git status -s                  | Show simplified info about stage status   |
| git commit -m "Comentario"     | Creates a commit with a message.          |

---
Reference: [[Introduction to Git Chap1.pdf]]