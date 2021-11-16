# What About the Data?
- ACRE (Agri-food Competition for Robot Evaluation)
- To get the data used you will need to sign up for the competition at CodaLab
- Autonomous robots capturing images using an RGB camera
- Small Dataset - 90 images for training and 15 for testing
- 2048x1536 pixels - 3 MP
- Manually labeled ground-truth segmentations. (Image Masks)
- Image Masks are colored, but need to be converted into labels

# Model
- Built using the VGG16 CNN architecture
- Uses skip connections

# Hyperparams
All the hyperparams were picked based on some previouse analysis done using gridsearch with k-fold validation, early stops, and tensorboard visualization.

# Evaluation
- Using IoU which is equal to `area of overlap/ area of Union`