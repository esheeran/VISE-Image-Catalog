# VISE-Image-Catalog
This project is a small-scale example of the Oxford VGG VISE software. It creates an image catalog that supports text, reverse image, and similarity search.

#Instructions for opening
1. Open the Windows command line or powershell.
2. Run the following code sequentially:
  cd ~/wise-2.1.0 
  source wise-dep/bin/activate
  python3.11 serve.py --project-dir wise-projects/MyPhotos/

#Instructions to add new images
1. Add new images to local images folder. Remove and replace old folder. Then run:
  python3.11 extract-features.py ~/images/ --project-dir wise-projects/MyPhotos/
  python3.11 create-index.py --project-dir wise-projects/MyPhotos/
