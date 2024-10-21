java cLab 1 – INT 404: Image and Video Processing
Start Date: 2024-10-09 Deadline: 2023-10-23
15% of the final marks
Late Submission Policy: 5% of the total marks available for the assessment shall be deducted from the assessment mark for each working day after the submission date, up to a maximum of five working days.
Objectives:
1- Introducing the image processing capabilities of Matlab and its Image Processing Toolbox.
2- Learn to read and display different images.
3- Learn basic image processing steps.
4- Master different image enhancement techniques
Download:
Download the files of lab1-Material.zip from the Learning Mall, unzip the file into a folder lab1- Material, which contains “lenna512_low_dynamic_range.bmp”and “lenna512.bmp”.

Tasks:
1. Task1: PSNR (5’):
Write a function to measure the Peak Signal to Noise Ratio (PSNR) between two gray images in dB. For the peak value use 255. 255^2
T h e P S N R i s g i v 𝑃𝑃 𝑃𝑃𝑃𝑃 𝑃𝑃 𝑃𝑃 ( 𝑑𝑑 𝑑𝑑 ) = 1 0 𝑙𝑙 𝑙𝑙 𝑙𝑙 1 0 ( 𝑚𝑚 𝑚𝑚 𝑚𝑚 ) Where mse is the mean square error, and it is evaluated as:
 12 𝑚𝑚𝑚𝑚𝑚𝑚 = � ��𝑖𝑖𝑚𝑚(𝑟𝑟𝑖𝑖, 𝑐𝑐𝑖𝑖) − 𝑖𝑖𝑚𝑚2(𝑟𝑟𝑖𝑖, 𝑐𝑐𝑖𝑖)�
∀𝑟𝑟𝑐𝑐 ∀𝑐𝑐𝑐𝑐
2. Task 2 (37’)
In this task, we use the monochrome image Lenna (i.e., lenna512.bmp ) to do the following
sub tasks, and let’s call the original image Lenna as I0.
(a) I0 -> down-sampling to I1 with 1/2 size of I0 (both horizontally and vertically) using mean value. First, describe your algorithm and implement it by yourself. Then, display it and compare to the original image. Finally, explain your founding in the report; (10’)
(b) I1-> up-sampling to I1’ with the same size of I0 using nearest neighbor interpolation. First, describe your algorithm and implement it by yourself. Then, display it and compare to the original image. Finally, explain your founding in the report. (12’)
(c) First,calculatethePSNRbetweentheoriginalimageI0andtheup-sampledimages,i.e., nearest, bilinear, and bicubic, respectively. Then, describe the algorithm of bilinear. Finally, Compare the results of different interpolation methods and Explain your founding in the report. (15’) (Note: for the bilinear and bicubic interpolation, you can use the matlab function directly).
Image nearest bilinear bicubic PSNR (dB)
Task 3 (26’)
Import the image “lenna512_low_dynamic_range.bmp” as im_ldr, then finish the following sub-tasks:
(1) Write a function to generate a piece-wise linear mapping transform to enhance the contrast of im_ldr; Verify the effectiveness of several mapping transform functions by
            3.

evaluating the PSNR with respect to the reference image, and show all enhanced images;
Identify the best intensity mapping function you obtained. (10’)
(2) Briefly describe the technique of histogram equalization; Use this technique to enhance
4.
the contrast of the low quality 代 写Program、Matlab
代做程序编程语言image im_ldr; Display the obtained image and show its histogram in the report; Compare the current result with the best intensity mapping function in (1), and explain your finding. (16’)
Task 4 (32’)
In this task, we use the monochrome image Lenna (i.e., lenna512.bmp ) to do the following sub tasks, and let’s call this reference image Lenna as im.
a) Add Gaussian white noise with zero mean and variance 16 to the image im and display the noisy image. Name it as im_wn. Please write one function to generate this image instead of calling matlab function directly. (6’)
b) Describe the technique of average filter and weighted average filter with a 3X3 window, respectively. Then implement both of them by yourself and use the same template in the slides. Finally, compute the PSNR in the following table and display all filtered images and compare them to the original image. You can use add one boundary with the same as its neighboring pixel values (i.e., nearest neighbor padding). (10’)
Method Average filter Weighted average filter PSNR (dB)
c) Describe the technique of Image Averaging, and explain why it can remove noise. Use this technique to remove the noise of im_wn, e.g., average 10 images to get im_wn10, average 100 images to get im_wn100, and average 1000 images to get im_wn1000. You need to implement this by yourself.
Display these three images and Evaluate the PSNR of these three images with respect to the reference image im.
Comment which one is better by comparing to the mean. (16’)
im_wn10 im_wn100 im_wn1000
         Image PSNR (dB)
            
Lab Report
Write a short report which should contain a concise description of your results and observations. Include listings of the Matlab scripts that you have written. Describe each of the images that you were asked to display.
Answer each question completely:
– Do not attach the code at the end of the report, just put the useful code under each question
– The results maybe contain some figures, please add some index and title of each figure Report format: Single column; Fond size:  Page number: no more than 15;
Submission before 2024-10-23.
– Electrical version to LM with a rar (ZIP) of all files
• Rar file name: INT404-Lab1-Name-studentID.rar
• One file with same file name of Rar File: Report ( with studentID, name, Lab title on the
homepage)
• One folder: codes and other materials. (I can run it directly)
Marking scheme
80%-100% Essentially complete and correct work.
60%-79% Shows understanding, but contains a small number of errors or gaps.
40%-59% Clear evidence of a serious attempt at the work, showing some understanding, but with important gaps.
20%-39% Scrappy work, bare evidence of understanding or significant work omitted. <20% No understanding or little real attempt made.
This page last modified on 2024-10-08 8:53 AM

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
