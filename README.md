# OTSU
from the paper we could find that , if u want to find the threshold u should find the maximum deltaB^2.
the main formulation is(we assume the photo that you used is a grayscale)
1.   pi=ni/N       N:means the total number of pixels. 
                   ni : means how many pixels of each gray-levl.
                   so we could think this formulation as the probability of each gray-level occur



2.   w0+w1=1       w0:u chould regard it as the probability of the object in the photo that u want.
     w(k)          accumulate from i to k of the pi.



3.   U0orU1=i*pi    weighting probability 
     UT=i*pi       accumulate from i to L.
     U(k)          accumulate from i to k.
     
     
     
4.  i means the gray-level [0,1,2...255] .


5.  k is the threshold u shold find.



now we can use deltaB^2 = [UTw(k)-U(k)]^2/w(k)[1-w(k)]

so the problem is simplified , we just need to maximize the deltaB^2
Besides that u should avoid w(k)=1 it will make the deltaB^2 = infinite



Please give me more advice.


![image](https://github.com/tinghsienchin/OTSU/blob/master/2773BFA3-424D-4557-86B8-D7473A3F8465.png)
