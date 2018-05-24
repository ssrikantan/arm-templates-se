# arm templates - service endpoints enablement
ARM Templates to enable VNet Service end points based access to Azure Resources

CreateVnetWithSe.json  - this ARM Template has to be run first to enable the SE endpoints feature on the target VNet +Subnet that ought to be allowed access to the Azure Services. This template enables for all Service types, i.e. Azure Storage, Cosmos DB and Azure SQL Database
