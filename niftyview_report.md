# NiftyView: A Zero-Footprint Web Application for viewing DICOM and NIfTI files

## Introduction
NiftyView is a free web application developed for viewing medical images. The current version supports both NIfTI[^1] and DICOM[^2] format. It has zero footprint; Only a web browser and an Internet connection are needed to run the NiftyView. It’s advantageous over conventional desktop applications in that NiftyView doesn’t require installation and constant updates. It can run on any Operating System as long as an Internet connection is available. As a minimal image viewer, it’s a convenient tool for users who need a quick and easy tool for viewing medical images. The beta version of NiftyView currently is freely available at http://www2.hawaii.edu/~weiran/NiftyView.html.  

## Approach
NiftyView is a front-end web application developed in JavaScript with jQuery[^3] for HTML document manipulation and event handling, jQueryUI[^4] for user interface, and DicomParser[^5] for parsing DICOM files. It’s compatible with popular web browsers including Microsoft Internet Explorer, Apple Safari, Mozilla Firefox, and Opera. To launch NiftyView, a user simple point the browser to the link http://www2.hawaii.edu/~weiran/NiftyView.html. Either DICOM or NIfTI images can be loaded by dragging files into the browser window. Loaded images can be displayed in either single-slice mode or tiled multi-slice mode. After loading, images are automatically arranged according to the scan ID for DICOM files and the file name for NIfTI files. Current functions include image zooming and adjustment of image brightness and contrast. These functions can be used either in the single or titled mode. The number of image columns can be adjusted in the tiled to maximize the use of the displace space. The contrast and brightness of images can be adjusted by clicking and holding the right mouse button or using a unique double slider widget in the tool bar. 

## Results and Discussion
![Image of NiftyView]
(https://github.com/weirandeng/niftyview_brainhack_report/blob/master/niftyview_ui.png)
Figure-1 shows that nearly 1,500 DICOM files from 11 MRI scans are loaded and displayed in NiftyView in multi-slice tiled mode. 
NiftyView however is a lightweight and high-performance view taking less than ten seconds to load all the DICOM files into NiftyView.The inherent limitation of a web-based application developed in JavaScript is slow performance compared to its counterpart developed in C/C++ and compiled into an executable. However, moving from the desktop to the cloud is an inevitable trend and the performance gap between the native and web app is narrowing with the collective effort from industry leaders such as Google, Microsoft, and Apple who are investing in new technologies such as WebAssembly to improve the performance of web applications. Future work will include support of access files stored in HIPAA (Health Insurance Portability and Accountability Act) cloud storages such as Box and Amazon S3 and a responsive design compatible with mobile platforms such as iOS and Android. The final version of NiftyView will be released under a General Public License that allows end users to freely run, modify, and share the program.

## Conclusion
NiftyView is a free and convenient web application for quick and easy viewing of NIfTI and DICOM medical images. It is especially helpful for situations where a study subject is given data with an accompanying program which usually runs only in Microsoft Windows.

## References
[^1]: NIfTI Data Format Working Group, NIfTI: Neuroimaging Informatics Technology Initiative, http://nifti.nimh.nih.gov. 
[^2]: The association of Electrical Equipment and Medical Imaging Manufacturers, DICOM: Digital Imaging and Communications in Medicine, http://dicom.nema.org. 
[^3]: jQuery JavaScript Library, http://jquery.com. 
[^4]: jQuery User Interface, http://jqueryui.com.
[^5]: Chris Hafey, https://github.com/chafey/dicomParser. 


