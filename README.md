# AutoLog: Smart Vehicle Parking System

Final project for the Building AI course  
Building AI course project

## Summary

AutoLog is an AI-powered system that automates vehicle identification and parking logging. It captures license plates, calculates fees, and stores data efficiently, reducing human effort and errors in parking management.

## Background

This project solves common parking issues, such as manual logging delays and fee calculation mistakes.  
Motivation: simplify daily parking operations and improve accuracy.  
Importance: provides real-time vehicle tracking and secure data management.

* Manual vehicle logging is slow
* Fee calculation errors are frequent
* Real-time tracking is difficult

## How is it used?

AutoLog captures vehicle information using cameras at parking entrances. The system uses OCR to identify license plates, calculates fees based on duration, and stores logs in a secure database.  

Users: Parking facility staff, security personnel, and management.  

![Parking Camera](images/parking_camera.jpg)

Example code:
from autolog import ParkingSystem

ps = ParkingSystem()
ps.capture_vehicle("ABC-123")
ps.calculate_fee("ABC-123")
ps.generate_report()


## Data sources and AI methods

Data is collected through live camera feeds. OCR and image processing models are used for license plate recognition. Python, OpenCV, and Tesseract are the primary tools.

[OpenCV](https://opencv.org)  
[Tesseract OCR](https://github.com/tesseract-ocr/tesseract)

| Syntax      | Description |
| ----------- | ----------- |
| OCR Model   | Recognizes license plates from images |
| Database   | Stores vehicle logs, timestamps, and fees |

## Challenges

* Lighting conditions and blurry images may reduce OCR accuracy
* Privacy concerns when collecting vehicle data
* System requires proper hardware for real-time operation

## What next?

* Integrate predictive analytics for peak-time management  
* Add mobile notifications for users  
* Expand to multiple parking facilities with cloud sync

## Acknowledgments

* Project template provided by Building AI course (Reaktor & University of Helsinki)  
* [OpenCV](https://opencv.org) and [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)  
* Parking camera image by Umberto Salvagnin / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
