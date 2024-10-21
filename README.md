# DCFC_10_HMI
This Repository contains the Project of 10 Inches HMI for the DC Fast Chargers under the Zenergize Power Tech Pvt Ltd.
The Given HMI contains certain improvements to the previous version .

As of the Date 21/10/2024 , the improvements are : 

    Detailed info page code implementation at HMI end
    Instead of keeping code on buttons, we can just send some fixed text to a hidden text field on this page from MCU and implement the same code in the timer.
    Hidden Text field name : ccs (width & height is kept as 2)

    Code Implementation on button clicks: (What MCU will send in ccs.txt)
    Charger Tab clicked = “C1”
    OCPP LCU Tab Clicked = “L1”
    PMU Tab Clicked = “P1”
    Currently left right page toggling is only for Charger configurations (left right clicks and which page to display will be decided by MCU itself):
    For Page 1 = “C1”
    For Page 2 = “C2”
    For Page 3 = “C3” (if there will be any)
    
    Note: Code for PreInitialize event of this page will be same as for “C1” as it is the default page when page opens up. Also if any other pages are added in LCU and PMU configurations, data will be sent in 
    similar pattern later ON
