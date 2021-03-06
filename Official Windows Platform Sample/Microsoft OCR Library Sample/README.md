# Microsoft OCR Library Sample
## Requires
- Visual Studio 2013
## License
- MS-LPL
## Technologies
- OCR
## Topics
- Imaging
- OCR
## Updated
- 09/30/2014
## Description

<div id="mainSection">
<div class="clsServerSDKContent">
<div id="mainSection">
<div class="clsServerSDKContent">
<h1><a id="gallery_samples.ocr_cs"></a>Microsoft OCR Library Sample</h1>
</div>
<p>This sample demonstrates how to use the Microsoft OCR Library for Windows Runtime to extract text in the specified language from an image.</p>
<p><strong>Note</strong>&nbsp;&nbsp;</p>
<p class="note">This sample requires you to download and install the OCR Library into the sample project. The OCR Library is a NuGet package. For more info, see the instructions on this page.&nbsp;</p>
<p>This sample demonstrates following features:</p>
<ul>
<li>Extract text in the specified language from an image. </li><li>Overlay extracted text over the image. </li></ul>
<p>The OCR Library reads text from images and returns the text and layout information. All of this happens locally on the user's device. When you add the OCR Library to an application, you control how your application interprets the returned text. When the
 OCR Library recognizes patterns, such as email addresses, phone numbers, and URIs, your app can launch common actions such as sending an email, making a phone call, or visiting a web site.</p>
<p>To use the OCR Library in your app, call the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrengine.recognizeasync.aspx">
RecognizeAsync</a> method of the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrengine.aspx">
OcrEngine</a> class. This method returns an <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrresult.aspx">
OcrResult</a> object, which contains the recognized text and its size and position. The result is split into lines, and the lines are split into words.</p>
<ul>
<li>The <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrresult.aspx">
OcrResult</a> contains a collection of <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrline.aspx">
OcrLine</a> objects, which you access through the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrresult.lines.aspx">
Lines</a> property of the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrresult.aspx">
OcrResult</a>. </li><li>Each <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrline.aspx">
OcrLine</a> object contains a collection of <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrword.aspx">
OcrWord</a> objects, which you access through the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrline.words.aspx">
Words</a> property of each <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrline.aspx">
OcrLine</a>. </li><li>Each <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.ocrword.aspx">
OcrWord</a> object specifies the text, size, and position information of the word in the image.
</li></ul>
<p>For more info about the OCR Library, see <a href="http://msdn.microsoft.com/en-us/library/windows/apps/windowspreview.media.ocr.aspx">
WindowsPreview.Media.Ocr</a>.</p>
<p>To obtain an evaluation copy of Windows&nbsp;8.1, go to <a href="http://go.microsoft.com/fwlink/p/?linkid=301696">
Windows&nbsp;8.1</a>.</p>
<p>To obtain an evaluation copy of Microsoft Visual Studio&nbsp;2013, go to <a href="http://go.microsoft.com/fwlink/p/?linkid=301697">
Visual Studio&nbsp;2013</a>.</p>
<p><strong>Downloading and installing the OCR Library</strong></p>
<p>See the <a href="http://go.microsoft.com/fwlink/p/?LinkID=394348">NuGet documentation</a> for all the ways you can download and install the NuGet package in your project. To install the package from within Microsoft Visual Studio, do the following:</p>
<ol>
<li>In Visual Studio, select <strong>PROJECT | Manage NuGet Packages</strong>. </li><li>In the <strong>Online</strong> section, select nuget.org. Search for <strong>
Microsoft.Windows.Ocr</strong>. </li><li>Click <strong>Install</strong>. </li><li>Select <strong>BUILD | Configuration Manager</strong> to change the build configuration of your project from
<strong>AnyCPU</strong> to <strong>x86</strong>, <strong>x64</strong>, or <strong>
ARM</strong>. </li><li>If Intellisense does not work after you have installed the NuGet package, unload and reload the Visual Studio project. In Solution Explorer, right-click the project and select
<strong>Unload Project</strong>. Then right-click the project again and select <strong>
Reload Project</strong>. </li></ol>
<h2>Operating system requirements</h2>
<table>
<tbody>
<tr>
<th>Client</th>
<td><dt>Windows&nbsp;8.1 </dt></td>
</tr>
<tr>
<th>Server</th>
<td><dt>Windows Server&nbsp;2012&nbsp;R2 </dt></td>
</tr>
<tr>
<th>Phone</th>
<td><dt>Windows Phone 8.1 </dt></td>
</tr>
</tbody>
</table>
<h2>Build the sample<span style="font-size:10px">&nbsp;</span></h2>
<ol>
<li>Start Visual Studio Express&nbsp;2013 for Windows --&gt; and select <strong>File</strong> &gt;
<strong>Open</strong> &gt; <strong>Project/Solution</strong>. </li><li>Go to the directory in which you unzipped the sample. Go to the directory named for the sample, and double-click the Visual Studio Express&nbsp;2013 for Windows Solution (.sln) file.
</li><li>Press F7 or use <strong>Build</strong> &gt; <strong>Build Solution</strong> to build the sample.&nbsp;
</li></ol>
<h2>Run the sample</h2>
<p>To debug the app and then run it, press F5 or use <strong>Debug</strong> &gt; <strong>
Start Debugging</strong>. To run the app without debugging, press Ctrl&#43;F5 or use <strong>
Debug</strong> &gt; <strong>Start Without Debugging</strong>.</p>
</div>
</div>
</div>
