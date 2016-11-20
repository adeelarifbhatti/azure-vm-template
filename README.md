# azure-vm-template
###For Deploying the resource group run the following command in the powershell.

New-AzureRmResourceGroup -name testdeployment -location "west europe"

### For creating the new deployment under this group, enter following command.

New-AzureRmResourceGroupDeployment -ResourceGroupName testdeployment -TemplateFile "C:\azuredeploy.json" -TemplateParameterFile "c:\azuredeploy.parameter.json"
###### Where files are stored on c:\

###To remove the resource group deployment i.e. azuredeploy(the file name i.e. json file name  would be chosen as deployment), use following command

remove-azurermresourceGroupDeployment -ResourceGroupName testdeployment -name azuredeploy

### To remove the resourceGroup, following command should be used.

remove-Azurermresourcegroup -name testdeployment
