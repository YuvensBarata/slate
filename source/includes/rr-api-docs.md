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

Retention & Referral List of API

Here you can find the list of API which is used by the Retention & Referral Team.
This list will always be updated if there're any changes.

# /AUTH/LOGIN
## ***POST*** 

**Summary:** API for login

```shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/auth/login"
      -H "accept: application/json"
      -H "Content-Type: application/json"
      -d "{ "captcha": \"string\",
            "email": \"string\",
            "password": \"string\"
         }"

```

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

**Summary:** API to change business


``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/business-service/change"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "business_client_id": \"string\",
            "business_service_client_id": \"string\"
         }"

```

### HTTP Request 
`***POST*** /business-service/change`

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

# /BUSINESS-SERVICE/LIST
## ***POST*** 

**Summary:** API to get List of business service

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/business-service/list"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "business_client_id": \"string\"}"

```

### HTTP Request 
`***POST*** /business-service/list`

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

**Summary:** API to create relation between user and business service client

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/client"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "business_service_client_id": \"string\",
            "status": \"string\",
            "user_id": \integer\
         }"

```

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

**Summary:** API to create relation between user and the role in the business

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/client/role"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "business_service_client_id": \"string\",
            "role_id": \integer\,
            "status": \"string\",
            "user_id": \integer\
         }"

```

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

**Summary:** API for sending email

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/email"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "captcha": \"string\",
            "email": \"string\"
         }"

```

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

**Summary:** API to send email to the invitee

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/invitation"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "role_id": \integer\,
            "user_email": \"string\"
         }"

```

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

**Summary:** API to confirm an invitee which is invited to a business

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/invitee-confirmation"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "token": \"string\",
            "user_id": \integer\
         }"

```

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

**Summary:** API for invitee registration

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/invitee-registration"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "agreement": boolean, 
            "fullname": \"string\", 
            "password": \"string\",
            "phone_calling_code": \"string\",
            "phone_number": \"string\", 
            "token": \"string\", 
            "user_id": \integer\
         }"

```

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

**Summary:** API to create business after listening the data from kafka 

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/kafka/business"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "businessClientId": \"string\",
            "businessServiceClientId": \"string\",
            "createdBy": \"string\",
            "name": \"string\"
         }"

```

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

**Summary:** API to create business service from a business after listening the data from kafka

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/kafka/business/service"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "businessClientId": \"string\",
            "businessServiceClientId": \"string\",
            "createdBy": \"string\", 
            "name": \"string\"
         }"

```

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

**Summary:** API to get data after choosing a specific menu

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/menu/change"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "menu_id": \integer\}"

```

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

**Summary:** API to create password

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/password"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "password": \"string\", 
            "token": \"string\",
            "user_id": \integer\
         }"

```

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

# /REGISTRATION
## ***POST*** 

**Summary:** API for user registration

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/registration"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "agreement": \boolean\,
            "captcha": \"string\",
            "email": \"string\",
            "name": \"string\",
            "phone": \"string\",
            "phone_calling_id": \"string\",
            "referral_id": \"string\",
            "user_type": \"string\"
         }"

```

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

**Summary:** API for creating role

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/role"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "role_name": \"string\",
            "type": \"string\"
         }"

```

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

**Summary:** API to get list of roles

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/roles"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "id": \integer\,
            "role_name": \"string\",
            "type": \"string\"
         }"

```

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

# /TEAM-MEMBER-LIST
## ***POST*** 

**Summary:** API to get team member list with pagination

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/user/v1/team-member-list"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "pages": 0}"

```

### HTTP Request 
`***POST*** /team-member-list` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| pages | body | pages | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /TOKEN-VERIFICATION
## ***POST*** 

**Summary:** API for verifying the token to check whether the token is still valid

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/token-verification"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "token": \"string\",
            "user_id": \integer\
         }"

```

### HTTP Request 
`***POST*** /token-verification` 

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

# /USER-CONFIG
## ***POST*** 

**Summary:** API to create additional user configuration

``` shell

curl  -X POST "http://jokul-retention-dev.103.10.130.53.xip.io/retention/
               user/v1/user-config"
      -H "accept: */*"
      -H "Content-Type: application/json"
      -d "{ "key": \"string\",
            "user_id": 0, 
            "value": \"string\"
         }"

```

### HTTP Request 
`***POST*** /user-config` 

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
