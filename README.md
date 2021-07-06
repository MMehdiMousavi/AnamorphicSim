# AnamorphicSim

This tool allows you to distort footage, and apply anamorphic Lens Flares automatically in post.
For best results, use a short clip from your footage, and try to optimize the variables for your specific shooting environment.
If you have any questions, open a Ticket in Issues.

You need to install the latest version of the following packages to run this code:
- numpy
- python-opencv
- PILLOW
- matplotlib
- scipy 

The entry of the program is titled as <b>Main Execution</b>. 
There are few parameters that can be modified in order to adjust the nature of flare we generate:
1. input_video = Full path to input video
2. output_video = full path of the output video file
3. write_fps = fps for writing output.
4. binarize_thr = binarize threshold. The more this value, the less flares you will get.
5. conn_comp_diam_limit = Cnnected component diameter. Each detected light source might not qualify as a flare source. So we  limit it by a diameter range. Saying that flares can only be within a diameter range(10-500pixels in our experiments)
6. light_src_limit = maximum number of flares we want in the video at once.
7. bright_increment = How much bright we want the flares to be. Increasing this value makes the flares brighter.

## Download the dataset videos and generated outputs from google drive: https://drive.google.com/file/d/1cse7xKlZ03iok0HDsRqw__nNvzPtFnbr/view?usp=sharing
## and put the 'vid' folder where you have your script

Once you adjust the above parameters, you can run the whole script. The output will be saved in the file specified.

## Example Video: 
[![Anamorphic Format Simulator](https://img.youtube.com/vi/OsQQ8_si5kc/0.jpg)](https://www.youtube.com/watch?v=OsQQ8_si5kc)

