# Auth Service

Auth Service is reponsible for login, registration, 
and Carrier identification.

## Events for Receive
* [Login](#login-event)
* [Registration](#registration-event)
* [GetToken](#gettoken-event)
* [Logout](#logout-event)
* [ForgotPassword](forgotpassword-event)

### Login Event

#### Request Fields:

| Field | Type [min/length/max] | Description | 
| --- | --- | --- |
| username* | string [255] | Carrier user name |
| password* | string [255] | Carrier password |
| device_id* | string [100] | Carrier Device ID | 

\* required

####  Response Fields:

| Field | Type [min/length/max] | Description |
| --- | --- | --- |
| status* | [status_type](AdditionaServicesGenericTypes.md#status-type) | Response status |
| token_info | [token_info_type](AdditionaServicesGenericTypes.md#token-info-type) | Token information for User |

\* required 

### Registration Event

#### Request Fields:

| Field | Type [min/length/max] | Description | 
| --- | --- | --- |
| usernamee* | string [255] | Carrier user name |
| password* | string [255] | Carrier password |
| device_id* | string [100] | Carrier Device ID |
| profile* | [profile_type](AdditionaServicesGenericTypes.md#profile-type) | Profile user information |

\* required

####  Response Fields:

| Field | Type [min/length/max] | Description |
| --- | --- | --- |
| status* | [status_type](AdditionaServicesGenericTypes.md#status-type) | Response status |
| token_info | [token_info_type](AdditionaServicesGenericTypes.md#token-info-type) | Token information for User |

\* required 

### GetToken Event

#### Request Fields:

| Field | Type [min/length/max] | Description | 
| --- | --- | --- |
| device_id* | string [100] | Carrier Device ID | 

\* required

####  Response Fields:

| Field | Type [min/length/max] | Description |
| --- | --- | --- |
| status* | [status_type](AdditionaServicesGenericTypes.md#status-type) | Response status |
| token_info | [token_info_type](AdditionaServicesGenericTypes.md#token-info-type) | Token information for User |

\* required 

### Logout

#### Request Fields:

| Field | Type [min/length/max] | Description | 
| --- | --- | --- |
| device_id* | string [100] | Carrier Device ID | 

\* required

####  Response Fields:

| Field | Type [min/length/max] | Description |
| --- | --- | --- |
| status* | [status_type](AdditionaServicesGenericTypes.md#status-type) | Response status |

\* required 


### ForgotPassword

#### Request Fields:

| Field | Type [min/length/max] | Description | 
| --- | --- | --- |
| username* | string [255] | Carrier user name |
| device_id* | string [100] | Carrier Device ID | 

\* required

####  Response Fields:

| Field | Type [min/length/max] | Description |
| --- | --- | --- |
| status* | [status_type](AdditionaServicesGenericTypes.md#status-type) | Response status |

\* required 
