---
title: "Working with Files and Storage using Aspose.CAD Cloud"
type: docs
url: /working-with-files-and-storage-using-aspose-cad-cloud/
weight: 60
---

## **Introduction**
Aspose.CAD Cloud provides helper functions to work with files uploaded to Aspose.CAD Cloud Storage or any other Cloud Storage of your choice. If you need any help getting started with setting third party storage please refer to [How to Configure 3rd Party Cloud Storages](https://docs.aspose.cloud/total/getting-started/dashboard/how-to-configure-3rd-party-cloud-storages/).
### **Download a file from Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|GET|Download a File from Storage|[DownloadFile](https://apireference.aspose.cloud/cad/#/File/DownloadFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="1" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=78946fb4-3bd4-4d3e-b309-f9e2ff9ac6f9&client_secret=b125f13bf6b76ed81ee990142d841195" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"

```

```java

curl  -v -X GET "https://api.aspose.cloud/v3.0/cad/storage/file/presentation_images.dxf" -H "Content-Type: application/json" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYmYiOjE1NjAwOTI3OTcsImV4cCI6MTU2MDE3OTE5NywiaXNzIjoiaHR0cHM6Ly9hcGkuYXNwb3NlLmNsb3VkIiwiYXVkIjpbImh0dHBzOi8vYXBpLmFzcG9zZS5jbG91ZC9yZXNvdXJjZXMiLCJhcGkucGxhdGZvcm0iLCJhcGkucHJvZHVjdHMiXSwiY2xpZW50X2lkIjoiNzg5NDZmYjQtM2JkNC00ZDNlLWIzMDktZjllMmZmOWFjNmY5Iiwic2NvcGUiOlsiYXBpLnBsYXRmb3JtIiwiYXBpLnByb2R1Y3RzIl19.rFS4KehYAg1yOVGmteeinIh-AFq7nVEmtUr_cDltIfk0iN0JJJ3o6TK1StpnItAAqlkb_QtF0WcY5D8NCjeyTVKL1oewdIshjjODoPEN1tmCsRXceHGYTG5f--B8sWrMuZtOqSzlbr-x3_Mat9Fy7xcNbS6nNNmBv7mo3suRDF4xdUZWdIY7bO6yBptc-qyhIFb0olNMxdeAZPsN8sPLW0XIbEGf8CaE16p9al_O5SjWLtEZT7APuvDesJwWYOSPtG6hCsXtHItphKDAcMULEnqJ-QW_QpzBxybTnQ1VNzundQWOYM_viYzU8hOlf6VTE4YQKyCmgz72Ena8KZx0VA" --ssl-no-revoke

```

{{< /tab >}}

{{< /tabs >}}
### **Uploading a file from Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|PUT|Upload a file to Cloud Storage|[UploadFile](https://apireference.aspose.cloud/cad/#/File/UploadFile)|
#### **cURL Example**
{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=78946fb4-3bd4-4d3e-b309-f9e2ff9ac6f9&client_secret=b125f13bf6b76ed81ee990142d841195" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"

```

```java

curl  -v -X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/presentation_images_1.dxf" -H "Content-Type:application/octet-stream" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYmYiOjE1NjAwOTI3OTcsImV4cCI6MTU2MDE3OTE5NywiaXNzIjoiaHR0cHM6Ly9hcGkuYXNwb3NlLmNsb3VkIiwiYXVkIjpbImh0dHBzOi8vYXBpLmFzcG9zZS5jbG91ZC9yZXNvdXJjZXMiLCJhcGkucGxhdGZvcm0iLCJhcGkucHJvZHVjdHMiXSwiY2xpZW50X2lkIjoiNzg5NDZmYjQtM2JkNC00ZDNlLWIzMDktZjllMmZmOWFjNmY5Iiwic2NvcGUiOlsiYXBpLnBsYXRmb3JtIiwiYXBpLnByb2R1Y3RzIl19.rFS4KehYAg1yOVGmteeinIh-AFq7nVEmtUr_cDltIfk0iN0JJJ3o6TK1StpnItAAqlkb_QtF0WcY5D8NCjeyTVKL1oewdIshjjODoPEN1tmCsRXceHGYTG5f--B8sWrMuZtOqSzlbr-x3_Mat9Fy7xcNbS6nNNmBv7mo3suRDF4xdUZWdIY7bO6yBptc-qyhIFb0olNMxdeAZPsN8sPLW0XIbEGf8CaE16p9al_O5SjWLtEZT7APuvDesJwWYOSPtG6hCsXtHItphKDAcMULEnqJ-QW_QpzBxybTnQ1VNzundQWOYM_viYzU8hOlf6VTE4YQKyCmgz72Ena8KZx0VA" --ssl-no-revoke --data-binary @destination.pptx

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

   "uploaded":[

      "input_1.dxf"

   ],

   "errors":[

   ]

}

```

{{< /tab >}}

{{< /tabs >}}
### **Copying a file to a new location on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/copy/{srcPath}|PUT|Duplicate a file to a new location on Cloud Storage|[CopyFile](https://apireference.aspose.cloud/cad/#/File/CopyFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="8" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=78946fb4-3bd4-4d3e-b309-f9e2ff9ac6f9&client_secret=b125f13bf6b76ed81ee990142d841195" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"

```

```java

curl -v -X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/copy/input.dxf" -H "Content-Type:application/json" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYmYiOjE1NjAxMDY1MDcsImV4cCI6MTU2MDE5MjkwNywiaXNzIjoiaHR0cHM6Ly9hcGkuYXNwb3NlLmNsb3VkIiwiYXVkIjpbImh0dHBzOi8vYXBpLmFzcG9zZS5jbG91ZC9yZXNvdXJjZXMiLCJhcGkucGxhdGZvcm0iLCJhcGkucHJvZHVjdHMiXSwiY2xpZW50X2lkIjoiNzg5NDZmYjQtM2JkNC00ZDNlLWIzMDktZjllMmZmOWFjNmY5Iiwic2NvcGUiOlsiYXBpLnBsYXRmb3JtIiwiYXBpLnByb2R1Y3RzIl19.FeU2K-qTf4meenSv1IQZqUpSPQREk0MmYK5oMMRx2t_LqELHMRnBawHC8nJ5DzGKsK_xyZwPpIANRA8eWHPoPICMoZnDZtUbLagxvSbFMZPReV2Ip3sVTTSvQXA-UOaLC6BbWnyHWDAbAGPv92AFMu_A0wiEBVs68vx_ZOOhjhZkX1rKfJFbJjWr8tJC9HVkEGubfiqXAb6ejL2ISwWcvUr49napuPPVrejJkAbj27z1oGSjmzYvoUuN4tP8Tb2VwD6L4B_Q99EOAs0y4VownW1BE3Ku_rKUgGAOa7OKZKtzOgKrtWqSc9oQ9h0DuiIkmKhn5I_PczHwigZ-ytb3OQ" --ssl-no-revoke -d {}

```

{{< /tab >}}

{{< /tabs >}}
### **Moving a file to a new location on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/MOVE/{srcPath}|PUT|Move a file to a new location on Cloud Storage|[MoveFile](https://apireference.aspose.cloud/cad/#/File/MoveFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="11" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=78946fb4-3bd4-4d3e-b309-f9e2ff9ac6f9&client_secret=b125f13bf6b76ed81ee990142d841195" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"

```

```java

curl -v -X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/move/input.dxf" -H "Content-Type:application/json" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYmYiOjE1NjAxMDY1MDcsImV4cCI6MTU2MDE5MjkwNywiaXNzIjoiaHR0cHM6Ly9hcGkuYXNwb3NlLmNsb3VkIiwiYXVkIjpbImh0dHBzOi8vYXBpLmFzcG9zZS5jbG91ZC9yZXNvdXJjZXMiLCJhcGkucGxhdGZvcm0iLCJhcGkucHJvZHVjdHMiXSwiY2xpZW50X2lkIjoiNzg5NDZmYjQtM2JkNC00ZDNlLWIzMDktZjllMmZmOWFjNmY5Iiwic2NvcGUiOlsiYXBpLnBsYXRmb3JtIiwiYXBpLnByb2R1Y3RzIl19.FeU2K-qTf4meenSv1IQZqUpSPQREk0MmYK5oMMRx2t_LqELHMRnBawHC8nJ5DzGKsK_xyZwPpIANRA8eWHPoPICMoZnDZtUbLagxvSbFMZPReV2Ip3sVTTSvQXA-UOaLC6BbWnyHWDAbAGPv92AFMu_A0wiEBVs68vx_ZOOhjhZkX1rKfJFbJjWr8tJC9HVkEGubfiqXAb6ejL2ISwWcvUr49napuPPVrejJkAbj27z1oGSjmzYvoUuN4tP8Tb2VwD6L4B_Q99EOAs0y4VownW1BE3Ku_rKUgGAOa7OKZKtzOgKrtWqSc9oQ9h0DuiIkmKhn5I_PczHwigZ-ytb3OQ" --ssl-no-revoke -d {}

```

{{< /tab >}}

{{< /tabs >}}
### **Deleting a file on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|DELETE|Delete a file from Cloud Storage|[DeleteFile](https://apireference.aspose.cloud/cad/#/File/DeleteFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="14" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=78946fb4-3bd4-4d3e-b309-f9e2ff9ac6f9&client_secret=b125f13bf6b76ed81ee990142d841195" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"

```

```java

curl -v -X DELETE "https://api.aspose.cloud/v3.0/cad/storage/file/sample.dxf" -H "Content-Type:application/json" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYmYiOjE1NjAxMDY1MDcsImV4cCI6MTU2MDE5MjkwNywiaXNzIjoiaHR0cHM6Ly9hcGkuYXNwb3NlLmNsb3VkIiwiYXVkIjpbImh0dHBzOi8vYXBpLmFzcG9zZS5jbG91ZC9yZXNvdXJjZXMiLCJhcGkucGxhdGZvcm0iLCJhcGkucHJvZHVjdHMiXSwiY2xpZW50X2lkIjoiNzg5NDZmYjQtM2JkNC00ZDNlLWIzMDktZjllMmZmOWFjNmY5Iiwic2NvcGUiOlsiYXBpLnBsYXRmb3JtIiwiYXBpLnByb2R1Y3RzIl19.FeU2K-qTf4meenSv1IQZqUpSPQREk0MmYK5oMMRx2t_LqELHMRnBawHC8nJ5DzGKsK_xyZwPpIANRA8eWHPoPICMoZnDZtUbLagxvSbFMZPReV2Ip3sVTTSvQXA-UOaLC6BbWnyHWDAbAGPv92AFMu_A0wiEBVs68vx_ZOOhjhZkX1rKfJFbJjWr8tJC9HVkEGubfiqXAb6ejL2ISwWcvUr49napuPPVrejJkAbj27z1oGSjmzYvoUuN4tP8Tb2VwD6L4B_Q99EOAs0y4VownW1BE3Ku_rKUgGAOa7OKZKtzOgKrtWqSc9oQ9h0DuiIkmKhn5I_PczHwigZ-ytb3OQ" --ssl-no-revoke -d {}

```

{{< /tab >}}

{{< /tabs >}}
