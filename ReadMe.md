Striders
---
Android application
- Transferring acceleration data
Android sends real-time acceleration values ​​to Windows server via Bluetooth communication.

- Get approval from the server
Waits for an approval signal from the server. Then stores the identification parameter received from the server. 



Windows server
- Communicate with android using bluetooth
It configures communication channels with various Android.

- Storing and managing data by device ID 
Configure a profile to manage acceleration data for each device. Contrast with profile when connecting device.

- Pass the parameters to the deep learning server
Pass the parameters to the deep learning server. Choose whether to create a profile or identify this device.



Deep learning server
- Build the learner
Data was processed with test set and test label to learn the matrix of acceleration values.

- Saving and loading learned models 
Store the learned model to save time and recall it when each device connected.

- Calculate the loss
After receiving the walk data, the loss is calculated by comparing with the model.
