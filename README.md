# Code extensions install
Runs code --code-extensions on list of extensions in vscode.extensions.txt

# Manual installation
``` PowerShell
$extensions = (Get-Content .\vscode.extensions.txt) # Enumerates Extensions to install
$extensions |  Foreach-Object { code --install-extension $_ } # Run code install for each extensions
```