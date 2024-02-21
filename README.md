**Basic Instructions**: Enter the name and path of the YT-DLP live chat json  file in cell B1 and hit refresh all. You can enter it manually or click the open file to run a macro.   Hit "refresh all" to load the file and refresh the output.
The nicely formatted chat history is refreshed in the Chat History worksheet.  The Chat History workbook contains a small subset of available fields.   To add fields edit the "Query Output" powerquery.

**Macros**: Enabling Macros is not necessary for the spreadsheet to work.  If you want to run without macros enabled: 1. instead of clicking the Open File button, cut and past the path to the file into cell B3.  2. Instead of clicking on the Refresh All button, click on Refresh All under the Data menu.

**Json Repair**: The Powerqueres in this workbook repairs the YT_DLP json by adding comma between rows and wrapping in []

**Emoticons:** Chat emoticons are not rendered property and add extra rows to the output, often with a null value in the message text property. Rows with a null in the message text are filtered out.

**Chat Timestamps:**  Absolute Timestamps: Its recommended to sort the output by the timestampUsec property.  This is the unix epoch of the absolute chat time.
Chat timestamp relative to the start of the live is the VideoOfsetTimeMsec field and is in milliseconds. This value comes from the YT-DLP json file and can be be slightly different from the live replay chat timestamp (for reasons unknown).  Excel powerquery derives an Excel formatted relative timestamp from  VideoOfsetTimeMsec and stores it in the ChatTimestamp 


