# FAA Fleet Inventory Report  

***
## Report Information

#### Report Name(s)  
* Leased and Owned Inventory by LOB  
* Leased and Owned Inventory Baseline Comparison  

#### Frequency  
Monthly  

#### Location  
* *Internal*: [KSN Fleet Management Reporting](https://ksn2.faa.gov/arc/arc/Logistics/alo400/FleetMgmt/SitePages/Reporting.aspx)  
* *External*: [FAA Fleet Reporting](https://ksn2.faa.gov/arc/arc/Logistics/alo400/FleetMgmt/FleetReporting/SitePages/Documents.aspx)  

#### Owner Office  
FAA APM-400 Fleet Manager

#### Report Owner  
Eugene Tumblin (OST)  

#### Report Admin/POC
Christopher Burch (CTR)  

#### Admin Email  
christopher <dot> m-ctr <dot> burch <at> faa <dot> gov  

## Report Purpose  
The FAA Leased and Owned Inventory by LOB is a monthly inventory report of *on road reportable* motor vehicles, and includes information on vehicle VIN, tag, mileage, location, and contact information. It is used to manage current inventory levels and determine if any vehilces may be underutilized in their current roles.  
The FAA Leased and Owned Inventory and Baseline Comparison report looks at current *on road reportable* motor vehicle inventory levels compared with a baseline inventory from FY2015. This report is used to mesure FAA Fleet progress against fleet size reduction goals.

***

## References  

### Upstream Reference  
*If this report requires another prepared report as input, list that here.*    
**Required Reports**: None

### Downstream Reference  
*List all reports which use this report as an input and which may be affected by changes in this report.*    
* [FAA Fleet Low Utilization Report](https://github.com/burch-cm/faa-fleet-report-low-utilization)  
* [FAA Fleet Fuel Use Report](https://github.com/burch-cm/faa-fleet-report-fuel-use)  
* [FAA Fleet CRASH Report](https://github.com/burch-cm/faa-fleet-report-crash)

***

## Report Inputs  

#### Input  
	**Name**: Customized Inventory Report by Agency  
	**File Type**: CSV  
	**Origin**: GSA Drive Thru  
	**Filename**: Customized_Inventory_Report_Agency_069_Bureau_05.csv  
	**Link**: https://drivethru.gsa.gov  

#### Input  
   **Name**: MVS All Vehicle Inventory  
   **File Type**: XLSX  
   **Origin**: FAAMVS  
   **Filename**: AllVehicleInventory.xlsx  
   **Link**: https://mvs.faa.gov  

#### Input  
	**Name**: Delphi Datastring by Tag  
	**File Type**: XLSX  
	**Origin**: FAAMVS  
	**Filename**: DelphiDatastringByTag.xlsx  
	**Link**: https://mvs.faa.gov  

#### Input  
	**Name**: Fuel Use Report  
	**File Type**: CSV  
	**Origin**: GSA Drive Thru  
	**Filename**: FUR-G-Summary-Vehicle-for-069-05.csv  

#### Input  
	**Name**: MVS Owned Mileage  
	**File Type**: CSV  
	**Origin** FAAMVS  
	**Filename**: \<Month>\<Year>FAAMileage.csv  

#### Input  
	**Name**: MVS Leased Mileage  
	**File Type**: CSV  
	**Origin** FAAMVS  
	**Filename**: \<Month>\<Year>GSAMileage.csv  

***

## Report Procedures
FAA Fleet Inventory reports are currently generated using automated scripts located in the [FAA Fleet Inventory Report Tool repo](https://github.com/burch-cm/faa_fleet_inventory). Currently, the inventory is generated via [R](https://www.r-project.org) scripts in a [Shiny](https://shiny.rstudio.com) web interface.  

Procedures for manually generating the report can be found in the [FAA Fleet Reports Process](https://github.com/burch-cm/faa-fleet-report-inventory/docs/FAA Fleet Reports Process.docx). This document is out of date but can be used to generate the report if automated tools are not available.
