# ip_project
 Removing Camera Shake from a Single Photograph

https://github.com/yangyangHu/deblur
patch selection = round(axis)

resize the image before we select the points

Priors for
	- noise
	- latent image
	- kernel

Debluring
	- difference btween ideal and blurry
	- finding the ideal (latent)
		- approximating distributions of pixels in the image
			we know that they may be heavy tailed from recent research
			we try to approx this distro by approxing its defining parameters
			which in our paper are K and gradient(Lp)
			we approximate these two parameter by coordinate descent