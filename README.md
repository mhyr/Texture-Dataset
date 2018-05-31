# Texture-Dataset
This dataset is a collection of different textures which can be used as a (train/test) set for Texture Defect Detection algorithems.

During the following three months, I am going to gradually add new textures in separate folders, where each includes 150 samples of defected texture, 1000 samples of clean texture. Each folder also includes masked copy of defected samples and a "csv" file consisting lables of -what I call bounding ellipses- of defected areas.

**Camera**
I'm simply using my cell phones primary camera which is a Samsung Galaxy S4 I9500 model. The basic specification of the camera is: 13 MP (f/2.2, 31mm, 1/3", 1.14µm), autofocus.
The first problem with this cheap and convinient camera is its output, which is of a lossy format with no access to the RAW image data. In addition, low shutter speed and lack of marco lense does not result in the best quality photos.
The lower quality of the photos however, can be beneficial in the sense that whatever algorithem that is trained with these photos, would be potentially more robust.

The preparation steps after taking the photos are as folows:

**Photoshop**

	1-1- open image

	1-2- F4 to slice horizental phtos/ F6 to slice vertical photos

	1-3- ctrl+"." to crop more

	1-4- F5 to save each slice as a separate file

	1-5- F7 select previous document
  
**Imagej**

	2-a- Ellips

		2-a-1 open

		2-a-2 select

		2-a-3 press "6" to make labels and save in a "csv" file

		2-a-4 repeat 2-a-2, 2-a-3 (if needed)

		2-a-5 7 go to the next image

	2-b- Mask

		2-b-1 open

		2-b-2 select

		2-b-3 t save to ROI (if more than one area, if only one are, jump this step)

		2-b-4 8 save mask to new binary file

		2-b-5 7 go to the next image
