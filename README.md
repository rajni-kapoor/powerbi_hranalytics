# powerbi_hranalytics
*HR Analytics project using Power BI*
Project: Power BI
Hi everyone, My Power BI dashboard project. This project is a case study for HR Analytics. 

![image](https://user-images.githubusercontent.com/123319398/228378508-96ce92b0-867f-4f9f-87ea-0de4e0da7bef.png)


**About the project :** Human Resource is a very important for any business which drives the business to the path of success or bankruptcy if managed efficiently. In this project we will analyze the data regarding the recruitment, retention or retrenchment to improve the business outcomes. This analytic project will help the management to take data-driven decisions to promote the positive employees experience.

Data-set : CSV file format “HR Analytics data.csv”

*Problem-Statement:* The company has faced financial crisis after covid pandemic’s effect and the ongoing recession, and asked the human resource team to analyze the data and provide insights so that management can take decision to improve the company’s condition.

![image](https://user-images.githubusercontent.com/123319398/228572884-bd32855f-b56d-4e58-a1f1-f3d7afa2cfdf.png)

Data Cleaning : The data was in a csv format which I import in a power bi desktop application and used power query editor to scrub the data. Following were the steps I took:  
•	Splitting Columns by Delimiter as the whole content was separated by commas and in single cell  
•	Used first row as headers  
•	Remove Duplicates  

*DAX measures:* I created simple measures to create important fields with the help of following DAX formulas  
•	COUNTROWS  
•	CALCULATE  
•	DIVIDE  
•	ISBLANK  
•	IFELSE  
With the help of this formulas I created following measures  
•	Total Employees  
•	Male (Number of male employees)  
•	Female (Number of female employees)  
•	% male employees  
•	%female employees  
•	Due for promotion  
•	Not due  
•	% Due promotion  
•	% Not due  
•	On Service  

![image](https://user-images.githubusercontent.com/123319398/228378675-1be1002a-ac0f-4dc3-8c94-4e8e28c4d522.png)


I also created Conditional Column to add data   
•	Job Levels  
•	Service Year  
•	Retrenchment Status  
•	Distance Status  
•	Employee Name  
•	Job Satisfaction Level  
•	Performance Rating  
*Due for promotion/Not due:* Management decided that employees who had never been promoted since the last 10 years and above is now due for promotion.  

*Layoffs/Retrenchment:* The company needs to retrench some employees for some reasons, so company will let employees go who have worked in the organization for 18 or more years.  

*Distance from home to work:* We need to find how many workers are very far, near and very close to the organization or office.  

*Severance Pay:* The organization needs to pay SEVERANCE Benefit to people that ought to be promoted but suddenly on a retrenchment list. Our job is to extract those employees before they are retrenched.  

Import the data from employeedata.csv and merged with the main dataset. In this file the employees name will be added and sorted in ascending order. Then I added a column where I put the condition if the employee name of first table is equal to the name of second table and the column of due for promotion and retrenchment also contain 1 then this cell will contain the employee name otherwise just leave blank.  

![image](https://user-images.githubusercontent.com/123319398/228378905-f1278b6f-949d-4609-afe6-34bc3139a375.png)


*Job Satisfaction Score:* The company wants to know how many employees are satisfied working with the organization. Thus we divided the scores so that if job satisfaction score >3 then the satisfaction level is “High”, elseif the score is equals to 3 then the satisfaction level is “Medium”, otherwise it is “Low”.  

*Performance Ratings:* The management wants to assess the performance of the employees for future reward or promotion. So if the performance rating is 4 then it is “High Rating” and if it is 3 the it is “Low Rating”.  

*Distance Status:* The measure I used for distance is that if the distance from home to company is greater than 20 km, then they come under “very far” category, 10-20 km comes under “close” category and people who lives under 10 km from office is put into “very close” category.  

![image](https://user-images.githubusercontent.com/123319398/228379045-1b8c1a08-ee0c-4dc3-b7e8-e47d86e3e717.png)


*Findings/Outcomes:  *
	An interactive dashboard which is a 3 page report linked with buttons. Home is the main page of our dashboard which shows the total employees, male and female employees, distribution of total employees by service years and job levels and the number of employees who are due for promotion.  
	The next page is action page which shows the number of people who likes to do overtime and who do not. It also shows the number of people who got high and low ratings in their work, and the number of employees job roles who are due for promotion and retrenchment. A stacked bar chart shows that maximum number of people have low satisfaction with their job at 569, which is a matter of concern. So, there should be reasons which should be find out how their satisfaction level can be improve for the betterment of the work culture.  
	List page has 3 important visuals which shows the list of employees who should receive Severance pay, the number of people who are due for promotion and retrenchment categorized on our main departments like Research & Development, Human Resource and Sales, and it also shows how many employees are living far, close and very close to the company premise.  

![image](https://user-images.githubusercontent.com/123319398/228379103-44eaa475-b315-471e-a634-5f8fa6ee301e.png)


