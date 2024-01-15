# No-Show Analysis of Medical Appointment

## Objective
We would be looking to answer some questions and importantly, try to understand what factors contribute to patients showing up for their appointments or not;
* How do gender and age influence no-show rates?
* Does the day of the week affect patient no-shows?
* How does the neighborhood impact patients' likelihood of showing up?
* Is there a correlation between patients receiving scholarships and their attendance at appointments?

## Dataset
The dataset used for this project contains information on over a Hundred-thousand patients in Brazil who were booked for medical appointments. It also contains information on if they showed up or didn't show up for their registered appointment. The dataset was downloaded from kaggle [here](https://www.kaggle.com/datasets/joniarroba/noshowappointments). Each observation is made up 14 attributes collected to help with our analysis.

The information collected on each potential patient are as follows;

* `PatientId`: Unique number given to identify each patient.
* `AppointmentID`: Unique identifier for each registered appointment.
* `Gender`: Identifies if a patient is Male or Female.
* `ScheduledDay`: Indicates the date on which the appointment was registered.
* `AppointmentDay`: Indicates the date booked for the patient's appointment(Date to visit the clinic).
* `Age`: Represents the patient's age.
* `Neighbourhood`: Indicates the area in where the patient lives.
* `Scholarship`: Indicates if the patient is enrolled in Bolsa Familia welfare program.
* `Hypertenstion`: Signifies if the patient is Hypertensive.
* `Diabetes`: Signifies if the patient suffers from diabetes.
* `Alcoholism`: Indicates if the patient suffers from alcohol addiction.
* `Handicapped`: Signifies if the patient lives with a disability.
* `SMS_received`: Indicates if the patient was reminded about their appointment via SMS
* `No-Show`: Indicates if the patient did not show up for the appointment (‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up)

## Wrangling and Transformation
A number of transformation techniques were carried out to make analysis suitable and accurate. Some of the transformation techniques applied to the dataset include:
* Renaming of data attributes using the snake_case convention.
* Modification of column types for appropriateness.
* Removal of irrelevant observations for more focused analysis.

## Summary of Analysis
* Among our initial questions, waiting time emerged as a significant factor affecting appointment attendance. Longer waiting times correlate with increased no-show rates, this could possibly be as a result of patients feeling much better after a long period of wait or possibly patients forgetting about their appointments completely.
* The day of the week shows a weak correlation as patients tend to prefer showing up during the weak compared to the end and start of the week, with Wednesday the most preffered day of the week.
* The analysis of neighborhood impact on no-shows does not yield strong actionable insights. While we can identify areas with higher no-show rates, the reasons behind these patterns remain unclear. Incorporating data on distance from healthcare facilities and neighborhood income levels could offer more comprehensive insights.
* Age analysis reveals that less than twenty percent of infants and seniors miss their appointments, the lowest no-show rates among all age groups. This trend could be attributed to the heightened health risks for these age groups, prompting more vigilant care from parents for their children and adult children for their old parents.
