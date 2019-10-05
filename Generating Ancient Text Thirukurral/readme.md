<h3> Generating Ancient Text Thirukkural </h3>

<p> This is fun little project where I tried to generate new thirukkural text. Thirukkural is an ancient text written by sage thiruvalluvar The Tirukkural, or shortly the Kural, is a classic Tamil text consisting of 1,330 couplets or Kurals, dealing with the everyday virtues of an individual. It is one of the two oldest works now extant in Tamil literature in their entirety, the other being the Tolkappiyam.
  
![image](https://user-images.githubusercontent.com/35063929/66252690-0c4f5f00-e77c-11e9-9061-dcbe2b7700ae.png)

The above shown is the text of thirukkural. We will implement a word level RNN/LSTM to generate new couplets given a seed word.

<h3> Why I did not use char level RNN? </h3>

Though building one is totally possible and works well. Tamil is a complex language. The short vowel and long vowel are created on a particular way. If I split the first sentence into letters as shown below
![image](https://user-images.githubusercontent.com/35063929/66252808-a1068c80-e77d-11e9-9895-15c4828ae8f5.png)

You may notice the word 
![image](https://user-images.githubusercontent.com/35063929/66252828-cc897700-e77d-11e9-8361-f1f63db9c646.png) is split into ![image](https://user-images.githubusercontent.com/35063929/66252832-e32fce00-e77d-11e9-83f2-5105ebf0a831.png).


This behaviour is not desirable and each of letters are not in their original complete form. Hence we started of with word level RNN.


<h3> Generated kural?? </h3>

Below are the some examples of them, We will see a comparision of how the text looked at first epoch and how it looked at the last epoch.

Epoch 1: 

![image](https://user-images.githubusercontent.com/35063929/66252882-4cafdc80-e77e-11e9-89e7-0899238034c7.png)

![image](https://user-images.githubusercontent.com/35063929/66252915-9e586700-e77e-11e9-8f2f-e320ea9015d8.png)


Epoch 10: 

![image](https://user-images.githubusercontent.com/35063929/66252935-d5c71380-e77e-11e9-998a-929f2f8b31d0.png)

Most important thing to notice here is the word 3 ends with a characters which tells its relation with that starting character of the successor word. 
