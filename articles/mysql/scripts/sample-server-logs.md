---
title: CLI script - Download slow query logs - Azure Database for MySQL
description: This sample Azure CLI script shows how to enable and download the server logs of an Azure Database for MySQL server.
author: savjani
ms.author: pariks
ms.service: mysql
ms.devlang: azurecli
ms.topic: sample
ms.custom: mvc, devx-track-azurecli
ms.date: 02/10/2022
---

# Enable and download server slow query logs of an Azure Database for MySQL server using Azure CLI

[[!INCLUDE[applies-to-mysql-single-flexible-server](../includes/applies-to-mysql-single-flexible-server.md)]

This sample CLI script enables and downloads the slow query logs of a single Azure Database for MySQL server.

[!INCLUDE [quickstarts-free-trial-note](../../../includes/quickstarts-free-trial-note.md)]

[!INCLUDE [azure-cli-prepare-your-environment.md](../../../includes/azure-cli-prepare-your-environment.md)]

## Sample script

[!INCLUDE [cli-launch-cloud-shell-sign-in.md](../../../includes/cli-launch-cloud-shell-sign-in.md)]

### Run the script

:::code language="azurecli" source="~/azure_cli_scripts/mysql/server-logs/server-logs.sh" range="4-49":::

## Clean up resources

[!INCLUDE [cli-clean-up-resources.md](../../../includes/cli-clean-up-resources.md)]

```azurecli
az group delete --name $resourceGroup
```

## Sample reference

This script uses the commands outlined in the following table:

| **Command** | **Notes** |
|---|---|
| [az group create](/cli/azure/group#az_group_create) | Creates a resource group in which all resources are stored. |
| [az mysql server create](/cli/azure/mysql/server#az_mysql_server_create) | Creates a MySQL server that hosts the databases. |
| [az mysql server configuration list](/cli/azure/mysql/server/configuration#az_mysql_server_configuration_list) | List the configuration values for a server. |
| [az mysql server configuration set](/cli/azure/mysql/server/configuration#az_mysql_server_configuration_set) | Update the configuration of a server. |
| [az mysql server-logs list](/cli/azure/mysql/server-logs#az_mysql_server_logs_list) | List log files for a server. |
| [az mysql server-logs download](/cli/azure/mysql/server-logs#az_mysql_server_logs_download) | Download log files. |
| [az group delete](/cli/azure/group#az_group_delete) | Deletes a resource group including all nested resources. |

## Next steps

- Read more information on the Azure CLI: [Azure CLI documentation](/cli/azure).
- Try additional scripts: [Azure CLI samples for Azure Database for MySQL](../sample-scripts-azure-cli.md)
