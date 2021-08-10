## **My environment configs**
-----------------------------

### **First i get my terminals, because terminal is all**

  - Get Windows Terminal from Microsoft Store

  - Get PowerShell 7 (or the newest)

### **Now let's configure them**

  In a high privilegies session excecute the commands bellow

  - Freeing script execution policy
  ```powershell
  # All users
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned

  # Current user only
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```
  
  - Installing nuget provider

  ```powershell
  Install-PackageProvider -Name NuGet -Force
  ```

  - Installing powershell get

  ```powershell
  Install-Module -Name PowerShellGet -Force
  ```

  - Updating powershell get
  ```powershell
  Update-Module -Name PowerShellGet
  ```

### **Getting the extra modules**

  - Installing posh-git
  ```powershell
  Install-Module posh-git -Scope CurrentUser
  ```
  - Installing oh-my-posh
  ```powershell
  Install-Module oh-my-posh -RequiredVersion 2.0.496 -Force -Scope CurrentUser
  ```