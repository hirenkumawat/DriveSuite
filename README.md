# DriveSuite

Application Suite to prevent distracted driving.  
Created for TeenHacks LI Hackathon in April 2019.  
**Team Members: Hiren Kumawat, Jeremy Kim, Danyil Blyschak, Nishanth Araveti, Michael Chan.**  
***For more information, see https://devpost.com/software/drivesuite.***  
 
Included: 
* GestureSoftware application: Python application enabling users to accept or reject incoming calls with hand gestures detected by a Leap Motion Controller sensor.
* DistractedDriver application: iOS application to detect distracted drivers using CoreML and Apple's Vision API.

**How we built it** (more info on [Devpost](https://devpost.com/software/drivesuite))  
> We built the app using CoreML. I used transfer learning to finetune a Resnet 50 network and then exported it to CoreML. I then used Apple's Vision API and AVFoundation and AVKit to process video frames and then run each frame through the deep learning model to provide live predictions of whether or not a person is distracted while driving or not. Some examples of being distracted would be if a person is texting, or doing their hair/makeup, or talking with a different person. We trained our deep learning model with a dataset from StateFarm. The involvement of a major insurance company as StateFarm demonstrates how critical of an issue driver safety is for insurance companies and the general public. We also hosted our data with Microsoft Azure. We proceeded to build an app so that our software would be highly scalable. After developing our app, we decided that we should tackle this challenge even more and moved to develop a suite of applications. As a result, we used the LeapMotion sensor to track hand motions. Our hands are one of the most versatile and expressive organs and utilizing this agility would be helpful in enabling the driver to communicate with technology around them in a more efficient way. For instance, a key product we developed with LeapMotion was automated call rejection and acceptance. We used the Twilio API to automate sending calls and with very intuitive grasping and release motions, we are able to send and decline calls. This efficiency enables the driver to focus on driving and not getting into accidents.Ideally, we wanted our project to use both positive, and negative reinforcement in preventing Driver Distraction. The alarm and AI monitoring would deter future transgressions via negative reinforcement and the minimally invasive, hands-free driver user interface would prevent both the need and the motive for being distracted in the first place.
