# FACE-An-assistive-device-for-face-recognition
 

The original idea for the FACE project was inspired by a difficulty experienced by a significant portion of the population: meeting a new person, then soon after forgetting their name. This common scenario takes place many times throughout the course of a year; attending business conferences, going to a wedding, meeting new people at a workplace or in school, and getting to know people at various other gatherings. While this may seem like a minor inconvenience, easily solvable by nametags or mental training, the problem is much more widespread across the world than it would first appear. After further researching the problem, we came across several articles discussing variation in the ability to remember faces and names between different individuals. While some people have good facial memory, and others have poor facial memory, there also exists a portion of the population that has a complete inability to remember faces. Several research articles and survey surmise that around 2% of the population experiences total face blindness, a disability called prosopagnosia. While memorization techniques may work for most people and a nametag might be given to conference members, these are not universal solutions. An individual will not wear a nametag while roaming around in public, and memorization techniques require time and focus. One suffering from prosopagnosia has difficulty remembering faces all the time, not just at specific events. Further compounding the issue is the current pandemic and the resultant widespread use of facemasks, making facial identification a greater challenge even to the general public. 

Therefore, we decided to design a technological solution to alleviate the effects of face blindness, poor name recall, and masking. The function of our prototype FACE is simple, it recognizes the target person, and conveys the name of the detected person to the user. Additionally, our prototype should be intuitive, unobtrusive, reliable, cost-effective, and usable in multiple scenarios. Our proposal was designed with these requirements in mind, and we believe it effectively meets them. 

Our product is composed of three basic parts: the camera, the microprocessor, and a phone application. The camera is clipped on to the user's glasses and provides a continuous live video feed to the microprocessor. The microprocessor runs code built off the OpenCV framework to analyze the video feed and identify faces. If a face can be matched to the microprocessor's pre-built face database, the identity will then be sent to a web server, and then the respective person’s name would be given as an output to an app installed on the user's phone. FACE has two basic modes that can be toggled between via a button found on the hip unit; continuous and triggered. In continuous mode, the microprocessor code constantly searches for faces, and sends any matched names to be displayed in the phone app. In triggered mode, the microprocessor stays idle unless another button is pressed, after which the code begins to search for a face. After a face is found in triggered mode, the results are displayed on the phone app, and the code returns to idle mode. 

the dataset for the project is removed due to privacy issues

to operate this system 
import the each persons images with different angle atleast 20 image per person in a folder 
for masked people use MASK folder with name
then train the algorithm 
then test out on random images


For accuracy and efficiency, we took 20 images from each person and ran them through our system out of which most of the results were good.  

With the above figures in mind, we go 87.5 percent accuracy with still images. This result is also depended on the tested image as most of the image were taken with straight orientation, which is beneficial to the face recognition system. 

For masked face detection testing we took 5 images per person, and we got an average of 3 to 4 detection per person overall with accuracy of 70 percent. 

For video-based testing we randomly took 5 min of footage and checked how many faces it recognized correctly. In the first few seconds after the camera is first turned towards a person, face recognition is mostly inaccurate due to the camera lag, and camera movement and resulting blur. However, after a few seconds of stabilization we were able to reach 70 percent efficiency, as we also considered pre stabilization faces in checking the algorithm. 

The biggest limitation of this system is face alignment; as the target face tilts away from looking straight on at the camera, the accuracy of the model decreases. 
