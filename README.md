# Clinware Compliance API

This is a Spring Boot application that provides two REST APIs:

1. **Offender Search API** - Searches for offender records from the NSOPW.gov database.
2. **Address Validation API** - Validates and standardizes U.S. addresses using Google's Address Validation API.

---

Tech Stack

- Java 17
- Spring Boot 3.1.3
- Maven
- Google Address Validation API
- NSOPW.gov API (via HTTP)

---

 How to Run

1. Clone the repository
2. Add your Google API key in application.properties
3. Run the application:
   ```
   mvn spring-boot:run
   ```

---

 Endpoints

### 1. /api/address/validate
**POST**  
Request Body:
```json
{
  "addressLine1": "1600 Amphitheatre Parkway",
  "addressLine2": "",
  "city": "Mountain View",
  "state": "CA",
  "zipCode": "94043"
}
```

### 2. /api/offender-search
**POST**  
Request Body:
```json
{
  "firstName": "John",
  "lastName": "Doe",
  "city": "Austin",
  "state": "TX",
  "dob": "1990-01-01"
}
```

---

 Author

**Jaya Dhiman**  
GitHub: [jayadhiman31](https://github.com/jayadhiman31)

