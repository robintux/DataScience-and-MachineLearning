# Problem Description
Budgets for schools and school districts are huge, complex, and unwieldy. It's no easy task to digest where and how schools are using their resources. Education Resource Strategies is a non-profit that tackles just this task with the goal of letting districts be smarter, more strategic, and more effective in their spending.

Our task is a multi-class-multi-label classification problem with the goal of attaching canonical labels to the freeform text in budget line items. These labels let ERS understand how schools are spending money and tailor their strategy recommendations to improve outcomes for students, teachers, and administrators.

## The features in this dataset
Our goal is to predict the probability that a certain label is attached to a budget line item. Each row in the budget has mostly free-form text features, except for the two below that are noted as float. Any of the fields may or may not be empty

FTE float - If an employee, the percentage of full-time that the employee works.<br>
Facility_or_Department - If expenditure is tied to a department/facility, that department/facility.<br>
Function_Description - A description of the function the expenditure was serving.<br>
Fund_Description - A description of the source of the funds.<br>
Job_Title_Description - If this is an employee, a description of that employee's job title.<br>
Location_Description - A description of where the funds were spent.<br>
Object_Description - A description of what the funds were used for.<br>
Position_Extra - Any extra information about the position that we have.<br>
Program_Description - A description of the program that the funds were used for.<br>
SubFund_Description - More detail on Fund_Description<br>
Sub_Object_Description - More detail on Object_Description<br>
Text_1 - Any additional text supplied by the district.<br>
Text_2 - Any additional text supplied by the district.<br>
Text_3 - Any additional text supplied by the district.<br>
Text_4 - Any additional text supplied by the district.<br>
Total float - The total cost of the expenditure.

## The labels in this dataset
For each of these rows, ERS attaches one label from each of 9 different categories:

Function:

Aides Compensation<br>
Career & Academic Counseling<br>
Communications<br>
Curriculum Development<br>
Data Processing & Information Services<br>
Development & Fundraising<br>
Enrichment<br>
Extended Time & Tutoring<br>
Facilities & Maintenance<br>
Facilities Planning<br>
Finance, Budget, Purchasing & Distribution<br>
Food Services
Governance
Human Resources
Instructional Materials & Supplies
Insurance
Legal
Library & Media
NO_LABEL
Other Compensation
Other Non-Compensation
Parent & Community Relations
Physical Health & Services
Professional Development
Recruitment
Research & Accountability
School Administration
School Supervision
Security & Safety
Social & Emotional
Special Population Program Management & Support
Student Assignment
Student Transportation
Substitute Compensation
Teacher Compensation
Untracked Budget Set-Aside
Utilities
Object_Type:

Base Salary/Compensation
Benefits
Contracted Services
Equipment & Equipment Lease
NO_LABEL
Other Compensation/Stipend
Other Non-Compensation
Rent/Utilities
Substitute Compensation
Supplies/Materials
Travel & Conferences
Operating_Status:

Non-Operating
Operating, Not PreK-12
PreK-12 Operating
Position_Type:

(Exec) Director
Area Officers
Club Advisor/Coach
Coordinator/Manager
Custodian
Guidance Counselor
Instructional Coach
Librarian
NO_LABEL
Non-Position
Nurse
Nurse Aide
Occupational Therapist
Other
Physical Therapist
Principal
Psychologist
School Monitor/Security
Sec/Clerk/Other Admin
Social Worker
Speech Therapist
Substitute
TA
Teacher
Vice Principal
Pre_K:

NO_LABEL
Non PreK
PreK
Reporting:

NO_LABEL
Non-School
School
Sharing:

Leadership & Management
NO_LABEL
School Reported
School on Central Budgets
Shared Services
Student_Type:

Alternative
At Risk
ELL
Gifted
NO_LABEL
Poverty<br>
PreK<br>
Special Education<br>
Unspecified Use:<br>

Business Services<br>
ISPD<br>
Instruction<br>
Leadership<br>
NO_LABE<br>L
O&M<br>
Pupil Services & Enrichment<br>
Untracked Budget Set-Aside<br>
Note, there is a hierarchical relationship for these labels. If a line is marked as Non-Operating in the Operating_Status category, then all of the other labels should be marked as NO_LABEL since ERS does not analyze and compare non-operating budget items.

Reference: <b>Reboot: Box-Plots for Education, HOSTED BY EDUCATION RESOURCE STRATEGIES</b>
