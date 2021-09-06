# UFOs
## Summary
Providing users with an online interface for filtering UFO sighting data to easily sift through the available information.  The data is contained within a table that can be dynamically filtered using 5 fields on the left side of the screen to focus on the desired data points.

## Results
The search fields to the left allow the user to dynamically filter the tabular data in real-time.  Simply enter the desired information into the correct field, ensure it is splled correctly and follwos the same syntax as the data in the table.  For example, if we wish to filter for sightings on Jan 1, 2010, entering 01/01/2010 will not work - the data is currently sutrctured such that 1/1/2010 is required.  Enter the date desired and press tab and the list will instantly filter:
![Filter1](https://github.com/rscalise88/UFOs/blob/main/report/Capture1.PNG)

The same follows for further filtering the data from there.  There were a number of sightings on the 1st - let's trim the results down to just those in California:
![Filter12](https://github.com/rscalise88/UFOs/blob/main/report/Capture2.PNG)

Perhaps we have family in El Cajon and wish to see potential UFO activity there:
![Filter3](https://github.com/rscalise88/UFOs/blob/main/report/Capture3.PNG)

Additionally, the data can be filtered by type of phenomenon:
![Filter4](https://github.com/rscalise88/UFOs/blob/main/report/Capture4.PNG)


## Conclusion
As made clear in the preceding section, there exists a glaring drawback to the current format of this tool: the lack of any kind of dynamic input interpretation.  Ideally, the tool would be able to understand that 01/01/2010 and 1/1/2010 represent the same day and thus return the same results from the filtering.  As it currently stands, there is zero room from error from the end user, otherwise the tool will not function properly.  This could be implmeneted by improving the reading capabilities of tool itself, or by forcing the user to only select those options that are available either through strict input validation and an error message or by providing drop-down menus to ensure that only the proper options can be selected.

In addition to the above mentioned shortcoming, I believe it would be useful if the end user were able to see the results in real-time as the text is entered.  As it exists currently, the pseudo-realtime setup requires all text to be entered and the field in use to be exited from before the results are visible.  Further, when working with significantly larger datasets, it would be beneficial to have a sort function on top of the table, similar to the filtering options avilable in Excel, or providing an option in the filter tool on the left that would allow the user to sort the data as they see fit.
