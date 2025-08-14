# 📝 Note Management System

A comprehensive REST API built with **MuleSoft 4.9.0** for managing notes with MySQL database integration and Salesforce synchronization.

## 🚀 Features

- **CRUD Operations**: Create, Read, Update, Delete notes
- **Bulk Operations**: Import multiple notes efficiently  
- **Database Integration**: MySQL with connection pooling
- **Salesforce Integration**: Sync notes with Salesforce platform
- **API Console**: Interactive API documentation
- **Error Handling**: Comprehensive error responses
- **Security**: Encrypted configuration properties

## 🛠️ Technology Stack

- **MuleSoft Runtime**: 4.9.0
- **Database**: MySQL
- **Integration**: Salesforce Connector
- **Build Tool**: Maven
- **Testing**: MUnit 3.4.0

## 📋 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/notes` | Retrieve all notes |
| GET | `/notes/{id}` | Get note by ID |
| POST | `/notes` | Create new note |
| PUT | `/notes/{id}` | Update note |
| DELETE | `/notes/{id}` | Delete note |
| POST | `/notes/bulk` | Bulk import notes |
| GET | `/console` | API Console |

## 🏃‍♂️ Running the Application

1. **Configure Database**: Update `Note.properties` with your MySQL credentials
2. **Configure Salesforce**: Add your Salesforce connection details
3. **Start Application**: Deploy to Mule Runtime
4. **Access API**: `http://localhost:8082/api/notes`
5. **API Console**: `http://localhost:8082/console`

## 📬 Testing with Postman

Import the included Postman collection:
- `Note-Management-System-Port-8082.postman_collection.json`
- `Note-Management-System-Environment.postman_environment.json`

## 🔧 Configuration

The application uses encrypted properties in `Note.properties`:
- Database connection settings
- Salesforce credentials  
- HTTP listener port (8082)

## 📁 Project Structure

```
src/
├── main/
│   ├── mule/
│   │   └── note-management-system.xml    # Main flow configuration
│   └── resources/
│       ├── Note.properties               # Configuration (encrypted)
│       ├── application-types.xml         # RAML data types
│       └── log4j2.xml                   # Logging configuration
└── test/
    └── munit/                           # MUnit tests
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License.

---
**Built with ❤️ using MuleSoft**
