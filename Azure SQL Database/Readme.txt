Before running these templates, first enable the Subnet in the VNet for Service Endpoints for Azure SQL Database. ARM template CreateVnetWithSe.json in the root folder shows how to create a new VNet and a subnet within it, and enables the Service Endpoint feature in it, for Cosmos DB, Azure Storage and to Azure SQL Database.

1) AzureSQLDb_EnableServiceEndpoint.json   - a sample Template that confogures a VNet Service Endpoint on an existing Azure SQL Database. An exisiting VNet and a Azure SQL Database server to be linked, both in the same Azure Region, are a pre-requisite

2) AzureSQLDb_New_WithSe.json - Creates a new Azure SQL Database and configures a Service Endpoint to an existing VNet, in the same region as the latter
Apart from the Service endpoint configuration, this template only enables minimal configuration on the SQL Database Server. You would need to add other features like enabling TDE, Auditing, etc to this template, if required.
(At this point the ARM Template option does not seem to support enabling 'Bypass Azure Services' when setting the firewall rules