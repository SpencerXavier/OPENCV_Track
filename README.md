# WORK FLOW
End goal : do the training (retrain the custom data) and inference  on nano to detect the smoke and let ppl know where it's ther fire (simultaneously fire the alarm)and notify the firefighter


PATH1 : Digits[cloud platform] (make step by step tutorial)
- We use digits to do the training and test the inference on digits (30secs)
1. we put the Dataset from drone and we can distinguishh the sky and lrerrin
2.now we are trying feed the smoke data and label it to train and let it detect smoke in DIGITS(smoke and not smoke)60 pics

3.use the smoke data provided by researcher (solve label problem automatically,modify the layer text,come up with different scence for smoke) --label automatically and let ppl correct it manually create an UI(find a javascipt guy)


4.run the motion vector algorithm to see moving smoke and observe their behavior(addoition annotation see if it's from fire based on weather,wind) and different (joseph)
6.let ppl run on live camera (social network)


- run the model on jestoon nano(edge device) to do inference(2 mins)

------------------
PATH2 : KERAS (USE tensorflow 2.0)
- use keras to run it do the same thing


PATH3 :Use motion_estimation to detect the smoke[to track smoke behavior]
https://github.com/ross-abaco/rtp-motion-estimation
https://developer.ridgerun.com/wiki/index.php?title=Xavier/JetPack_4.1/Components/VisionWorks

PATH4 : UC Berkeley;s algorithm 
build a container and storage place and use UC Berkeley;s algorithm 



# use DIGITS to train and run on Jeston nano (you can test your own data )
https://github.com/dusty-nv/jetson-inference
ps. download and extract the trained model snapshot to Jetson (snapshot is in job)
NET = snapshot folder , png = your own data
segnet-console north_firecam_720.png output_firetower.png --prototxt=$NET/deploy.prototxt --model=$NET/snapshot_iter_4522.caffemodel --labels=$NET/fpv-labels.txt --colors=$NET/fpv-deploy-colors.txt --input_blob=data --output_blob=score_fr
use custom dataset to train models in digits (you can also test inference on digits)


# data provided by researcher
http://hpwren.ucsd.edu/HWB/HPWREN-FIgLib/20180717-otay-om-s-mobo-c/
https://github.com/byungheon-jeong/HPWREN-data

# Data-preprocess : Label tool
snorkel : https://github.com/HazyResearch/snorkel


# plan
poster
powerpoint
pragma conference

