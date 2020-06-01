# Exploratory Data Analysis (EDA) Projects of MTA Turnstile Data

This repo contains Project-01 at Istanbul Data Science Academy.

## About MTA

The Metropolitan Transportation Authority is North America's largest transportation network, serving a population of 15.3 million people across a 5,000-square-mile travel area surrounding New York City through Long Island, southeastern New York State, and Connecticut.

The MTA network comprises the nation’s largest bus fleet and more subway and commuter rail cars than all other U.S. transit systems combined. The MTA's operating agencies are MTA New York City Transit, MTA Bus, Long Island Rail Road, Metro-North Railroad, and MTA Bridges and Tunnels. 

## MTA Turnstile Data

Data obtained from http://web.mta.info/developers/turnstile.html. 

### Field Description

C/A,UNIT,SCP,STATION,LINENAME,DIVISION,DATE,TIME,DESC,ENTRIES,EXITS


C/A      = Control Area (A002)<br />
UNIT     = Remote Unit for a station (R051)<br />
SCP      = Subunit Channel Position represents an specific address for a device (02-00-00)<br />
STATION  = Represents the station name the device is located at.<br /> 
LINENAME = Represents all train lines that can be boarded at this station
           Normally lines are represented by one character.  LINENAME 456NQR repersents train server for 4, 5, 6, N, Q, and R trains.<br />
DIVISION = Represents the Line originally the station belonged to BMT, IRT, or IND.<br />     
DATE     = Represents the date (MM-DD-YY).<br />
TIME     = Represents the time (hh:mm:ss) for a scheduled audit event.<br />
DESc     = Represent the "REGULAR" scheduled audit event (Normally occurs every 4 hours).<br /> 
           1. Audits may occur more that 4 hours due to planning, or troubleshooting activities.<br />   
           2. Additionally, there may be a "RECOVR AUD" entry: This refers to a missed audit that was recovered.<br />   
ENTRIES  = The comulative entry register value for a device.<br /> 
EXIST    = The cumulative exit register value for a device.<br /> 



Example:
The data below shows the entry/exit register values for one turnstile at control area (A002) from 09/27/14 at 00:00 hours to 09/29/14 at 00:00 hours<br />


C/A,UNIT,SCP,STATION,LINENAME,DIVISION,DATE,TIME,DESC,ENTRIES,EXITS.<br /> 
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,00:00:00,REGULAR,0004800073,0001629137,<br />    
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,04:00:00,REGULAR,0004800125,0001629149,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,08:00:00,REGULAR,0004800146,0001629162,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,12:00:00,REGULAR,0004800264,0001629264,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,16:00:00,REGULAR,0004800523,0001629328,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-27-14,20:00:00,REGULAR,0004800924,0001629371,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,00:00:00,REGULAR,0004801104,0001629395,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,04:00:00,REGULAR,0004801149,0001629402,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,08:00:00,REGULAR,0004801168,0001629414,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,12:00:00,REGULAR,0004801304,0001629463,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,16:00:00,REGULAR,0004801463,0001629521,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-28-14,20:00:00,REGULAR,0004801737,0001629555,<br />  
A002,R051,02-00-00,LEXINGTON AVE,456NQR,BMT,09-29-14,00:00:00,REGULAR,0004801836,0001629574,<br />  
