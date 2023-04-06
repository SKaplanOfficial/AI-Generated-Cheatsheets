# Azure Cheatsheet

Azure is a cloud computing platform that provides a wide range of services and tools for building and deploying applications. Here is an overview of some of its basic syntax and features.

## Virtual Machines

### Creating a VM
```
az vm create --resource-group myResourceGroup --name myVM --image UbuntuLTS --admin-username azureuser --generate-ssh-keys
```

### Stopping a VM
```
az vm stop --resource-group myResourceGroup --name myVM
```

### Starting a VM
```
az vm start --resource-group myResourceGroup --name myVM
```

## Storage

### Creating a storage account
```
az storage account create --name mystorageaccount --resource-group myResourceGroup --location eastus --sku Standard_LRS
```

### Uploading a file
```
az storage blob upload --account-name mystorageaccount --account-key myaccountkey --container-name mycontainer --type block --name myblob --source /path/to/local/file
```

### Downloading a file
```
az storage blob download --account-name mystorageaccount --account-key myaccountkey --container-name mycontainer --name myblob --file /path/to/local/file
```

## Functions

### Creating a function
```
az functionapp create --resource-group myResourceGroup --consumption-plan-location eastus --name myFunctionApp --runtime python --storage-account mystorageaccount --functions-version 3 --os-type linux
```

### Invoking a function
```
az functionapp function invoke --resource-group myResourceGroup --name myFunctionApp --function-name myFunction --output json --data '{"key1": "value1", "key2": "value2", "key3": "value3"}'
```

## Resources

- [Azure Documentation](https://docs.microsoft.com/en-us/azure/)
- [Azure CLI Command Reference](https://docs.microsoft.com/en-us/cli/azure/)