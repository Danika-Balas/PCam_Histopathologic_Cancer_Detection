# PCam_Histopathologic_Cancer_Detection
I developed convolutional neural networks (CNN) in order to classify images of stained lymph nodes as cancerous or non-cancerous within the PatchCamelyon dataset, also known as PCam (Veeling, 2018). I explored numerous model architectures in order to identify a model topology that provided high accuracy while being mindful of model complexity and constrained by resource scarcity. I explored CNN topologies trained fully on the PCam data as well as two pre-trained networks, VGG16 and ResNet50.

I found the best model to be VGG16 with the final six convolutional layers trained on the PCam dataset, followed by a fully connected layer with 256 nodes and 30% dropout in its final layer (see Figure 1). This model had an accuracy of 84.5% and an AUROC of 0.914 on the testing dataset.

I also found a two-layer CNN that was fully trained on the PCam data to be less computationally expensive while having competitive results (see Figure 2). This model took **one quarter of the time to train** as the VGG16 model and had an accuracy of 82.5% and an AUROC of 0.897 on the testing dataset.
