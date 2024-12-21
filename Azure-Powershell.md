Azure PowerShell is a set of cmdlets for managing Azure resources directly from PowerShell. Below is a categorized list of commonly used Azure PowerShell commands:

---

### **General Azure Management**
| **Command** | **Description** |
|-------------|-----------------|
| `Connect-AzAccount` | Sign in to your Azure account. |
| `Get-AzSubscription` | List all subscriptions in your account. |
| `Set-AzContext` | Set the current subscription or context. |
| `Get-AzEnvironment` | Get Azure environments (e.g., AzureCloud, AzureChinaCloud). |

---

### **Resource Management**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzResource` | Get resources in the current subscription. |
| `New-AzResource` | Create a new Azure resource. |
| `Remove-AzResource` | Delete a resource. |
| `Get-AzResourceGroup` | Get details of resource groups. |
| `New-AzResourceGroup` | Create a new resource group. |
| `Remove-AzResourceGroup` | Delete a resource group. |

---

### **Virtual Machines (VMs)**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzVM` | Get details of Azure virtual machines. |
| `New-AzVM` | Create a new virtual machine. |
| `Start-AzVM` | Start a virtual machine. |
| `Stop-AzVM` | Stop (deallocate) a virtual machine. |
| `Restart-AzVM` | Restart a virtual machine. |
| `Remove-AzVM` | Delete a virtual machine. |

---

### **Azure Storage**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzStorageAccount` | List Azure storage accounts. |
| `New-AzStorageAccount` | Create a new storage account. |
| `Remove-AzStorageAccount` | Delete a storage account. |
| `Get-AzStorageBlob` | Get details of blobs in a container. |
| `Set-AzStorageBlobContent` | Upload a file to a blob container. |
| `Get-AzStorageBlobContent` | Download a blob to a file. |

---

### **Azure Networking**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzVirtualNetwork` | Get details of virtual networks. |
| `New-AzVirtualNetwork` | Create a new virtual network. |
| `Remove-AzVirtualNetwork` | Delete a virtual network. |
| `Get-AzPublicIpAddress` | List public IP addresses. |
| `New-AzPublicIpAddress` | Create a public IP address. |
| `Get-AzNetworkSecurityGroup` | Get details of NSGs (Network Security Groups). |
| `New-AzNetworkSecurityGroup` | Create a new NSG. |

---

### **Azure App Services**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzWebApp` | Get details of web apps. |
| `New-AzWebApp` | Create a new web app. |
| `Remove-AzWebApp` | Delete a web app. |
| `Start-AzWebApp` | Start a web app. |
| `Stop-AzWebApp` | Stop a web app. |

---

### **Azure Kubernetes Service (AKS)**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzAksCluster` | Get details of AKS clusters. |
| `New-AzAksCluster` | Create a new AKS cluster. |
| `Remove-AzAksCluster` | Delete an AKS cluster. |
| `Get-AzAksNodePool` | Get details of node pools in an AKS cluster. |
| `Set-AzAksNodePool` | Update a node pool in an AKS cluster. |

---

### **Azure SQL**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzSqlServer` | Get details of SQL servers. |
| `New-AzSqlServer` | Create a new SQL server. |
| `Remove-AzSqlServer` | Delete a SQL server. |
| `Get-AzSqlDatabase` | Get details of SQL databases. |
| `New-AzSqlDatabase` | Create a new SQL database. |
| `Remove-AzSqlDatabase` | Delete a SQL database. |

---

### **Azure Functions**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzFunctionApp` | Get details of Azure Functions. |
| `New-AzFunctionApp` | Create a new Azure Function App. |
| `Remove-AzFunctionApp` | Delete a Function App. |
| `Start-AzFunctionApp` | Start a Function App. |
| `Stop-AzFunctionApp` | Stop a Function App. |

---

### **Azure Monitor**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzLog` | Retrieve Azure activity logs. |
| `Get-AzMetric` | Retrieve Azure metrics for resources. |
| `Set-AzDiagnosticSetting` | Enable diagnostic settings for a resource. |

---

### **Azure Identity and Access Management (IAM)**
| **Command** | **Description** |
|-------------|-----------------|
| `Get-AzRoleAssignment` | List role assignments. |
| `New-AzRoleAssignment` | Assign a role to a user or group. |
| `Remove-AzRoleAssignment` | Remove a role assignment. |
| `Get-AzADUser` | Get details of Azure AD users. |

---

### **Automation Tips**
1. **Search for Cmdlets**: Use the following command to find available cmdlets:
   ```powershell
   Get-Command -Module Az.*
   ```

2. **Get Help for a Cmdlet**:
   ```powershell
   Get-Help <cmdlet-name> -Full
   ```
   Example:
   ```powershell
   Get-Help New-AzResourceGroup -Full
   ```

3. **Install Azure PowerShell**:
   Install the Azure PowerShell module using:
   ```powershell
   Install-Module -Name Az -AllowClobber -Scope CurrentUser
   ```

---

Let me know if you need practical examples or further assistance!
