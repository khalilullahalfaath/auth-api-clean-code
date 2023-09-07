auth-api/ → Project Root.
├─ config/ → Configuration folder, used to configure node-pg-migrate for the testing database.
├─ migrations/ → Database migration files.
├─ src/ → Application source code.
│ ├─ Applications/ → Application Business Rules.
│ │ ├─ security/ → Abstractions/interfaces of tools and helpers related to security used in use cases. Examples include AuthTokenManager and EncryptionHelper.
│ │ ├─ use_cases/ → Business flow of the application.
│ ├─ Commons/ → Shared folder.
│ │ ├─ exceptions/ → Custom exceptions.
│ ├─ Domains/ → Enterprise Business Rules.
│ │ ├─ authentications/ → Subdomain for authentications, containing domain models (entities) and abstractions/interfaces for the AuthenticationRepository.
│ │ ├─ users/ → Subdomain for users, containing domain models (entities) and abstractions/interfaces for the UserRepository.
│ ├─ Infrastructures/ → External Agents such as Frameworks and External Tools.
│ │ ├─ database/ → Database driver.
│ │ ├─ http/ → HTTP Server using Hapi.js.
│ │ ├─ repositories/ → Concrete implementations of domain repositories.
│ │ ├─ security/ → Concrete implementations of tools and helpers related to security.
│ │ ├─ container.js → Container for all instances of services used in the application.
│ ├─ Interfaces/ → Interface Adapter. Here, we define route configurations and handlers wrapped with Hapi Plugins.
│ ├─ app.js → Application entry point.
├─ tests/ → Utilities needed for testing.
├─ .env → Environment variables.
├─ package.json → Project Manifest.
