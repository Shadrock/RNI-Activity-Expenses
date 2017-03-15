# RNI Activity Expenses


This repository contains a dataset detailing expenses for activities that were conducted as part of [Ushahidi](https://www.ushahidi.com)'s [Resilience Network Initiative](http://cityresilience.net/what-is-rni.html) ("RNI") in Indonesia. You can learn more about the project [in this video](https://vimeo.com/129603769) and [this blog post](http://www.100resilientcities.org/blog/entry/kathmandu-semarang-citizen-engagement-and-open-data-mapping-in-two-cities#/-_/).

## Data
The [data folder](https://github.com/Shadrock/RNI-Activity-Expenses/tree/master/data) contains:
* A complete [list of **all** expenses](data/RNI IND Project Expenditures 2014-2015.json) associated with RNI's work in Indonesia in [JSON](http://www.json.org/), which is a great open standard data format. 
* A complete [list of **all** expenses](data/RNI IND Project Expenditures 2014-2015.csv) associated with RNI's work in Indonesia in a table... for those who like that sort of thing. 

### Key Code
* __Expense Type:__ Primary field used for internal reporting. Range includes:
  * Travel - costs such as airfare, hotels, meals, etc.
  * Services - specifically online services such as web hosting.
  * Contractor - anyone who received funds to carry out activities for the project. This includes local partners.
  * Operational - funds used by Ushahidi to implement aspects of the project, such as software customization.
  * Equipment - material items purchased.
* __Sub-type__ - Additional detail of expense type. 
* __Purpose__ - Specifies the purpose or activity to which the expenditure belongs such as attending a planning meeting or a payment to a local partner for a specific event.
* __Notes__ - Additional detail.
* __Date of Sale__ - Date in dd/mm/yy format. This indicates the date the purchase or transfer of funds was made.
* __Location at Point of Sale__ - The physical location of the entity receiving funds. "Online" refers to purchases made via the web in which case the physical location of the receiving entity may be unknown. 
* __Country of Activity__ - Primary country in which the activity took place.
* __City of Activity__ - Primary city in which the activity took place.
* __Amount (USD)__ - Cost in U.S. dollars. Costs in other currencies were converted using Google's currency converter or bank statements. 
* __Code__ - Refers to which aspect of the project the expense can be associated:
  * RNI - Expenses that were applicable to the entire RNI project, such as donor meetings or conferences.
  * RNI/IND - Expenses exclusively related to activities in Indonesia. 
  * RNI/IND/VN - Expenses that were applicable to project work in Viet Nam and Indonesia. In some cases it was more cost effective to combine trips to limit the amount spent on airfare or other travel costs. In these cases it wasn't possible to determine exactly which portion of the expense could be assigned to only one project site. 

### Abbreviations
Several abbreviations are used throughout this data set. They include: 
* VN = Viet Nam
* IND = Indonesia 
* NYC = New York City
* DC = Washington, D.C. 
* RT = round trip 
* ATL = Atlanta
* USAID = [U.S. Agency for International Development](https://www.usaid.gov)
* USAID/OTI = [U.S. Agency for International Development's Office of Transition Initiatives](https://www.usaid.gov/who-we-are/organization/bureaus/bureau-democracy-conflict-and-humanitarian-assistance/office-1)
* DHS = [The Demographic and Health Surveys Program](http://dhsprogram.com/)
* HOT = [Humanitarian OpenStreetMap Team](https://hotosm.org/)
* OSM = [OpenStreetMap](https://www.openstreetmap.org/)
* JKT = Jakarta
* GA = Georgia (U.S. State)
* SoW = Scope of work; includes work plan discussions. 

## Data Creation Process for this Repository
These data were created and used primarily as a method of internal expense tracking and final reporting to donors at the close of the project. Expenses were generally logged using receipts collected during activities. Monthly logs in spreadsheet form were used by the Ushahidi accounting team. As Director, I kept a running spreadsheet of every expense that was possible to track. The data in this repository is a sub-set of data relating specifically to our project work in Indonesia. The original Excel workbook was saved as a .csv and converted using [this tool](http://www.convertcsv.com/csv-to-json.htm).

### Redaction Process
For the most part, the records presented here are unedited. I have redacted individual names, which were used to appropriately split or assign costs when working with Ushahidi colleagues who had their own budgets. In these cases I have simply used the term "colleague." In a few instances I have added greater clarity to descriptions or abbrevations that were used internally. 

I see this dataset as an example of the granularity that is possible for reporting and how Ushahidi can be more open and transparent about how and where we work. This is a work in progress for us and I welcome feedback on how data creation of this type can be improved for various uses.


