# gitcad_robot
My project with mine idle for visual robot
## robocad 1.6 beta
**robocad 1.6 beta** includes a new important functions for programming visual (or real) robot with 3 omni wheels.  
At first you need to open IDLE in the folder called **"gui"** and start **"gui.exe"**  
To open viewer you need to go to the folder called **"view"** and then start **"view.exe"**  
## watch the [video about robocad 1.6](https://www.youtube.com/watch?v=frR_C2sS0FI&t=8s "Youtube")  

![](https://github.com/CrackAndDie/robocad_1.4b/blob/master/cad_low.png)
## new additions
### new veeery small and pretty robocad
![](https://github.com/CrackAndDie/gitcad_python_private/blob/master/Yandex/robocad1.6.png)
#### robotino.get_image_path(im_name: str, start_x: int, start_y: int, infelicity=14, dispersion=3, is_start=True, power=3, reverse_x=False, reverse_y=True, number_in_arr=10, start_dis=3, slowly=True)  

Getting b/w image with black line by which it will drive

:param im_name: Image name (image needs to be in the same folder as program)  
:param start_x: X position of pixel on the image from which robot will drive  
:param start_y: Y position of pixel on the image from which robot will drive  
:param infelicity: Distance of return to last pixel that has more than one path  
:param dispersion: Dispersion of search nearest pixels  
:param start_dis: Start dispersion of search nearest pixels  
:param is_start: If True start_X and start_Y will be (0, 0)  
:param power: Coefficient to multiple to coords  
:param reverse_x: Reverses X coord  
:param reverse_y: Reverses Y coord  
:param number_in_arr: Last number to return in arr that has more than one path  
:param slowly: If True start_dis will go to dispersion by adding 2  
:return: Path includes array of tuples coords like [(0, 0), (9, 18), (4, 82)]  

#### robotino.drive_by_image(arr: array)

Func to drive by image

:param arr: Path array  
:return: None  

#### robotino.drive_by_axis(tup: tuple)

Func to drive by axis X, Y and rotate

:param tup: Tuple of X, Y and rot  
:return: None  
