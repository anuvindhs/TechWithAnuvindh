### **D1 - 13.12.24 7:30 PM to 9:00 PM**
**Team Meeting with Anu and Project Teams**

Anu guided us to **register** and **download** essential tools and accounts:
- Visual Studio Code
- Git Account
- Git Software
- AWS Account

Anu then explained **what Git is and how it works**.

---

### **Git Terminology Learnt**

- **Repository:**
  A storage space where project files and version history are tracked using Git.

- **Git:**
  A version control system that tracks changes in code and helps collaborate and manage projects.

- **Commit:**
  A snapshot of changes made to files in a Git repository, similar to saving your work.

- **Pull:**
  Retrieves the latest changes from a remote repository and merges them with the local repository.

- **Branch:**
  A separate line of development in Git. Once work is completed, branches can be merged back.

- **Push:**
  Uploads local commits to a remote repository, such as GitHub, to allow others to access updates.

- **Git Add:**
  Adds specific files or changes to the staging area, preparing for a commit.

![alt text](<Assets/Git repository explaination.png>)

---

### **Practical Steps Followed**

1. **Creating a New Repository on GitHub:**
   - Created a repository named **Lego-city** (Public).
   - Linked Git with Visual Studio Code.

2. **Generating SSH Keys for GitHub:**
   - Open Git Bash and run the following commands:
     ```bash
     $ ssh-keygen -t edxxxxx -C "your_email@example.com"
     ```
     - Private keys are sensitive; do **not** share the content of `id_edxxxxx` or `id_edxxxxx.pub`.

  ![alt text](<Assets/Create SSH key.png>)

   - To verify connection:
     ```bash
     $ ssh -T git@github.com
     ```
     Select "Yes" when prompted.

3. **Adding SSH Key to GitHub:**
   - Open **GitHub Account** > Settings > SSH and GPG Keys.
   - Add the generated public key securely.

---

### **Cloning Repository into Local System**

1. Created a folder named **Lee** on the computer.
2. Opened Git Bash in the folder and cloned the repository:
   ```bash
   $ git clone https://github.com/anuvindhs/TechWithAnuvindh.git

![alt text](<Assets/Cloning into 'TechWithAnuvindh'.png>)