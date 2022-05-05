# Upload document collections

## NormalLogin-UpdloadDocs

This collection uses the authentication with Normal Login (based on OAuth2.0 Implicit flow).

This collection has collection variables that need to be completed. You should complete the variables with the values provided by Taiger.

### Required parameters

This parameter should be configured in Collection Variables. Use Initial Value column to set them.

| Parameter | Description | Example |
| ----------- | ----------- | ----------- |
| uua_url     | URL of the Authentication and Authorization service | https://[server]/api/kcp |
| idp_url     | URL of IDP extraction engine service | https://[server]/api/idp/extraction-engine |
| user_name   | A user name registered on the system | N/A |
| password    | Password related with the user_name  | N/A |
| organization | Unique organization identifier. It should be a UUID. The user should have permission over this organization | 2e0d9c91-bc82-4557-9c8c-08a5434f71f3 |
| project_uuid | Unique project identifier. The user should have permission over this project. It should be a UUID | 841b2f1c-cc50-11ec-9d64-0242ac120002 |

Furthermore, you need to select the file to upload. Please go to **Upload Document** step, select the body tab and you can find a field in the form-data called file. Please select the file to upload. **Please,don't forget to SAVE the changes**

**IMPORTANT NOTE:** Postman could have rights issues with the folder which contains the selected file. Please, we recommend placing it in Postman working directory. You can consult it General tab in Postman settings.

## NewLogin-UploadDocs

This collection uses the authentication with New Login (based on OAuth2.0 Authorization Code Grant flow).

This collection has collection variables that need to be completed. You should complete the variables with the values provided by Taiger.

### Required parameters

This parameter should be configured in Collection Variables. Use Initial Value column to set them.

| Parameter | Description | Example |
| ----------- | ----------- | ----------- |
| uua_url     | URL of the Authentication and Authorization service | https://[server]/api/kcp |
| idp_url     | URL of IDP extraction engine service | https://[server]/api/idp/extraction-engine |
| organization | Unique organization identifier. It should be a UUID. The user should have permission over this organization | 2e0d9c91-bc82-4557-9c8c-08a5434f71f3 |
| clientId | Idenfier of the client to identify the authentication source | omnitive |
| spaState | Random string to be related with the login attemp | qwerty |
| user_name   | A user name registered on the system | N/A |
| password    | Password related with the user_name  | N/A |
| project_uuid | Unique project identifier. The user should have permission over this project. It should be a UUID | 841b2f1c-cc50-11ec-9d64-0242ac120002 |


Furthermore, you need to select the file to upload. Please go to **Upload Document** step, select the body tab and you can find a field in the form-data called file. Please select the file to upload. **Please,don't forget to SAVE the changes**

**IMPORTANT NOTE:** Postman could have rights issues with the folder which contains the selected file. Please, we recommend placing it in Postman working directory. You can consult it General tab in Postman settings.
