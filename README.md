!
## Entity Relationship Diagram

### User

| Key           | Name          | Type          |
|---------------|---------------|---------------|
| id            | ID            | Primary Key (UUIDField) |
| username      | Username      | CharField     |
| password      | Password      | CharField     |
| account_type  | Account Type  | CharField     |
| region        | Region        | CharField     |
| account_name  | Account Name  | CharField     |
| qr_code       | QR Code       | CharField     |

### Document

| Key           | Name          | Type          |
|---------------|---------------|---------------|
| id            | ID            | Primary Key (UUIDField) |
| user          | User          | ForeignKey (User) |
| title         | Title         | CharField     |
| content       | Content       | TextField     |
| created_at    | Created At    | DateTimeField |
