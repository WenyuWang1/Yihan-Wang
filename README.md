# Part 3:
In part 3, we use APDS9960 to detect color and display the detection results on RP2040. 
We enable the color detection function on APDS9960 and store the data in r, g, b and c, which represent red, green, blue and clear data detected by APDS9960’s sensor respectively.
To display APDS9960’s sensor readings in real time, we have to change the number of samples for each sensor reading. In APDS9960’s data sheet, it shows that the value of color_integration_time determines time between readings. The default value is 256 and we could set this value small to speed up the sensor readings.


![screenshot1](https://user-images.githubusercontent.com/113371324/191817230-a68f800b-3ca7-4bbf-b15f-7f5a999350a6.png)

![screenshot2](https://user-images.githubusercontent.com/113371324/191817294-d1a07b96-58b6-4834-9639-6d7152f0cb81.png)
![screenshot3](https://user-images.githubusercontent.com/113371324/191817331-54c98fd4-b16e-46f1-842a-02392a846df0.png)

The display result is shown below:

![4_4record_AdobeExpress](https://user-images.githubusercontent.com/113371324/191828183-40272fe2-ccc7-48b0-aeb1-79829e2eb0b7.gif)

Clearer gifs are in the gif folder


# Part 4:
In part 4, we visualize APDS9960’s brightness reading by sending keyboard output and displaying them on the laptop. The sensor reads brightness twice in a very short time and the data are saved in different variables. By comparing these variables, the controller knows whether the environment is getting brighter or darker. And when the brightness increases, the keyboard will output "Crazy Thursday !!!". When the brightness increases, the keyboard will output "V me 50". 

The display result is shown below:



![WeChat_20220922150128_AdobeExpress](https://user-images.githubusercontent.com/113371324/191829813-82572219-fa3c-4e8a-badd-ee54058026aa.gif)

Clearer gifs are in the gif folder

The diagram that showws how the components interact is showing below:
![4](https://user-images.githubusercontent.com/113371324/191817534-be1cdefa-87f8-48ba-b8a0-3de8ff8355df.png)
