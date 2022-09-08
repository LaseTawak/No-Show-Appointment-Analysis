# No-Show Analysis of Medical Appointment

## Objective
We would be looking to answer some questions and try to find out if these variables can help predict patients showing up for their appointment or not and the other variables provided ;
* How does gender and Age influence on No-shows ?
* Does the day of the week have an effect on No-show ?
* Does neighbourhood influence patients showing up or not ?
* Is there a relationship between patients on scholarship and showing up for appointments ?

## Dataset
The dataset used for this project contains information on a 100thousand patients in Brazil who were booked for medical appointments. It also contains information on whether they showed up or didn't show up for their registered appointment. The dataset was downloaded from kaggle [here](https://www.kaggle.com/datasets/joniarroba/noshowappointments). Each observation is made up 14 attributes collected to help with our analysis.

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
A number of transformation techniques were carried out to make analysis suitable and accurate. Some of the actions carried out to make the sata suitable for analysis are as follows:
* Data attributes were renamed using the snake_case naming convention.
* Column types were changed to make appropriate.
* Some observations were removed as they did not make sense to our analysis.

## Summary of Analysis
* Of the questions we asked in the beginning of this analysis, only wait time seems to have a strong influence on how patients react to meeting up for their appointments, with patients less likely to show up the longer they have to wait. This could possibly be as a result of patients feeling much better after a long period of wait or possibly patients forgetting about their appointments completely.
* The day of the week shows a weak correlation as patients tend to prefer showing up during the weak compared to the end and start of the week, with Wednesday the most preffered day of the week.
* Analysis of neighbourhood's effect on No-show appointments does not show strong actionable information as we can only tell which locations have high No-Show rate but not why these places have high values. Having information on distance and neighbourhood income could help provide better insights.
* For Age, rate of No-Show tells us less than twenty percent of Infants and Seniors missed their appointments, which are the lowest rate of No-show by any of the age categories. This could be assumed to be as a result of these two categories have weaker immune systems, therefore Parents are less likely to take chances on the health of their infants. Adult Children also want to see their parents(Seniors) live longer and would most likely not take chances with their parents health.
