# Azurestack-SDK ADFS
Deploy Kubernetes with AKS Engine on Azurestack SDK ADFS version 2301

# SPN
How to create a SPN for the app:

Enter-PSSession -ComputerName AzS-ERCS01 -ConfigurationName PrivilegedEndpoint

New-GraphApplication -Name <appname> -GenerateClientSecret
Output:
give:
--client-id xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx \
--client-secret xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx \


# Follow this howto to deploy the Cluster
https://learn.microsoft.com/en-us/azure-stack/user/azure-stack-kubernetes-aks-engine-deploy-linux?view=azs-2306

# Remember to give the app access to your subscription-id

--subscription-id xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx \