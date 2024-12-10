**App Performance Analysis Dashboard**
======================================

**Project Overview**
--------------------

This project analyzes application logs to extract insights about app performance, user experience, and health. Using Python, key metrics such as response times, error rates, and usage patterns were calculated, and visualizations were created to help monitor the app's health effectively. Basic anomaly detection was also implemented.

**Features**
------------

1.  **Performance Metrics Calculation**:
    
    *   Average and P95 response times per endpoint.
        
    *   Error rates and breakdown by HTTP status codes.
        
    *   Peak usage periods by time and date.
        
    *   User experience insights (e.g., % of requests exceeding 1 second).
        
2.  **Visualization Dashboard**:
    
    *   Trends in response times.
        
    *   Error rate patterns.
        
    *   Peak usage analysis.
        
    *   Comparison of endpoint performance.
        
3.  **Anomaly Detection**:
    
    *   Identification of spikes in response times.
        
    *   Detection of error rate anomalies.
        
    *   Endpoint availability issues (hours with zero requests).
        

**Setup Instructions**
----------------------

### **Prerequisites**

*   Python 3.8+
    
*   Required Libraries: pandas, matplotlib, openpyxl
    

### **Installation**

1.  Clone the repository:
   
   git clone https://github.com/<your-username>/app-performance-analysis-dashboard.git
   cd app-performance-analysis-dashboard
    
2.  Install the required libraries:
   
   pip install -r requirements.txt
    
3.  Place the log file (Copy of app\_logs.xlsx) in the project directory.gi
    
### **Run the Script**

Execute the following command to calculate metrics, detect anomalies, and generate visualizations:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopy codepython main.py   `

**Key Insights**
----------------

### **Metrics Summary**:

*   **Response Times**:
    
    *   Average and P95 response times highlight endpoint performance.
        
*   **Error Rates**:
    
    *   Most errors occurred with specific endpoints, indicating areas to optimize.
        
*   **Peak Usage**:
    
    *   Certain time slots had significantly higher requests, which could help in load balancing.
        
*   **User Experience**:
    
    *   Around of requests exceeded 1 second.
        

### **Anomalies**:

*   Unusual spikes in response times were detected on .
    
*   Significant error anomalies identified for HTTP status codes 500 and 503.
    

**Visualizations**
------------------

### **Examples**:

1.  **Response Time Trends**:
    
    *   Time-series plots showing endpoint performance over time.
        
2.  **Error Patterns**:
    
    *   Bar charts showing the distribution of error types.
        
3.  **Peak Usage**:
    
    *   Hourly analysis of request patterns.
        

**Future Improvements**
-----------------------

1.  Add interactive visualizations using libraries like Plotly or Dash.
    
2.  Automate anomaly alerts using statistical models or machine learning.
    
3.  Extend the dashboard to include user-specific insights (e.g., session durations).
    
4.  Optimize performance for larger datasets.
    

**Contributors**
----------------

*   **Sanjana Satapathy** - Data Analyst
    

**License**
-----------

This project is licensed under the MIT License.