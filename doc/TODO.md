### General
- Job entries without samples are not reflected in the monthly report's raw data:
  * Setup a unit test in BEl and modify and test Job.getJobReportRecords()
  * Use the method from one of the costing/invoice reports to get the job sample records.
- Check out claim that the reports are not responding to parameter changes.
  Also check why last/this does not give the correct period.
- Implement month report feature update in accordance with proforma, report template
  and GA's email:
  * Update Job class to contain the new fields according to the new monthly report format:
    ~ Add the fields to the Job class for the number of services offered (eg noOfTrainings).
      Export the first 2 rows of the report template as PDF for reference.
  * Update the Job dialog to allow entry into the new fields.
  * See Github issues.
- Remove code comment out of initDashboard() and initMainTabView() before deploment.