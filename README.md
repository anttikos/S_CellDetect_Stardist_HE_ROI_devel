# S_CellDetect_Stardist_ROI
Cytomine app for Cell (Nuclei) Detection in ROIs, using Stardist Python code (https://github.com/mpicbg-csbd/stardist/)
by Uwe Schmidt, Martin Weigert, Coleman Broaddus, and Gene Myers (MICCAI 2018).

This implementation applies a Stardist pre-trained model (versatile_HE) to regions of interest within large whole-slide images. A ROI annotation term identifier is given and the app applies the algorithm to all Cytomine annotations labeled by the user, with this term, in the whole image. Detected objects are labeled with object term identifier.

While the original model was trained with H&E images, it seems to produce decent results with other staining. Future work will investigate fine-tuning models with specific data.

This version use tensorflow CPU version to ensure compatibility with many computers.