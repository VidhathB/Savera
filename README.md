# Idea for codefundo++ Savera
Savera is a novel approach to disaster recovery for local servers which mainly focuses on drastically reducing server restore times.

## Problem Description
Natural calamities like floods, hurricanes and earthquakes cause huge losses especially to Small to Medium Enterprises. SMEs usually operate only in a few locations; while business assets are commonly localised. Disasters that significantly damage a small business’s assets sometimes prohibit the business from continuing operations. Data being one of the key drivers to businesses in this present era, loss of data or non-operational services can significantly dent turnovers and profits. Savera looks to address this issues in a very cost efficient way, without having to pay for a separate mirror server annually.

## Solution and Working
In the event of a natural calamity, servers placed in unprotected locations like office rooms are susceptible to severe damage and hence loss of data. Savera predicts the oncoming of a calamity that might affect the servers and initiates a high speed data transfer process to the cloud, firstly a machine learning model is run which helps decide which compression algorithm to apply according to the file and is later encrypted before transmission.
This model being the first version, caters only to floods. Flood prediction is done using neural nets which is fed with the following data:
- past data on water level and surges in level 
- past data on surges at different locations i.e estimation of safe levels for each place
- current rainfall level and forecasted values
- sensor data of moisture in server room

If the neural net triggers an interrupt that states the prediction of unsafe conditions, the file transfer process is initiated in the following manner:

![alt text](https://github.com/VidhathB/Savera/blob/master/flowchart1.png)

## Getting Legacy systems onto the Cloud
Enterprises hesitate change due to inertia of going through the process of a paradigm shift from old-school servers to new age cloud technologies. Once the after-effects of the disaster recede and a company is used to cloud based operations, they would never roll back to conventional methods hence pushing the enterprise tech industry.  
   

## Prerequisites
- Previous years rainfall pattern
- Areas(co-ordinates) more susceptible to flooding
- Flask-Python
- Numpy
- CriptIt
- Microsoft Azure Cloud Services

## Usage   
All the client has to do is subscribe to Savera on our website and have the web based application and give file transfer access to Savera services.

## Business Proposition
Natural calamities are a huge burden economically to insurance companies due to the massive scale of damage in the entire city. Therefore risk minimisation becomes very essential for all insurance companies, and a solution which cuts out costs of permanent Data Recovery Centres yet gives the security of data security before a calamity is a win-win situation for both the client and the insurer as the premium cost is reduced while keeping the risk an insurance company has to bear within limits. 

Data stored in central system without any Disaster recovery server facility with data mirroring facility. In case disaster can be predicted in advance, data can be evacuated to a predefined alternate location and the system can be made up and running without any interruption. Even insurers can consider this cost **X** under loss minimisation expenses if the data recovery cost and business interruption costs are insured. 

In case data back-up and recovery systems are not in place, cost of data rebuilding can be insured. Cost of such risk transfer will cost more as the risk is higher. In case of any disaster, cost of data rebuilding, increased cost of working and consequential losses like business interruption losses can be recovered from Insurers which is about **200X**.
