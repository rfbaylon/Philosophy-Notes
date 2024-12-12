
****
# Spreadsheets
## Pathways
#### All Pathways
*Not a spreadsheet, but a folder full of spreadsheets.*
When selecting a spreadsheet, there are a few tabs. For example, Bridgewater has the following:
Bridgewater, Bunker Hill, Bristol, Cape Cod, Massasoit, MassBay, North Shore, Roxbury.

Bridgewater / Bridgewater: The BS in CS degree requirements. 
	I will call this the '4y Tab'
Bridgewater / (Any Community College): The transfer degree from that CC to Bridgewater. 
These spreadsheets are formatted to appease [curricularanalytics.org](curricularanalytics.org). 
	I will call this a 'Transfer Tab'

##### Colors!
- Grey: A course that transferred from community college. Was used to replace a course in the four-years curriculum
- Blue: A course that transfers but the *only* thing that it counts for is general elective credits to get a student to 120 credit hours before graduation
- Red: (Inconsistently used) means it was a community college course that transferred in no way to the four year.
- Yellow: (Inconsistently used) (Mostly disregard) -- originally used to determine if the CC offered a course that transferred. If its yellow, it means yes, but it wasnt part of the AS. So useless that Catherine doesnt know yellow means anything. 

#### **Pathways Master**
Each of the green cells are community colleges within 50 miles driving distance (measured by google maps) from four-years in the state.

Has 4 sheets within it: Curricular Complexity, Cost, Credit Hours, % Credit Hours
- Curricular Complexity: Automatically calculated by curricularanalytics.org. Within All Pathways folder, for each 4y Tab and Transfer Tab, download as csvs. I then uploaded them to curricularanalytics, for the site to return a score. This score is inputted in Curricular Complexity section of Pathways Master.
- Credit Hours: For each 4y Tab and Transfer Tab, this cell just represents the sum of Column H. 
- % Credit Hours: For each Transfer Tab, this cell is the sum of credits for each *grey* course minus the sum of credits from the AS. The sum of credits for the AS is found by totalling Column H for each tab in 'All CC As'
- Cost: (Cost per year for each 4y / 24 credits) * (Total credits from Credit Hours -120)

#### All CC AS
The AS for each community college, formatted to appease [curricularanalytics.org](curricularanalytics.org). Used to make everything in the All Pathways folder.


## Heatmap
#### Four-Year Heatmap
*unlike* Pathways, this section does NOT care about the AS.

##### Tabs
- Tallys: The sum of courses within each field from the rest of the spreadsheet
- University: 
	- Row 1 features all of the requirements for a BS in CS at the named universtiy. Courses which are prerequisites to requirements are also featured.
	- Each row is a community college. A checkbox is under a course if that CC offers something that articulates to it. 
	- The Lower column is the % of LOWER DIVISION courses that articualte from a communtiy college. The Upper column is the % of ALL courses that articulate. 
	- The MT column is if the community college has a A2B Mapped Standard MassTransfer Articulation Agreement. MT = True; Empty = False
		- haha MT sounds like empty
- OG Work: (Useless) My first stab at this in august 2024. Oh, how naive I was.

##### Colors!
- Yellow: Elective Course
- Red: (just for me) if I havent filled out a course yet.
- Blue: Upper Division
	- Any combination of the primary colors is conjunctive. eg., purple is Unadded *and* Upper Division. 

Green (I like green)
- Green (if in row one): Elective *and* Upper Division
- Green (if in column A): MassTransfer
- Green (else): True

---


# Code

## Pathways
### ch_currcomp.ipynb
### course_distribution.ipynb

## Heatmap

### course_distribution.ipynb
In: The 'Tallys' tab of 'Four-Year Heatmap.xlsx' 
Out: field_distribution.png

### heatmap.ipynb
In: All university tabs of 'Four-Year Heatmap.xlsx' 
Out: 
- lowdiv_heatmap.png (all lower division articulations)
- all_heatmap.png (all lower+upper division articulations)

### masstransfer.ipynb
In: 'Four-Year Heatmap.xlsx' 
- Auto parses just the MassTransfer column from 'Four-Year Heatmap.xlsx' 
Out:  masstransfer.png
