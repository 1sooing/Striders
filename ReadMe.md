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

---
References

[Tutorial]
docker for windows download (+ other OS)
- http://pyrasis.com/Docker/Docker-HOWTO


running jupyter server
- https://plot.ly/python/ipython-notebook-tutorial/


RNN tutorial
- http://aikorea.org/blog/rnn-tutorial-1/


install NLTK
- http://www.nltk.org/install.html


install theano
- http://deeplearning.net/software/theano/install.html


[ Lecture ]
"모두를 위한 머신러닝/딥러닝 강의" | hunkim (kim sung hun)
- http://hunkim.github.io/ml/



Stanford Computer Engineering Artificial Intelligence Instruction 'CS231n'
- http://cs231n.stanford.edu/syllabus.html



RNN introduction |  Original : colah's blog
- https://brunch.co.kr/@chris-song/9
- http://colah.github.io/posts/2015-08-Understanding-LSTMs/


[ Supplement ]
A site that beautifully visualizes the process of machine learning.
- http://www.r2d3.us/visual-intro-to-machine-learning-part-1/



The utility of LSTM
- http://karpathy.github.io/2015/05/21/rnn-effectiveness/



Speeding up with Theano & GPU
- http://www.wildml.com/2015/09/speeding-up-your-neural-network-with-theano-and-the-gpu/


