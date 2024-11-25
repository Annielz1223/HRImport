# Employee Import Project

This project is used to import employees from client's system to Vault system.

## Features

WonderHealth Inc. will provide the employee data files based on different departments of WonderDrugs, WonderPharma and WonderBio. 
The import process will get the employee files, validate the employees and import the employees to Vault system.

## Technologies Used

- Java 17
- SpringBoot
- AWS
- Gradle

## Design Architecture

![image](https://github.com/user-attachments/assets/04ce4e8d-0b79-4d28-9a79-4d2c944736e7)

## Basic Workflow

![image](https://github.com/user-attachments/assets/da47d102-4acf-4761-9226-ad377131455a)

![image](https://github.com/user-attachments/assets/8e1f7735-712a-4517-aa83-a371455fdaf5)


## Dependency

There is another git repository for the event handler used by Lambda function based on the design architecture. Refer to for the code of event handler by below link.
- https://github.com/Annielz1223/ScheduledEventHandler
- This event handler will be triggered on a fixed time on a daily basis. And it will check if there are new employee data files uploaded to S3 or not. The batch job will be triggered when new file(s) are detected.

## More Information

For more information of this design, please refere to https://www.yuque.com/annie-a58a0/wddtft/ggz020gyrf8n1zga#msqDX.
