--- 

title: USER REST API 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

USER REST API 

**Version:** 0.0.1 

# /AUTH/LOGIN
## ***POST*** 

**Summary:** login

### HTTP Request 
`***POST*** /auth/login` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| authRequest | body | authRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /BUSINESS/SERVICE/CHANGE
## ***POST*** 

**Summary:** changeBusinessService

### HTTP Request 
`***POST*** /business/service/change` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| changeBusinessServiceRequest | body | changeBusinessServiceRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /BUSINESS/SERVICE/USER
## ***POST*** 

**Summary:** getBusinessServiceListByUser

### HTTP Request 
`***POST*** /business/service/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| businessServiceByUserRequest | body | businessServiceByUserRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /CLIENT
## ***POST*** 

**Summary:** createUserClient

### HTTP Request 
`***POST*** /client` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| requestFromUserClient | body | requestFromUserClient | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /CLIENT/ROLE
## ***POST*** 

**Summary:** createUserClient

### HTTP Request 
`***POST*** /client/role` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| requestFromUserClientRole | body | requestFromUserClientRole | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /EMAIL
## ***POST*** 

**Summary:** mail

### HTTP Request 
`***POST*** /email` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| emailRequest | body | emailRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /INVITATION
## ***POST*** 

**Summary:** inviteMember

### HTTP Request 
`***POST*** /invitation` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| invitationRequest | body | invitationRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /INVITEE-CONFIRMATION
## ***POST*** 

**Summary:** inviteeConfirmation

### HTTP Request 
`***POST*** /invitee-confirmation` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| inviteeConfirmationRequest | body | inviteeConfirmationRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /INVITEE-REGISTRATION
## ***POST*** 

**Summary:** inviteeRegistration

### HTTP Request 
`***POST*** /invitee-registration` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| inviteeRegisterRequest | body | inviteeRegisterRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /KAFKA/BUSINESS
## ***POST*** 

**Summary:** createBusinessKafka

### HTTP Request 
`***POST*** /kafka/business` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| kafkaBusinessServiceRequest | body | kafkaBusinessServiceRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /KAFKA/BUSINESS/SERVICE
## ***POST*** 

**Summary:** createBusinessServiceKafka

### HTTP Request 
`***POST*** /kafka/business/service` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| kafkaBusinessServiceRequest | body | kafkaBusinessServiceRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /MENU/CHANGE
## ***POST*** 

**Summary:** changeMenu

### HTTP Request 
`***POST*** /menu/change` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| menuChangeRequest | body | menuChangeRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PASSWORD
## ***POST*** 

**Summary:** password

### HTTP Request 
`***POST*** /password` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| passwordRequest | body | passwordRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PASSWORD/VERIFY
## ***POST*** 

**Summary:** passwordVerify

### HTTP Request 
`***POST*** /password/verify` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| passwordVerifyRequest | body | passwordVerifyRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /REGISTRATION
## ***POST*** 

**Summary:** register

### HTTP Request 
`***POST*** /registration` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| registerRequest | body | registerRequest | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /ROLE
## ***POST*** 

**Summary:** createRole

### HTTP Request 
`***POST*** /role` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| requestFromRole | body | requestFromRole | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /ROLES
## ***POST*** 

**Summary:** getAllRolesAndId

### HTTP Request 
`***POST*** /roles` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| requestGetRoles | body | requestGetRoles | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERCONFIG
## ***POST*** 

**Summary:** createUserConfig

### HTTP Request 
`***POST*** /userconfig` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| requestFromUserConfig | body | requestFromUserConfig | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
