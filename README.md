# o-detector: automatically detect microfluidic droplets using the hough transform, 
              GUI based on tkinter to interact with the annotated pictures and manually delete or annotate circles,
              outputs droplet size for statistical analysis of monodispersity

     
    
     Parameters
     ----------
     c_size : maximum circle size to detect\n
     can_thr : threshold HoughCircles uses for canny edge detection\n
     h_thr : threshold HoughCircles uses for circle detection\n
     
     
     Instructions
     ------------
     Choose files: select folder with your data\n
     Left click : Left click on picture , draw and release creates a new circle.\n
     Right click : Removes circle that was clicked\n
     Blur : Gaussian blurs the image which is used to detect circles\n
     Detect : Hough circle detection\n
     Next : appends circles to final list and skips to next image\n
     
     Notes
     -----
     Circle detection based on Yuen, H. K. et al. Image Vision Comput. 8 1, pp 71–77 (1990)
     and Canny, J. IEEE Trans. on Pattern Analysis and Machine Intelligence, 
     8(6), pp. 679-698 (1986).
