# NiftyView: A Zero-Footprint Web Application for viewing DICOM and NIfTI files
Author: Weiran Deng and V. Andrew Stenger
Institute: University of Hawaii JABSOM, Honolulu, HI 96813

## Introduction
NiftyView is a free web application developed for viewing medical images. The current version supports both NIfTI[^1] and DICOM[^2] format. It has zero footprint; Only a web browser and an Internet connection are needed to run NiftyView. It’s advantageous over conventional desktop applications in that NiftyView doesn’t require installation and constant updates. It can run on any Operating System as long as an Internet connection is available. As a minimal image viewer, it’s a convenient tool for users who need a quick and easy tool for viewing medical images. Currently, the beta version of NiftyView is freely available at http://www2.hawaii.edu/~weiran/NiftyView.html.  

## Approach
NiftyView is a front-end web application developed in JavaScript with jQuery[^3] for HTML document manipulation and event handling, jQueryUI[^4] for user interface, and DicomParser[^5] for parsing DICOM files. It’s compatible with popular web browsers including Microsoft Internet Explorer, Apple Safari, Mozilla Firefox, and Opera. To launch NiftyView, a user simple points the browser to the link http://www2.hawaii.edu/~weiran/NiftyView.html. Either DICOM or NIfTI images can be loaded by dragging files into the browser window. Loaded images can be displayed in either single-slice mode or tiled multi-slice mode. After loading, images are automatically arranged according to the scan ID for DICOM files and the file name for NIfTI files. Current functions include image zooming and adjustment of image brightness and contrast. These functions can be used either in the single or titled mode. The number of image columns can be adjusted in the tiled mode to maximize the use of the display space. The contrast and brightness of images can be adjusted by clicking and holding the right mouse button or using a double slider widget in the horizontal tool bar at the top of the window. 

## Results 
![Image of NiftyView]
(https://github.com/weirandeng/niftyview_brainhack_report/blob/master/niftyview_ui.png)
Figure-1 shows a few sagittal MRI images displayed in titled mode after loaidng approximately 1,500 DICOM files from 11 MRI scans. It took approximately ten seconds to load all the DICOM files into NiftyView. The images are organized into different vertical tabs by the sequence names stored in the DICOM files. 

## Discussion
The inherent limitation of a fontend web application developed in JavaScript is the slow performance compared to its counterparts, which are usually developed in a static typed language such as C/C++ and compiled and linked into an executable. However, shifting from the desktop to the cloud is an inevitable movement and the performance gap between the native and web application is narrowing with the collective efforts from industry leaders such as Google, Microsoft, and Apple, who are investing in new technologies such as WebAssembly to improve the performance of web applications. NiftyView has a minimal biolerplate and can handle a large number of files with relative ease. We are considering to further improve the performance of the application with HTML5 features such as Web Workers. Future work will also include support of accessing files stored in HIPAA (Health Insurance Portability and Accountability Act) compliant cloud storage servies such as Box and Amazon S3 and adapting a responsive design compatible with mobile platforms such as iOS and Android. The stable version of NiftyView will be released under a General Public License that allows end users to freely run, modify, and share the program. We are also open to accept comments and suggestions for future developments. 

## Conclusion
NiftyView is a free and convenient web application for quick and easy viewing of NIfTI and DICOM medical images. Although there are native desktop applications available, NiftyView should be a  useful aternative to users who need a quick access to an application without the hassle of downloading and installing any program.  

## References
[^1]: NIfTI Data Format Working Group, NIfTI: Neuroimaging Informatics Technology Initiative, http://nifti.nimh.nih.gov. 
[^2]: The association of Electrical Equipment and Medical Imaging Manufacturers, DICOM: Digital Imaging and Communications in Medicine, http://dicom.nema.org. 
[^3]: jQuery JavaScript Library, http://jquery.com. 
[^4]: jQuery User Interface, http://jqueryui.com.
[^5]: Chris Hafey, https://github.com/chafey/dicomParser. 


