### Data Preparation
* Data loading and inspection

---

### Data Cleaning / Processing
* Handled missing values
    * Found blanks in 'Carriageway_Hazards', 'Road_Surface_Conditions', 'Road_Type', 'Weather_Conditions', and 'Time' fields
* Handled incorrect data
    * Found typos in 'Junction_Control' and 'Accident_Severity' field
* Properly formatting data
    * 'Accident Date' field to 'YYYY-MM-DD'
    * 'Time' field to military time
* Extracted month and year value from 'Accident Date' field to use in analysis

---

### Exploratory Data Analysis
* EDA involved exploring the accidents data to answer key questions such as:
    * Total Casualties
    * Total Casualties & Percentage with respect to:
        * Accident severity
        * Vehicle type
    * Total Casualties with respect to vehicle type
    * Monthly trend comparing casualties for current and previous year
    * Casualties by road type
    * Total casualties by road surface
    * Relation between casualties by area / location & day/night

---

### Data Analysis
#### KPI
![KPI](KPI.png)

#### Dashboard
![Dashboard](Dashboard.png)

### EDA Results
|Total Casualties|
|---|
|417883|

---

* Total Casualties with respect to accident severity
<table>
<tr><th>Fatal</th><th>Serious</th><th>Slight</th></tr>
<tr><td>

|Severity|Total|Percentage|
|--|--|--|
|Fatal|7135|1.7%|
|Other|410748|98.3%|

</td><td>

|Severity|Total|Percentage|
|--|--|--|
|Serious|59312|14.2%|
|Other|358571|85.8%|

</td><td>

|Severity|Total|Percentage|
|--|--|--|
|Slight|351436|84.1%|
|Other|66447|15.9%|
</td></tr></table>

---

* Total Casualties & Percentage with respect vehicle type

|Vehicle Type|Casualties|Percentage|
|---|---|---|
|Agricultural_vehicle|1032|0.2%|
|Cars|333485|79.8%|
|Bus|12798|3.1%|
|Van|33472|8.0%|
|Bike|33672|8.1%|
|Others|3424|0.8%|

---

* Monthly trend comparing casualties for current and previous year
<table>
<tr><th>2021</th><th>2022</th></tr>
<tr><td>

|Month|Casualties|
|---|---|
|Jan|18173|
|Feb|14648|
|Mar|17815|
|Apr|17335|
|May|18852|
|Jun|18728|
|Jul|19682|
|Aug|18797|
|Sep|18456|
|Oct|20109|
|Nov|20975|
|Dec|18576|

</td><td>

|Month|Casualties|
|---|---|
|Jan|13163|
|Feb|14804|
|Mar|16575|
|Apr|15767|
|May|16775|
|Jun|17230|
|Jul|17201|
|Aug|16796|
|Sep|17500|
|Oct|18287|
|Nov|18439|
|Dec|13200|
</td></tr></table>

---

* Casualties by road type

|Road_Type|Casualties|
|---|---|
|Unknown|1.9K|
|Slip road|4.7K|
|One way street|7.4K|
|Roundabout|26.8K|
|Dual carriageway|67.4K|
|Single carriageway|309.7K|

---

* Total casualties by road surface

|Road_Surface|Casualties|
|---|---|
|Dry|279445|
|Unknown|396|
|Wet|115261|
|Snow/Ice|22781|

---

* Relation between casualties by area/location & day/night
<table>
<tr><th>Area</th><th>Light_Conditions</th></tr>
<tr><td>

|Area|Casualties|
|---|---|
|Rural|162.0K|
|Urban|255.9K|

</td><td>

|Light_Conditions|Casualties|
|---|---|
|Daylight|305.0K|
|Dark|112.9K|

</td></tr></table>

---