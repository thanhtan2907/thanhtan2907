import cv2
import numpy as np


# from cv2 import VideoWriter
# from cv2 import VideoWriter_fourcc

# # open the webcam video stream
webcam = cv2.VideoCapture(0)

# # open output video file stream
# video = VideoWriter('webcam.avi', VideoWriter_fourcc(*'MP42'), 25.0, (640, 480))

# # main loop
while True:
#     # get the frame from the webcam
     ret, frame = webcam.read()
     cv2.imshow('frame', frame)

     if cv2.waitKey(1) == ord('q'):
         break#     # if webcam stream is ok
#     if stream_ok:
#         # display current frame
#         cv2.imshow('Webcam', frame)
        
#         # write frame to the video file
#         video.write(frame)

#     # escape condition
#     if cv2.waitKey(1) & 0xFF == 27: break

# # clean ups


# # release web camera stream
webcam.release()
cv2.destroyAllWindows()

# # release video output file stream
# video.release()
