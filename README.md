# Grab_ComputerVision


1. Overview 
- Classification with localization problem with coordinates of bounding boxes provided
	- To compare if the use of bounding boxes provide more accurate predictions 
- Huge dataset with large labels will require large processing power 
	- To see if we can work with smaller sample size and leverage on data argumentation techniques 
	- Grouping of cars to see which forms the larger proprtion within the pack and train on those images 
	- Leverage on proven architecture and compare on their performances (AlexNet, VGG, ResNet, Inception, DenseNet etc)

2. Data files and Directories
- Files are downloaded onto a local directory
- Link: https://ai.stanford.edu/~jkrause/cars/car_dataset.html
		- cars training images dataset 
		- cars testing images dataset 
		- cars devkit  


3. Preprocessing 
	- Data checks: for null and duplicates 
		- 22 images removed from training
		- 18 images removed from test 
	- Data Extraction and Merging of Dataset
		- Images are cropped to bounding boxes and resized
		- labels are prepared with one hot encoding used
		- Images and labels are prepared as X and y	
		- training data and validation data is split 90:10	

4. Model 
	- Development of CNN model - compile and fit with data argumentation to create more images 

	(Future Runs)
	-First Run 20190616 - Sample size too small, too many labels = poorly classification ~1-2%
	- resize smaller, more epochs runs (up to 200)
	- insufficient run time and processing power 


5. Assessment (Did not complete) 
	- Model to be tested on new random generated car sampels 
	- Model Optimization 
	- Additional analysis: Leverage on proven architecture and compare on their performances (AlexNet, VGG, ResNet, Inception, DenseNet etc)

