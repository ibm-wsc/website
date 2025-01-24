# SMP/E Current Naming Standards - draft

This page contains current SMP/e standards. 

**This is a work in progress**

For updates create a pull request for your proposed additions/changes. Discussions can be done through issues as required as well. 
## WAZI
### Zone Names
Each major subsytem with version/release will be installed in its own SMP/e zone. This is to prevent deletion of the previous versions. 

HLQ for each product is **Product** + **Version** + **Release**.

Example: 
- z/OS v3.1    = xxx
- Db2 v13      = xxx
- IMS v15.5    = xxx
- CICS v6.2    = xxx

### SMP/E data sets naming standards 

All the SMP/E data sets are NON-SMS managed and are allocated to `xxx*` volumes. 

#### SMP/E zone data sets:
- Naming standards SMP/e Global zone: 
- Naming standards SMP/e Target zone: 
- Naming standards SMP/e Distributed zone: 
- Naming standards SMP/e Install datasets: xxxx

Example Installation Datasets:
- ZO1SMP.SMPPTS          
- ZO1SMP.ZO1T100.SMPMTS  
- ZO1SMP.ZO1T100.SMPSCDS 
- ZO1SMP.ZO1T100.SMPSTS    

**SMP/e Target and DLIB data sets:**

TLIB - `HLQ`.`3 character product prefix`.`S*`    
DLIB - `HLQ`.`3 character product prefix`.`A*`  

> `S*` and `A*` are the normal SMP/e TLIB and DLIB data set defaults

Example: 
- FEK DLIBs - xxx.**.A*
- FEK TLIBs - xxx.**.S*     

**SMP/e zFS data set names:**

ZFS data set name standards are: 
- zOS USS zfs ZT1USS.**.ZFS 
- SMPE zfs ZT1SMP.**.ZFS.

Example: 
- xxxx
 
## SMP/e Directory naming Standards and Structure 

### Mounting and USS directory structures

- Service mountpoint: 
    - /OTHER
- Service mountpoint for /usr/lpp/:
    - /OTHER/usr/lpp/xxx

Examples: 
Please provide two examples of Service mountpoint:
- xxx
- xxx

### SMP/e download directory:
- smpnts
    - /OTHER/smpnts
## ISV
### Zone Names
Each major subsytem with version/release will be installed in its own SMP/e zone. This is to prevent deletion of the previous versions. 

HLQ for each product is **Product** + **Version** + **Release**.

Example: 
- z/OS v3.1    = xxx
- Db2 v13      = xxx
- IMS v15.5    = xxx
- CICS v6.2    = xxx

### SMP/E data sets naming standards 

All the SMP/E data sets are NON-SMS managed and are allocated to `xxx*` volumes. 

#### SMP/E zone data sets:
- Naming standards SMP/e Global zone: 
- Naming standards SMP/e Target zone: 
- Naming standards SMP/e Distributed zone: 
- Naming standards SMP/e Install datasets: xxxx

Example Installation Datasets:
- ZO1SMP.SMPPTS          
- ZO1SMP.ZO1T100.SMPMTS  
- ZO1SMP.ZO1T100.SMPSCDS 
- ZO1SMP.ZO1T100.SMPSTS    

**SMP/e Target and DLIB data sets:**

TLIB - `HLQ`.`3 character product prefix`.`S*`    
DLIB - `HLQ`.`3 character product prefix`.`A*`  

> `S*` and `A*` are the normal SMP/e TLIB and DLIB data set defaults

Example: 
- FEK DLIBs - xxx.**.A*
- FEK TLIBs - xxx.**.S*     

**SMP/e zFS data set names:**

ZFS data set name standards are: 
- zOS USS zfs ZT1USS.**.ZFS 
- SMPE zfs ZT1SMP.**.ZFS.

Example: 
- xxxx
 
## SMP/e Directory naming Standards and Structure 

### Mounting and USS directory structures

- Service mountpoint: 
    - /OTHER
- Service mountpoint for /usr/lpp/:
    - /OTHER/usr/lpp/xxx

