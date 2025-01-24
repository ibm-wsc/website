# SMP/E Zones Current Standards - draft

This page contains current SMP/e standards. 

This page was developed during the Meeting from Dec 9, 2024 

**This is a work in progress**

For updates create a pull request for your proposed additions/changes. Discussions can be done through issues as required as well. 

## Terms
### SMPE Base z/OS image:
- ISV: what is shipped from shopz for base z/OS + MQ
- WSC: what is shipped from shopz base z/OS + freq asked for products ie( IDz )
- CPO: what is shipped from shopz base z/OS + freq asked for products ie( IDz )
- WAZI: what is shipped from shopz for base z/OS 

### Standard Running z/OS Base image:
- ISV: All in one image 
- WSC: zOS Target 
- CPO: zOS Target
- WAZI: Stock image 

## SMPE 
### Global zones:

#### WAZI: 7ish (only supporting latest version for the most part )
- z/OS 
    - ZOS31 tlib/dlib
- Program products
    -   compliers, misc
- Middleware
    - DB2
    - CICS
    - IMS
    - MQ
    - Datagate
    - WAS 
#### ISV:  200+ gloabl zone  ---- does support early code pre-ga + IESP
- ZOS24
    - tlib zos / dlib zos
    - tlib mq / dlib mq
- ZOS25
    - tlib zos / dlib zos
    - tlib mq / dlib mq
- ZOS31
    - tlib zos / dlib zos
    - tlib mq / dlib mq
- Program products 
    - 1 global per product
- DB2v12
    - 1 version per global
- DB2v13
- CICS63
- CICS64
- IMS
- WAS
#### WSC: IESP zOS
- ZOS
    - zos25 target
    - zos31 target 
- Program products
    - 1 global per product
- Db2 
    - db2v12 tlib / dlib
    - db2v13 tlib / dlib
- CICS
    - cics63 tlib / dlib
- IMS
- MQ
- WAS
#### CPO: 28 ish csi ----- IESP
- ZOS25
- ZOS31 
- Db2
- CICS
- IMS
- MQ
- ADFz global zone seperate for versions
- WAS

### What is included in the image:
- WAZI:
    - Tlib/dlib & CSI --- rdrw
- ISV:
    - Tlib/dlib & CSI and SMP dataset --- read only
- WSC:
    - tlib only for all,  csi for zos, provide holddata and listptf for products --- read only
- CPO:
    - Tlibs/dlibs 

### Freq for maint - NO PE always
- WAZI:
    - zOS: qtrly
    - Program Products: qtrly
    - Subsystem: qtrly
- ISV:
    - Rec is when notification of next RSU - Monthly
    - RSU Levels for all zone - monthly
    - Holddata - impacts apply & RSU
- WSC:
    - Rec is before monthly app
    - zOS: monthly - RSU level
    - Program Products: qtrly 
    - Subsystem: request bases and at time of request pull latest RSU level
- CPO:
    - Rec weekly 
    - Weekly
    - Rec/App all!!!

### Freq of deploy:
- WAZI:
    - New image qtrly, all exisiting image would need to migrate to new image
- ISV:
    - Monthly - included IPL
    - Recycle every 2 weeks on Sunday ( excluding Dec)
- WSC:
    - zos & Products 
        - Monthly to ztx test system - ipl
        - Next month to ESYS production  - ipl
    - zos
        - all other systems qtly 
    - Products 
        - All other system are to be requested for maint - 
- CPO
    - zos
        - monthly a day or two after RSU
    - Subsys 
        - upon request.


### ++Usermods/APARS/Early PTF(Non GA) - to Standard Running z/OS Base image:
- WAZI:
    - ++Usermods: None
    - APARS: if needed
    - Early PTF: if need
- ISV
    - ++Usermods: None 
    - APARS: Only if impacting many ISV 
    - Early PTF: only if impacting many ISV
    - Exception will apply APAR/ early PTF to keep ISV up
- WSC
    - ++Usermods: None
    - APARS: as requested 
    - Early PTF: as requested
- CPO
    - ++Usermods: Yes, not in SMPE Base z/OS image: only on Standard Running z/OS Base image clone
    - APARs: as requested
    - Early PTFs: as requested

### Service on live system
- WAZI:
    - NO
- ISV
    - NO
- WSC
    - NO
- CPO
    - NO


