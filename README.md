## PowerShell for Cloud Engineers / DevOps

![Image](https://images.openai.com/static-rsc-4/s2CvfJ47QUr4o_EAHgS4SFWseNTG8V8feYjbZyfzEaw_Mkdle6PPM4rkytWlcnBDX99du7pgwYfyTP2V4VleEKJSttNG0YwhmN6LkVLF5NfZP9y8WRsKTYe05rayxhM1dNW6Z9fcCjJfZm1YLPMaoCAeWuWoUuQTJCchBxR7dCy_L5vIhgAFAyUJyPDlyAuX?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/IwEcMg913GC_NEYe29_MB8_DlfD7Y_DaB1HuPo9YqLfGuBxZ624gtzeZShJW3GbgYiN2N5Eyt0oP-bFg7eHmD7P45Kp0qGCq4YmQ3vpRbnP-tVLZQoIZES02iGX7oMvI7FgESoyGjUNb9jqh4GAP9aneC7IMOEKEHpM7J4fSn0A68rZm31SV7AM96Gsgw0FA?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/X05fAiL5fBJTjxtw_m_bEuE4KpvyITjikDLogwA8Y9PCVwP-Ktp1YHaV-ljO72Qwkp1AhF6dq1435N8fsrC1UcnyImTUbO77IofnhweIQxDa0aHoHpN7bNph2fH6BisgFlJmy6MHvlqy5aLr6HSgM0Z-nEDavvJg_1N14CjjHqOvPV-eyAEd3EKpPWE-myV8?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/ejH9xm77udUSPzjeyK-Ve8ypAektFGrvqffVKA4ByyhDFV0Q_pVj_rfetryOJOtkjPe0pu6XncvQoHzEJJCDmRpIs4vRMDC3s9zSEZBey6iCtgxqsuapup81Npy8_07QnKbuXgHJVEEel4AG5X3rbdT-QbsDrSOAYkfvBxX8FieOVdxiw0onlD3IQQuVxKa0?purpose=fullsize)

### What is PowerShell?

PowerShell is a command-line shell and scripting language used for:

* Cloud automation
* Infrastructure management
* DevOps tasks
* CI/CD automation
* Server administration
* API automation
* Azure & AWS resource management

It works on:

* Windows
* Linux
* macOS

---

# Why Cloud Engineers Use PowerShell

### Common Use Cases

| Area             | Example                    |
| ---------------- | -------------------------- |
| Azure Automation | Create VMs, VNets, Storage |
| AWS Automation   | Manage EC2, S3, IAM        |
| DevOps           | CI/CD scripts              |
| Monitoring       | Collect logs and metrics   |
| Infrastructure   | Automate deployments       |
| Security         | User and access management |
| Kubernetes       | AKS/EKS automation         |

---

# Install PowerShell

## Windows

Install from:

[PowerShell Official Website](https://github.com/PowerShell/PowerShell?utm_source=chatgpt.com)

Check version:

```powershell
$PSVersionTable
```

---

# Basic PowerShell Commands

## Variables

```powershell
$name = "Atul"
$age = 30
```

## Print Output

```powershell
Write-Host "Hello World"
```

## Get Date

```powershell
Get-Date
```

## List Files

```powershell
Get-ChildItem
```

Shortcut:

```powershell
ls
dir
```

---

# File Operations

## Create File

```powershell
New-Item test.txt
```

## Read File

```powershell
Get-Content test.txt
```

## Copy File

```powershell
Copy-Item test.txt backup.txt
```

## Delete File

```powershell
Remove-Item test.txt
```

---

# Service Management

## Check Services

```powershell
Get-Service
```

## Restart Service

```powershell
Restart-Service sshd
```

---

# Process Management

## Check Running Processes

```powershell
Get-Process
```

## Kill Process

```powershell
Stop-Process -Name chrome
```

---

# Networking Commands

## Check IP

```powershell
ipconfig
```

## DNS Lookup

```powershell
nslookup google.com
```

## Test Connectivity

```powershell
Test-NetConnection google.com -Port 443
```

---

# Loops and Conditions

## IF Condition

```powershell
$num = 10

if ($num -gt 5) {
    Write-Host "Greater"
}
```

## FOR Loop

```powershell
for ($i=1; $i -le 5; $i++) {
    Write-Host $i
}
```

## FOREACH

```powershell
$users = "atul","admin","devops"

foreach ($user in $users) {
    Write-Host $user
}
```

---

# PowerShell for Azure

## Install Azure Module

```powershell
Install-Module Az -Force
```

## Login Azure

```powershell
Connect-AzAccount
```

## List Resource Groups

```powershell
Get-AzResourceGroup
```

## Create Resource Group

```powershell
New-AzResourceGroup `
-Name dev-rg `
-Location eastus
```

## Create VM

```powershell
New-AzVm `
-ResourceGroupName dev-rg `
-Name vm1 `
-Location eastus
```

Official docs:

[Azure PowerShell Documentation](https://learn.microsoft.com/powershell/azure/?utm_source=chatgpt.com)

---

# PowerShell for AWS

## Install AWS Tools

```powershell
Install-Module AWS.Tools.Installer -Force
```

## Configure AWS

```powershell
Set-AWSCredential
```

## List EC2 Instances

```powershell
Get-EC2Instance
```

## List S3 Buckets

```powershell
Get-S3Bucket
```

Official docs:

[AWS Tools for PowerShell](https://aws.amazon.com/powershell/?utm_source=chatgpt.com)

---

# PowerShell Script Example for Cloud Monitoring

```powershell
$cpu = Get-Counter '\Processor(_Total)\% Processor Time'

Write-Host "CPU Usage:"
Write-Host $cpu.CounterSamples.CookedValue
```

---

# PowerShell + DevOps

### Used With

* Jenkins
* GitHub Actions
* Azure DevOps
* Terraform
* Docker
* Kubernetes

---

# Important PowerShell Operators

| Operator  | Meaning       |
| --------- | ------------- |
| -eq       | Equal         |
| -ne       | Not Equal     |
| -gt       | Greater Than  |
| -lt       | Less Than     |
| -like     | Pattern Match |
| -contains | Contains      |

Example:

```powershell
if ($name -eq "Atul") {
    Write-Host "Valid User"
}
```

---

# Execution Policy

Check policy:

```powershell
Get-ExecutionPolicy
```

Allow scripts:

```powershell
Set-ExecutionPolicy RemoteSigned
```

---

# Real-Time Cloud Engineer Tasks Using PowerShell

### Daily Activities

* VM health checks
* Disk monitoring
* Azure resource automation
* AWS EC2 automation
* Backup scripts
* Log collection
* User management
* CI/CD deployment automation
* Kubernetes deployment scripting

---

# Best Practices

✅ Use functions
✅ Add comments
✅ Store secrets securely
✅ Use try/catch blocks
✅ Avoid hardcoded passwords
✅ Use modules
✅ Use version control with Git

---

# Learn PowerShell Roadmap

### Beginner

* Variables
* Loops
* Conditions
* File handling

### Intermediate

* Functions
* Modules
* APIs
* JSON handling

### Advanced

* Azure automation
* AWS automation
* CI/CD scripting
* Infrastructure automation
* DSC (Desired State Configuration)

---

# Important Commands Cheat Sheet

```powershell
Get-Help
Get-Command
Get-Process
Get-Service
Get-ChildItem
Get-Content
Test-NetConnection
Invoke-WebRequest
```

---

# Recommended for Your Cloud/DevOps Path

Since you work heavily with:

* Azure
* AWS
* DevOps
* Automation
* Terraform
* Kubernetes

PowerShell is extremely valuable for:

* Azure administration
* Windows server automation
* Hybrid cloud scripting
* CI/CD automation
* Monitoring and reporting
* Infrastructure provisioning
