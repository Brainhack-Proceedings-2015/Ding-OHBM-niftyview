# NiftyView: A Zero-Footprint Web Application for viewing DICOM and NIfTI files

## Introduction
NiftyView is a free web application for viewing NIfTI and DICOM images. Its purpose is to facilitate access to medical images in big data and open research. This abstract presents NiftyView, a zero-footprint web application for viewing NIfTI1 and DICOM2 images. It is a convenient web application for viewing medical images without the hassle of downloading, installing, or updating any software. NiftyView is developed in JavaScript and runs natively on web browsers therefore requiring no installation. It runs on any Operating System with a web browser as long as there is an Internet connection. NiftyView also has a minimal boilerplate hence a performance that allows loading and viewing large number of image files. 

## Approach
NiftyView is developed in JavaScript using several external libraries such as jQuery3 and DicomParser4. It is platform independent and runs on any Operating System including Linux, Mac OS X, and Microsoft Windows within a mainstream web browser such as Firefox, Chrome, Safari, or Opera. NiftyView has a zero footprint with no downloading or installation is required. It can be accessed at http://www2.hawaii.edu/~weiran/NiftyView.html and runs natively as a web application in the browser. To use NiftyView, a user can simply drag the DICOM or NIfTI files into the browser window. Images will be automatically organized into different tabs by scans. Images can be displayed in single-slice or tiled multi-slice mode. Images can be zoomed and the number of columns can be adjusted. The contrast and brightness can be adjusted by clicking and holding the right mouse button or using a double slider widget. Figure-1 shows that nearly 1,500 DICOM files from 11 MRI scans are loaded and displayed in NiftyView in multi-slice tiled mode. NiftyView however is a lightweight and high-performance view taking less than ten seconds to load all the DICOM files into NiftyView.

## Results
NiftyView is a free and convenient web application for quick and easy viewing of NIfTI and DICOM medical images. It is especially helpful for situations where a study subject is given data with an accompanying program which usually runs only in Microsoft Windows. The inherent limitation of a web-based application developed in JavaScript is slow performance compared to its counterpart developed in C/C++ and compiled into an executable. However, moving from the desktop to the cloud is an inevitable trend and the performance gap between the native and web app is narrowing with the collective effort from industry leaders such as Google, Microsoft, and Apple who are investing in new technologies such as WebAssembly to improve the performance of web applications. Future work will include support of access files stored in HIPAA (Health Insurance Portability and Accountability Act) cloud storages such as Box and Amazon S3 and a responsive design compatible with mobile platforms such as iOS and Android. The final version of NiftyView will be released under a General Public License that allows end users to freely run, modify, and share the program.
## Discussion

## Conclusion

## References
(1) NIfTI Data Format Working Group, NIfTI: Neuroimaging Informatics Technology Initiative, http://nifti.nimh.nih.gov. (2) The association of Electrical Equipment and Medical Imaging Manufacturers, DICOM: Digital Imaging and Communications in Medicine, http://dicom.nema.org. (3) jQuery, http://jquery.com. (4) Chris Hafey, https://github.com/chafey/dicomParser. 


