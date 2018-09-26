This Smith_DairyCoinfection_Readme.txt file was generated on 20171211 by Rebecca Lee Smith


-------------------
GENERAL INFORMATION
-------------------


1. Title of Dataset 
DairyCoinfection

2. Author Information


  Principal Investigator Contact Information
        Name: Rebecca Lee Smith
           Institution: University of Illinois College of Veterinary Medicine
           Address: 2001 S Lincoln Ave, VM BSB 2627, Urbana IL 61801
           Email: rlsdvm@illinois.edu


3. Date of data collection (single date, range, approximate date) 
20170130 to 20170831


4. Geographic location of data collection (where was data collected?): 
Northwestern Illinois, on two separate commercial dairy herds

5. Information about funding sources that supported the collection of the data:
funded by USDA-NIFA Hatch funds, ILLU-888-934



--------------------------
SHARING/ACCESS INFORMATION
-------------------------- 


1. Licenses/restrictions placed on the data: CC BY


2. Links to publications that cite or use the data:none


3. Links to other publicly accessible locations of the data:none


4. Links/relationships to ancillary data sets:none


5. Was data derived from another source? no


6. Recommended citation for the data:




---------------------
DATA & FILE OVERVIEW
---------------------


1. File List
   A. Filename: DiagnosticResultsAll.csv       
      Short description:        
	All results from diagnostic testing throughout the study. 

        
   B. Filename: ProductionResultsBefore.csv       
      Short description:        
	Animal production data as of 20161017, prior to diagnostic testing. 

        
   C. Filename: ProductionResultsAfter.csv       
      Short description:
	Animal production data as of 20171026, after diagnostic testing. 

2. Relationship between files:        
	Animal key is a combination of BarnName and Herd. Not all animals in DiagnosticResultsAll.csv have records in both production results files.



3. Additional related data collected that was not included in the current data package: PCDart files are not included




4. Are there multiple versions of the dataset? yes, there is one previous version






--------------------------
METHODOLOGICAL INFORMATION
--------------------------


1. Description of methods used for collection/generation of data: 
	Production results were downloaded from PCDart on the dates listed, and are based on the most recent DHIA test day.
	Diagnostic results were produced by analysis of serum at the University of Illinois Animal Diagnostic Laboratory using standard methodologies. 
	See metadata for details.


2. Methods for processing the data: Diagnostic results were collated from laboratory reports. Production results were not processed.


3. Instrument- or software-specific information needed to interpret the data: See metadata for details on testing methods. All tests were based on the standard methodologies of the University of Illinois Animal Diagnostic Laboratory in 2017.


4. Standards and calibration information, if appropriate: NA


5. Environmental/experimental conditions: All sera were collected from the coccygeal vein in a red-top tube and transported on ice to the animal diagnostic laboratory within 24 hours.


6. Describe any quality-assurance procedures performed on the data: All data were reviewed by the primary investigator.


7. People involved with sample collection, processing, analysis and/or submission: 
	Dr. Gianluigi Rossi: sample collection and collation of laboratory data
	Dr. Rebecca Smith: collection of production results




-----------------------------------------
DATA-SPECIFIC INFORMATION FOR: DiagnosticResultsAll.csv
-----------------------------------------


1. Number of variables: 14


2. Number of cases/rows: 415


3. Variable List
    A. Name: Herd
       Description: Identifies which of the two herds the animal belongs to
	Value labels: text, M or B

    B. Name: Day
       Description: Date of sampling
	Value labels: date, in M/D/YYYY format

    C. Name: Day_j
       Description: numeric version of date of sampling, with 30 being 2017/01/30
	Value labels: numeric, day

    D. Name: BarnName
       Description: name of animal	
	Value labels: text

    E. Name: Lactation
       Description: parity of animal at time of sampling
	Value labels: numeric, between 1 and 3

    F. Name: BLV
       Description: results of detection of antibodies to Bovine Leukosis Virus per ELISA test, based on 1.0 ml serum
	Value labels: text, NEGATIVE or POSITIVE

    G. Name: BLV_bin
       Description: numeric version of BLV
	Value labels: numeric, 0=NEGATIVE, 1=POSITIVE

    H. Name: MAP
       Description: results of detection of antibodies to Mycobacterium avium subsp. paratuberculosis per ELISA test, based on 2.0 ml serum
	Value labels: text, NEGATIVE or POSITIVE

    I. Name: MAP_bin
       Description: numeric version of MAP
	Value labels: numeric, 0=NEGATIVE, 1=POSITIVE

    J. Name: NEOS
       Description: results of detection of antibodies to Neospora caninum per ELISA test, based on serum
	Value labels: text, NEGATIVE or POSITIVE

    K. Name: NEOS_bin
       Description: numeric version of NEOS
	Value labels: numeric, 0=NEGATIVE, 1=POSITIVE

    L. Name: IBR_titer
       Description: results of a Bovine Herpesvirus type 1 serum neutralization screen assay, based on 1.0 ml serum	
	Value labels: numeric, titer of 1:[value], with values between 4 and 256. Negative means no effective titer.

    M. Name: BVD1_titer
       Description: results of a Bovine Viral Diarrhea Virus type 1 serum neutralization screen assay, based on 1.0 ml serum	
	Value labels: numeric, titer of 1:[value], with values between 4 and 256. Negative means no effective titer.

    N. Name: BVD2_titer
       Description: results of a Bovine Viral Diarrhea Virus type 2 serum neutralization assay, based on 1.0 ml serum	
	Value labels: numeric, titer of 1:[value], with values between 4 and 256. Negative means no effective titer.


