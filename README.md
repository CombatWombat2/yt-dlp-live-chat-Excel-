"READ ME

The Excel workbook takes the youtube live chat json file that is created by yt-dlp, repairs it and renders a subset of the available fields. I have not found any documentation for the json schema and uy-dlp uses a different live chat schema in different scenarios.  I have done my best to account for the different schemas but there may be errors.  If you notice that some of the outputted fields are blank, please log a issue with the attached json file.

**Basic Instructions:** Enter the name and path of the YT-DLP live chat json file in cell B1 and hit refresh all. You can enter it manually or click the open file button  to run a macro.   Hit ""refresh all"" to load the file and refresh the output (alternatively click on Refresh All under the data menu).

After you click on refresh all, the nicely formatted chat history is refreshed in the Chat History worksheet.  Remember to adjust any filters you used from your previous file.

**Macros:** Enabling Macros is not necessary for the spreadsheet to work.  If you want to run without macros enabled: 1. instead of clicking the Open File button, cut and past the path to the file into cell B3.  2. Instead of clicking on the Refresh All button, click on Refresh All under the Data menu.

**Json Repair:** The Powerqueres in this workbook repairs the YT-DLP json by adding comma between rows and wrapping in []

Emoticons: Chat emoticons are not rendered.

**Chat Timestamps:**  Absolute Timestamps: Its recommended to sort the output by the timestampUsec property. This is also the default sort order when.   This is the unix epoch of the absolute chat time. Chat timestamp relative to the start of the live is the ""TimeStamp"" field 
"




