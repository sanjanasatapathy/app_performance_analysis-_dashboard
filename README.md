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
   
 ```sh  
git clone https://github.com/sanjanasatapathy/app-performance-analysis-dashboard.git
cd app-performance-analysis-dashboard
```
    
2.  Install the required libraries:
```sh
   pip install -r requirements.txt
   ```
    
3.  Place the log file (Copy of app\_logs.xlsx) in the project directory. You can refer to this  [sample file](https://docs.google.com/spreadsheets/d/1iUd_HFOKm287Vd0VXyVsTNQRCkBzWBrh3co_uthaRNA/edit?gid=386998417#gid=386998417)
    
### **Run the Script**

Execute the following command to calculate metrics, detect anomalies, and generate visualizations:
```sh
python main.py   `
```

 **Approach Explanation**  
----------------
1. **Performance Analysis**:     

    *   Created Python functions to calculate key metrics such as average and P95 response times per endpoint, error rates, and   peak usage periods.     
    *   Derived user experience metrics like the percentage of requests exceeding 1 second.

2. **Visualization Dashboard**:     

    *   Developed time-series plots for response time trends and bar charts for error rate patterns.     
    *   Conducted hourly analysis for peak usage and comparison of endpoint performance.  

3. **Anomaly Detection**:     

    *   Implemented basic statistical methods to detect spikes in response times.     
    *   Identified error rate anomalies and potential endpoint availability issues using grouped aggregations and thresholds.  

4. **Code Structure**:     

    *   Functions were modularized for reusability.     
    *   Error handling and validations were added to manage inconsistent data.  

5. **Documentation**:  

    *   Added inline comments for better code readability.  



**Key Insights**
----------------

### **Metrics Summary**:

1.   **Response Times**:
    
     *   Average and P95 response times highlight endpoint performance.
        
2.   **Error Rates**:
    
     *   Most errors occurred with specific endpoints, indicating areas to optimize.
        
3.   **Peak Usage**:
    
     *   Certain time slots had significantly higher requests, which could help in load balancing.
        
4.   **User Experience**:
    
     *   Around of requests exceeded 1 second.
        

### **Anomalies**:

*   Unusual spikes in response times were detected on .
    
*   Significant error anomalies identified for HTTP status codes 500 and 504.
    

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


*   [Sanjana Satapathy](https://www.linkedin.com/in/sanjana-satapathy-926293228/) - Data Analyst
    

**License**
-----------

This project is licensed under the MIT License.