Examples: 
Please provide two examples of Service mountpoint:
- xxx
- xxx

### SMP/e download directory:
- smpnts
    - /OTHER/smpnts

## WSC
### Zone Names
Each major subsytem with version/release will be installed in its own SMP/e zone. This is to prevent deletion of the previous versions. 

HLQ for each product is **Product** + **Version** + **Release**.

Example: 
- z/OS v3.1    = xxx
- Db2 v13      = xxx
- IMS v15.5    = xxx
- CICS v6.2    = xxx

### SMP/E data sets naming standards 

All the SMP/E data sets are NON-SMS managed and are allocated to `xxx*` volumes. 

#### SMP/E zone data sets:
- Naming standards SMP/e Global zone: 
- Naming standards SMP/e Target zone: 
- Naming standards SMP/e Distributed zone: 
- Naming standards SMP/e Install datasets: xxxx

Example Installation Datasets:
- ZO1SMP.SMPPTS          
- ZO1SMP.ZO1T100.SMPMTS  
- ZO1SMP.ZO1T100.SMPSCDS 
- ZO1SMP.ZO1T100.SMPSTS    

**SMP/e Target and DLIB data sets:**

TLIB - `HLQ`.`3 character product prefix`.`S*`    
DLIB - `HLQ`.`3 character product prefix`.`A*`  

> `S*` and `A*` are the normal SMP/e TLIB and DLIB data set defaults

Example: 
- FEK DLIBs - xxx.**.A*
- FEK TLIBs - xxx.**.S*     

**SMP/e zFS data set names:**

ZFS data set name standards are: 
- zOS USS zfs ZT1USS.**.ZFS 
- SMPE zfs ZT1SMP.**.ZFS.

Example: 
- xxxx
 
## SMP/e Directory naming Standards and Structure 

### Mounting and USS directory structures

- Service mountpoint: 
    - /OTHER
- Service mountpoint for /usr/lpp/:
    - /OTHER/usr/lpp/xxx

Examples: 
Please provide two examples of Service mountpoint:
- xxx
- xxx

### SMP/e download directory:
- smpnts
    - /OTHER/smpnts

## CPO
### Zone Names
Each major subsytem with version/release will be installed in its own SMP/e zone. This is to prevent deletion of the previous versions. 

HLQ for each product is **Product** + **Version** + **Release**.

Example: 
- z/OS v3.1    = xxx
- Db2 v13      = xxx
- IMS v15.5    = xxx
- CICS v6.2    = xxx

### SMP/E data sets naming standards 

All the SMP/E data sets are NON-SMS managed and are allocated to `xxx*` volumes. 

#### SMP/E zone data sets:
- Naming standards SMP/e Global zone: 
- Naming standards SMP/e Target zone: 
- Naming standards SMP/e Distributed zone: 
- Naming standards SMP/e Install datasets: xxxx

Example Installation Datasets:
- ZO1SMP.SMPPTS          
- ZO1SMP.ZO1T100.SMPMTS  
- ZO1SMP.ZO1T100.SMPSCDS 
- ZO1SMP.ZO1T100.SMPSTS    

**SMP/e Target and DLIB data sets:**

TLIB - `HLQ`.`3 character product prefix`.`S*`    
DLIB - `HLQ`.`3 character product prefix`.`A*`  

> `S*` and `A*` are the normal SMP/e TLIB and DLIB data set defaults

Example: 
- FEK DLIBs - xxx.**.A*
- FEK TLIBs - xxx.**.S*     

**SMP/e zFS data set names:**

ZFS data set name standards are: 
- zOS USS zfs ZT1USS.**.ZFS 
- SMPE zfs ZT1SMP.**.ZFS.

Example: 
- xxxx
 
## SMP/e Directory naming Standards and Structure 

### Mounting and USS directory structures

- Service mountpoint: 
    - /OTHER
- Service mountpoint for /usr/lpp/:
    - /OTHER/usr/lpp/xxx

Examples: 
Please provide two examples of Service mountpoint:
- xxx
- xxx

### SMP/e download directory:
- smpnts
    - /OTHER/smpnts



