Benford's Law
=============
I have been fascinated by Benford for a while, so i finally decided to create a small ruby script that will take a 
CSV file and compute the frequency distribution of the first digit.
The interesting part is that i haven't used any external library to draw the bar chart, i do everything in the terminal.
If you think that these charts woudl lack of accuracy you will be totally right. I am trying to compensate for this lack
of accuracy by computing the margin of error between the result obtained from the data set and Benford's predictions.

```
fenec@ubuntu:~/Desktop/project/benford_s_law$ ruby benford.rb 
{"1"=>56.86, "2"=>20.68, "3"=>8.15, "4"=>5.37, "5"=>2.98, "6"=>2.19, "7"=>0.99, "8"=>1.19, "9"=>1.59}
1: ---------------------------------------------------------|result:56.86%-error:88.9%
2: ---------------------|result:20.68%-error:17.43%
3: --------|result:8.15%-error:34.75%
4: -----|result:5.37%-error:44.58%
5: ---|result:2.98%-error:62.37%
6: --|result:2.19%-error:67.26%
7: -|result:0.99%-error:82.93%
8: -|result:1.19%-error:76.76%
9: --|result:1.59%-error:65.28%
 20.000000   0.000000  20.000000 ( 22.070408)
fenec@ubuntu:~/Desktop/project/benford_s_law$ 
```

