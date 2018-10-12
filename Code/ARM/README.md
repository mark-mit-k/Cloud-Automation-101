# ARM

## Installation

[Installation Guide](https://docs.microsoft.com/en-us/powershell/azure/install-azurerm-ps?view=azurermps-6.10.0)

```PowerShell
Install-Module -Name AzureRM -AllowClobber
```

### Login

```PowerShell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```


## Run

Run the `add.json` ARM template to add two parameters. This demonstrate the ARM function functionality. To run the Add-ARM use:

```PowerShell
.\deploy.ps1
# 2
```

Specify the parameters by using a hashmap `@{ first = 1; second = 1}`

```PowerShell
.\deploy.ps1 -TemplateParameterObject = @{ first = 5; second = 6}
# 11
```