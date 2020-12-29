# ip_project
 Removing Camera Shake from a Single Photograph

https://github.com/yangyangHu/deblur
patch selection = round(axis)

resize the image before we select the points



UDP (User Defined Parameters) x3 BIRD IMAGE (in the project) #TO_DO
	Kernel size ################## A
	Scaling (for compoutational time) A
	Patch Selection ################# C
	Orientation of the Kernel (for compoutational time) C
	# of iterations of the reconstruction ############### M
	threshold on kernel intensities (mask for saturated image regions) M
	
Debluring
	Priors for
	- noise
	- latent image
	- kernel

	- difference btween ideal and blurry
	- finding the ideal (latent)
		- approximating distributions of pixels in the image
			we know that they may be heavy tailed from recent research
			we try to approx this distro by approxing its defining parameters
			which in our paper are K and gradient(Lp)
			we approximate these two parameter by coordinate descent
			we use 4 gausians and 4 gamma distros

Multi-scale Approach #TO_DO

Image Reconstruction #TO_DO

