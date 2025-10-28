Σκοπός

Να τρέξουμε αυτόματα τα API tests που έχουμε στο Postman,
χρησιμοποιώντας το εργαλείο Newman (το “CLI version” του Postman),
μέσα από ένα GitHub Actions pipeline (δηλαδή αυτοματοποιημένο workflow).

##  Test Reports

### Example Test Execution
```bash
newman run postman_collection.json -e postman_environment.json -r cli,html
```

### Test Results
![API Test Report](report-screenshot.png)

-  **5/5 Assertions Passed**
-  **2 API Requests Executed** 
-  **0 Failures**
-  **Average Response Time: 66ms**

### Reports Generated
- **CLI Report**: Real-time results in terminal
- **HTML Report**: Detailed report in `newman/` folder

## Allure Reporting Setup

### New Features
 **Allure Framework** integration for detailed test reporting
 **Automated test execution** with Newman
 **Visual analytics** with graphs and execution trends
 **Step-by-step execution** details for each API call


### Test Results
![Allure Overview](screenshots/allure-overview.png)
*Overview dashboard showing 100% test success rate*

![Allure Behaviors](screenshots/allure-behaviors.png)
*Test suites with detailed execution results*

![Allure Graphs](screenshots/allure-graphs.png)
*Analytics and execution trends*


