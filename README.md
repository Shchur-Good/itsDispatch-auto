# ITS Dispatch Automation Suite
(to be) An automation suite for data import and entry into [ITS Dispatch](http://itsdispatch.com).

## Motivation
ITS Dispatch, in all it's greatness (none really) has no ability to import data from outside sources. This means that data from one websystem can't be transfered to it in any way but manual copy-paste entry. This means, that for large fleets, transfering transaction and bank data from one system to ITS Dispatch can take hours if not longer and many people. This piece of software aims to automate this process so that the job of many can be completed by one in mere minutes.

## Technology
Current functionality will include the import of data from Fleet One Truck Fuel Banking system and then automatic entry into the IFTA systems of ITS Dispatch.

This will be done by downloading transaction data from the bank, parsing it into objects, then finding elementsByID within ITS Dispatch and inputing data into it using JavaScript. 

The reseason JavaScript is chosen is because of it's cross-platform nature and the fact that this is a bridge between webapps. This software needs to be able to work on multiple platforms and be very userfriendly. Because of this, I plan to use ElectronJS as an OS wrapper bridge to allow it to work like a desktop app on any computer.

## TODO

Once transaction import is complete, adding ability to export and parse data from ITS Dispatch would be useful, as well as adding tools to consolidate data and get statistics. 

Building a set of tools to help do certain tasks would also be very useful, such as implementing PDF OCR systems to parse rate confirmations from common companies so that manual entry of data can be automated.
