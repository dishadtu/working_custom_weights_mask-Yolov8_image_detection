# working_custom_weights_mask-Yolov8_image_detection

In this, I have used the custom-trained model for masks. So the weight used is best.pt and not yolov8.pt .
This is an example of using a custom weights developed using a custom model in a  program.

The custom model was created in the earlier program located here - https://github.com/dishadtu/working_custom_data_yolov8

model = YOLO("best.pt") - This is how we are using the custom weights.

I have also tested with different images to test the various cases of no-mask and mask only.

When working with prebuilt custom data models, one needs to also change the labels as per the custom data model.
    labels = {0: u'improper_mask', 1: u'no_mask', 2: u'mask'}
   
   
So, not just the custom model usage but also custom labels usage as per the custom model.

Case 1 - Default yolov8.pt model and default labels -  you will only get to see the default values only like person, cups, chairs, etc.
Case 2 - Default yolov8.pt with the custom labels, you will not get proper responses.
Case 3 - Custom best.pt with custom labels, proper response
Case 4 - Custom best.pt with default labels, improper response


![No Mask](https://github.com/dishadtu/working_custom_weights_mask-Yolov8_image_detection/blob/main/no-mask.png)https://github.com/dishadtu/working_custom_weights_mask-Yolov8_image_detection/blob/main/no-mask.png)


![Mask](https://github.com/dishadtu/working_custom_weights_mask-Yolov8_image_detection/blob/main/face-mask-detection.png)
