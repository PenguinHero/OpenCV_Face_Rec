# OpenCV Face Recognition

This repositiry is a modified copy of the code that can be found at: https://www.pyimagesearch.com/2018/09/24/opencv-face-recognition/

It uses OpenCV (plus a few other libraries) to build a solution that uses images to do face recognition for both still frame and video.
It does this without using dlib, and instead uses 128-d face embeddings and a Support Vector Machine (SVM).

Lots of details about how it works can be found at that site.

There is a large (30MB) file that you need for the extract/embedding/train sequence (but not the recognise, I believe) which is too big to upload here. You will need to get it from a source code option from the above site, or perhaps download it from somewhere else.
The file is called: openface_nn4.small2.v1.t7 and should be placed in the same (parent) folder as the python files.

Note that all my libraries were installed using PIP3 and I ran all my code as Python3.
If you wish to do this then when the web site gives instructions to run Python from the command line either add the digit 3 to the Python, or run it from a Python3 IDE like Thonny and include your run time arguments to match what is supplied on the web site.

Finally, I wrote this to run on my Raspberry Pi 3B+, and it does run well for everything except the real-time video recognition.
That runs at just under a frame per second. It works, detecting faces, just very slowly.
If you read the comments at the bottom of the site someone asks about this, and the author suggests using his instructions that are specifically for the Pi: https://www.pyimagesearch.com/2018/06/25/raspberry-pi-face-recognition/
This uses Haar cascades and dlib.
I had tried to use that approach before using this one, but I couldn't get the face_regognition libraray to install, but I'll have another go now that I understand more about installing troublesome libs on the Pi.
If I get it working I'll post that code here on GitHub too.
