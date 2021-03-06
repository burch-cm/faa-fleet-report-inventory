# FAA Fleet Inventory Report  

***
## Report Information

<div class="attribute-table" id="info-table">

Attribute | Value
--------- | ------
**Name** | Leased and Owned Inventory by LOB</br>Leased and Owned Inventory Baseline Comparison
**Frequency** | monthly
**Location** | [KSN Fleet Management Reporting](https://ksn2.faa.gov/arc/arc/Logistics/alo400/FleetMgmt/SitePages/Reporting.aspx)<br/>[FAA Fleet Reporting](https://ksn2.faa.gov/arc/arc/Logistics/alo400/FleetMgmt/FleetReporting/SitePages/Documents.aspx)  
**Owner Office** | FAA APM-400 Fleet Manager
**Owner Name** | Eugene Tumblin (OST)
**Admin Name** | Christopher Burch (CTR)
**Admin Email** | \<email>

</div>

## Report Purpose  
The FAA Leased and Owned Inventory by LOB is a monthly inventory report of *on road reportable* motor vehicles, and includes information on vehicle VIN, tag, mileage, location, and contact information. It is used to manage current inventory levels and determine if any vehilces may be underutilized in their current roles.  
The FAA Leased and Owned Inventory and Baseline Comparison report looks at current *on road reportable* motor vehicle inventory levels compared with a baseline inventory from FY2015. This report is used to mesure FAA Fleet progress against fleet size reduction goals.

## Linked Reports  

<div class="attribute-table" id="linked-table">

Upstream | Downstream
--- | ---
None | [FAA Fleet Low Utilization Report](https://github.com/burch-cm/faa-fleet-report-low-utilization)<br/>[FAA Fleet Fuel Use Report](https://github.com/burch-cm/faa-fleet-report-fuel-use)<br/>[FAA Fleet CRASH Report](https://github.com/burch-cm/faa-fleet-report-crash)

</div>

<div id="input-tables">

 ## Inputs  

 #### Input  

<div class="attribute-table">

 Attribute | Value
 --- | ---
 **Name** | Customized Inventory Report by Agency
 **File Type** | CSV
 **Origin** | GSA Drive Thru
 **Filename** | Customized_Inventory_Report_Agency_069_Bureau_05.csv  
**Link** | https://drivethru.gsa.gov

</div>

</div>

## Report Procedures
FAA Fleet Inventory reports are currently generated using automated scripts located in the [FAA Fleet Report Tools repo](https://github.com/burch-cm/faa_fleet_reports). Currently, the inventory is generated via [R](https://www.r-project.org) scripts in a [Shiny](https://shiny.rstudio.com) web interface.  

Procedures for manually generating the report can be found in the [FAA Fleet Reports Process](https://github.com/burch-cm/faa-fleet-report-inventory/docs/FAA_Fleet_Reports_Process.docx). This document is out of date but can be used to generate the report if automated tools are not available.
