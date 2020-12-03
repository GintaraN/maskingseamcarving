# maskingseamcarving
Seam Carving Method for removing and rescaling with interactive mask

How to use : 
1. Required Numpy, Numba, Scipy
2. run at terminal : masksc.py -argument

For Resize: 
masksc.py -resize -im path/image.jpg -out path/imageresult.jpg -mask(optional) -dy 0 -dx 0 -vis 

For Remove object:
masksc.py -remove -im path/image.jpg -out path/imageresult.jpg -mask(optional) -rmask -vis 

-dy and -dx are positive or negative integer
-vis : to visualize seam carving method
-hremove : for remove object horizontally (default= vertical)
-backward_energy : use backward energy (default= forward)
putting -mask and -rmask together will show first window for protective mask and next second window for mask or object or area to remove 
Press s on your keyboard after done masking

Seam Carving algorithm is from https://github.com/andrewdcampbell/seam-carving
