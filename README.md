# CVE-2021-46070

### Exploit Title: Vehicle Service Management System - 'Service Requests' Stored Cross Site Scripting (XSS)
### Exploit Author: <a href="https://www.plsanu.com">P.L.Sanu</a>
### CVE: CVE-2021-46070
### CVSS: 4.8 MEDIUM
### References: 
- https://www.plsanu.com/vehicle-service-management-system-service-requests-stored-cross-site-scripting-xss
- https://nvd.nist.gov/vuln/detail/CVE-2021-46070
- https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-46070

### Exploit:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Service Requests section and click on Create New button. 
3. Inject the below payload in Owner Contact, Address, Vehicle Name, Vehicle Registration Number & Vehicle Model input field.

### Payload:
```html
 "><script>alert(document.cookie)</script>
```

5. Click on Save Request button.
6. Malicious javascript code triggered.
7. Navigate to Report section.
8. Malicious javascript code triggered.
