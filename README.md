# NopCommerce-PersianCalendar
##Persian calendar for [NopCommerce](http://www.nopcommerce.com/) store

use this repository only for NopCommerce **Version 3.80**

###Usage :
- If you haven't change admin panel and you don't have any customization just copy and page repository files into your site root folder
- If you have done some customization do as below :
 - copy Persia.dll into Bin folder.
 - copy fa-IR.min.js and JalaliDate.min.js files to administration\scripts\ folder.
 - copy kendo.web.min.js file to administration\scripts\kendo\2014.1.318\ folder.
 - copy and replace DateTimeNullabled.cshtml file that is located in administration\views\shared\editorTemplate\
 - open _AdminLayout.cshtml that is located in administration\views\shared\ and remove Html.AppendScriptParts(string.Format("~/Administration/Scripts/kendo/{0}/kendo.web.min.js", kendoVersion)); from top of file and then add Html.AppendScriptParts("~/Administration/Scripts/fa-IR.min.js"); Html.AppendScriptParts(string.Format("~/Administration/Scripts/kendo/{0}/kendo.web.min.js", kendoVersion)); Html.AppendScriptParts("~/Administration/Scripts/JalaliDate.min.js");
