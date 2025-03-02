# CS-305 Project Two: Practices for Secure Software

## **Artemis Financial - Secure Software Implementation**

### **Client Overview**
Artemis Financial is a financial services company requiring improved security measures for its software applications. Their primary security concerns included securing client-server communications, ensuring data integrity, and mitigating vulnerabilities in third-party dependencies.

### **Security Measures Implemented**
To enhance the security of Artemis Financial's software, the following measures were implemented:

1. **Cryptographic Hashing (SHA-256)**  
   - SHA-256 was used for checksum validation to ensure file integrity.
   - Protects against unauthorized modifications and data tampering.

2. **SSL Certificate Generation (Java Keytool)**  
   - A self-signed SSL certificate was created to enforce HTTPS.
   - Ensured secure encrypted communication between the client and server.

3. **Checksum Verification Endpoint**  
   - Implemented a REST API endpoint to verify file integrity.
   - Utilized SHA-256 to generate unique hashes for transmitted files.

4. **Secure Communications (HTTPS Implementation)**  
   - Configured Spring Boot application to enforce HTTPS using a self-signed SSL certificate.
   - Prevents man-in-the-middle (MITM) attacks by encrypting client-server communications.

5. **Static Security Analysis (OWASP Dependency-Check)**  
   - Scanned third-party dependencies for known vulnerabilities.
   - Mitigated risks by updating libraries and removing insecure dependencies.

6. **Functional Testing & Code Validation**  
   - Verified application functionality after refactoring.
   - Ensured secure data transmission and correct checksum verification.

### **Challenges and Lessons Learned**
- Implementing **SHA-256 hashing** and ensuring correct checksum validation was challenging but reinforced the importance of **data integrity** in secure applications.
- **Generating and configuring SSL certificates** required understanding Java Keytool and HTTPS security configurations.
- **Using OWASP Dependency-Check** highlighted the importance of regularly scanning for vulnerabilities in third-party libraries.

### **Tools & Best Practices Used**
- **Java Keytool** – for SSL certificate generation.
- **Spring Boot Security** – for enforcing HTTPS.
- **SHA-256 Hashing** – for data integrity verification.
- **OWASP Dependency-Check** – for identifying security vulnerabilities.
- **Postman** – for API endpoint testing.
- **Maven** – for building and managing dependencies securely.

### **Portfolio Value & Future Use**
This project demonstrates expertise in **secure software development** and **vulnerability assessment**, which is valuable for future roles in cybersecurity and software engineering. Key skills showcased include:
- Implementing **cryptographic hashing** for data integrity.
- Enforcing **secure HTTPS communications** with SSL certificates.
- Performing **static security analysis** to mitigate third-party risks.
- Conducting **functional testing** to validate security measures.

### **GitHub Repository**
(https://github.com/synthesoul/CS305)

This project highlights critical secure coding techniques and can serve as a strong portfolio piece for potential employers.
