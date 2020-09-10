# Imagesampling

Image sampling and quantization


 # A. Nearest Neighbour 
 
 This is the simplest and requires the least processing time of  all  the  interpolation  algorithms.  
 Nearest  neighbor selects  the  value  of  the  nearest  pixel  by  rounding  the coordinates of the desired interpolation point.  
 Using this method one  finds  the  closest corresponding pixel  in  the source (original)  image for  each  pixel  in the  destination image. 
 New pixels are made the same as others close-by. The pixels or dots of color are duplicated to create new pixels as  the image grows. 
 It  creates pixilation or  edges that break up curves into steps or jagged edges. 
 This form of interpolation suffers from normally unacceptable effects for both enlarging and reduction of images].   
 
 # B. Bilinear Interpolation 
 
 Bilinear interpolation takes a weighted average of the four neighborhood  pixels  to  calculate  its  final  interpolated value. 
 The result is much smoother image than the original image. When all known pixel distances are equal, then the interpolated  value is  simply their  sum  divided by  four. 
 This technique performs  interpolation in  both directions, horizontal and vertical. 
 This technique gives better result than  nearest  neighbor  interpolation  and  take  less computation time compare to bicubic interpolation.   
 
 # C. Bicubic Interpolation 
 
 Bicubic goes one step beyond bilinear by considering the closest 4x4 neighborhood of known pixels for a total of 16 pixels.  
 Since  these  are  at  various  distances  from  the unknown pixel, closer pixels are given a higher weighting in  the  calculation.  
 Bicubic  produces  noticeably  sharper images than the previous two methods, and is perhaps the ideal combination of  processing time  and output quality. 
 For  this  reason  it  is  a  standard  in  many  image  editing programs including Adobe Photoshop, printer drivers and in-camera interpolation