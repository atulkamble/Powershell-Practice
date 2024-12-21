# Powershell-Practice

To run PowerShell from a terminal, the steps depend on your operating system and the type of terminal you're using. Below are instructions for common scenarios:

---

### **1. Windows Command Prompt (cmd.exe)**
1. Open Command Prompt.
2. Type the following command and press Enter:
   ```cmd
   powershell
   ```
   This will start a PowerShell session.

3. To run a specific PowerShell command directly:
   ```cmd
   powershell -Command "Write-Host 'Hello from PowerShell'"
   ```

---

### **2. Windows Terminal**
1. Open Windows Terminal.
2. Select the PowerShell profile from the dropdown menu (or add it if not present).
3. Alternatively, run:
   ```bash
   powershell
   ```

---

### **3. From Bash (Linux or macOS Terminal)**
1. Ensure PowerShell (pwsh) is installed. You can install it using [Microsoft's installation guide](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell).
2. Run the following command:
   ```bash
   pwsh
   ```
   This starts a PowerShell session.

3. To execute a specific PowerShell command without starting an interactive session:
   ```bash
   pwsh -Command "Write-Host 'Hello from PowerShell'"
   ```

---

### **4. Using PowerShell Core (Cross-Platform)**
If you're using PowerShell Core (`pwsh`), the steps are the same:
- Start an interactive session:
  ```bash
  pwsh
  ```
- Run a single command:
  ```bash
  pwsh -Command "Get-Process"
  ```

---

### **5. From Visual Studio Code**
1. Open Visual Studio Code.
2. Press `Ctrl+` ` to open the integrated terminal.
3. Select PowerShell as the default shell:
   - Click the dropdown arrow in the terminal tab.
   - Choose "Select Default Profile" > "PowerShell".
4. Run commands directly in the terminal.

---

Let me know if you need help with installation or running specific commands!
