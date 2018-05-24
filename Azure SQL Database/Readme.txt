Before running these templates, first enable the Subnet in the VNet for Service Endpoints for Azure Storage. ARM template CreateVnetWithSe.json shows how to create a new VNet and a subnet within it, and enables the Service Endpoint feature in it, for Cosmos DB, Azure Storage and to Azure SQL Database.

1) StorageAccount_EnableServiceEndpoint.json   - a sample Template that confogures a VNet Service Endpoint on an existing Azure Storage Account. An exisiting VNet and a Storage Account to be linked, both in the same Azure Region, are a pre-requisite

2) StorageNewWithSe.json - Creates a new Storage Account and configures a Service Endpoint to an existing VNet, in the same region as the latter