4. Missing data codes:
       NA        not available; in the case of diagnostic results, not performed





-----------------------------------------
DATA-SPECIFIC INFORMATION FOR: ProductionResultsBefore.csv
-----------------------------------------


1. Number of variables: 14


2. Number of cases/rows: 282


3. Variable List
    A. Name: BarnName
       Description: name of animal	
	Value labels: text

    B. Name: Herd
       Description: Identifies which of the two herds the animal belongs to
	Value labels: text, M or B

    C. Name: Lactation
       Description: parity of animal at time of sampling
	Value labels: numeric

    D. Name: LctAvSCCAct
       Description: Average somatic cell count over all DHIA test days in the current lactation
	Value labels: numeric

    E. Name: Proj305MEM
       Description: Projected 305-day mature equivalent milk production at most recent DHIA test day
	Value labels: numeric

    F. Name: Proj305MEFCM
       Description: Projected 305-day mature equivalent fat-corrected milk production at most recent DHIA test day
	Value labels: numeric


    G. Name: Proj305MEECM
       Description: Projected 305-day mature equivalent energy-corrected milk production at most recent DHIA test day
	Value labels: numeric


    H. Name: Proj305MEP
       Description: Projected 305-day mature equivalent protein production at most recent DHIA test day
	Value labels: numeric

    I. Name: Proj305MEF
       Description: Projected 305-day mature equivalent fat production at most recent DHIA test day
	Value labels: numeric

    J. Name: ProjClvInt
       Description: Projected calving interval for current lactation at most recent DHIA test day
	Value labels: numeric

    K. Name: TmsBrd
       Description: Number of times animal has been bred during current lactation
	Value labels: numeric

    L. Name: YldDevM
       Description: Difference between Proj305MEM and herd average Proj305MEM at most recent DHIA test day
	Value labels: numeric

    M. Name: YldDevP
       Description: Difference between Proj305MEP and herd average Proj305MEP at most recent DHIA test day
	Value labels: numeric

    N. Name: YldDevF
       Description: Difference between Proj305MEF and herd average Proj305MEF at most recent DHIA test day
	Value labels: numeric



4. Missing data codes:
        NA        Not available





-----------------------------------------
DATA-SPECIFIC INFORMATION FOR: ProductionResultsAfter.csv
-----------------------------------------
<create sections for each dataset (or file if appropriate) included>


1. Number of variables: 274


2. Number of cases/rows: 14


3. Variable List
    A. Name: BarnName
       Description: name of animal	
	Value labels: text

    B. Name: Herd
       Description: Identifies which of the two herds the animal belongs to
	Value labels: text, M or B

    C. Name: Lactation
       Description: parity of animal at time of sampling
	Value labels: numeric

    D. Name: LctAvSCCAct
       Description: Average somatic cell count over all DHIA test days in the current lactation
	Value labels: numeric

    E. Name: Proj305MEM
       Description: Projected 305-day mature equivalent milk production at most recent DHIA test day
	Value labels: numeric

    F. Name: Proj305MEFCM
       Description: Projected 305-day mature equivalent fat-corrected milk production at most recent DHIA test day
	Value labels: numeric


    G. Name: Proj305MEECM
       Description: Projected 305-day mature equivalent energy-corrected milk production at most recent DHIA test day
	Value labels: numeric


    H. Name: Proj305MEP
       Description: Projected 305-day mature equivalent protein production at most recent DHIA test day
	Value labels: numeric

    I. Name: Proj305MEF
       Description: Projected 305-day mature equivalent fat production at most recent DHIA test day
	Value labels: numeric

    J. Name: ProjClvInt
       Description: Projected calving interval for current lactation at most recent DHIA test day
	Value labels: numeric

    K. Name: TmsBrd
       Description: Number of times animal has been bred during current lactation
	Value labels: numeric

    L. Name: YldDevM
       Description: Difference between Proj305MEM and herd average Proj305MEM at most recent DHIA test day
	Value labels: numeric

    M. Name: YldDevP
       Description: Difference between Proj305MEP and herd average Proj305MEP at most recent DHIA test day
	Value labels: numeric

    N. Name: YldDevF
       Description: Difference between Proj305MEF and herd average Proj305MEF at most recent DHIA test day
	Value labels: numeric


4. Missing data codes:
        NA        Not available


