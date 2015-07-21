# stache-castle
Grunt task for converting Sandcastle Documentation to Stache (JSON + markdown)

## Instructions <a name="Instructions"></a>

- the task is a default so all you have to do is run grunt.
- Go into the grunt task (Gruntfile.js) and edit some config options for convert
  - Set the src and dest properties to be the source XML file and the destination JSON
  - NOTE: these files should exist before running, the task will not create the files for you
- Go into the grunt task (Gruntfile.js) and edit some config options for cash_stache
  - Set the directory where your XML files and html folder will be.
  - Set the name of the folder your html files will be in, default is 'html'
  - Set the destination JSON file.
  - Set whether or not the Url's are included in the XML
  - Set the name of the attribute that contains the Url
  - NOTE: these files should exist before running, the task will not create the files for you.

## Class JSON Format <a name="Class"></a>
######(Files beginning in T_, generally pages with all information regarding a class)
```
				{
					"name": "T:Blueshirt.Core.Crm.Panel",
					"summary": "\r\n            Base class to handle interactions for panels.\r\n            ",
					"params": {
						"inheritance": {
							"http://msdn2.microsoft.com/en-us/library/e5kfa45b": "SystemAddLanguageSpecificTextSet(\"LST7F1E7F6D_25?cs=.|vb=.|cpp=::|nu=.|fs=.\");Object",
							"T_Blueshirt_Core_Base_BaseComponent.htm": "Blueshirt.Core.BaseAddLanguageSpecificTextSet(\"LST7F1E7F6D_26?cs=.|vb=.|cpp=::|nu=.|fs=.\");BaseComponent",
							"#": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_27?cs=.|vb=.|cpp=::|nu=.|fs=.\");Panel",
							"T_Blueshirt_Core_Crm_AdHocQueryPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_28?cs=.|vb=.|cpp=::|nu=.|fs=.\");AdHocQueryPanel",
							"T_Blueshirt_Core_Crm_BatchEntryPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_29?cs=.|vb=.|cpp=::|nu=.|fs=.\");BatchEntryPanel",
							"T_Blueshirt_Core_Crm_BusinessProcess.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_30?cs=.|vb=.|cpp=::|nu=.|fs=.\");BusinessProcess",
							"T_Blueshirt_Core_Crm_ConstituentPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_31?cs=.|vb=.|cpp=::|nu=.|fs=.\");ConstituentPanel",
							"T_Blueshirt_Core_Crm_EventManagementTemplatesPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_32?cs=.|vb=.|cpp=::|nu=.|fs=.\");EventManagementTemplatesPanel",
							"T_Blueshirt_Core_Crm_EventPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_33?cs=.|vb=.|cpp=::|nu=.|fs=.\");EventPanel",
							"T_Blueshirt_Core_Crm_InformationLibraryPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_34?cs=.|vb=.|cpp=::|nu=.|fs=.\");InformationLibraryPanel",
							"T_Blueshirt_Core_Crm_LocationsPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_35?cs=.|vb=.|cpp=::|nu=.|fs=.\");LocationsPanel",
							"T_Blueshirt_Core_Crm_MajorGivingSetupPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_36?cs=.|vb=.|cpp=::|nu=.|fs=.\");MajorGivingSetupPanel",
							"T_Blueshirt_Core_Crm_MarketingAcknowledgementsPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_37?cs=.|vb=.|cpp=::|nu=.|fs=.\");MarketingAcknowledgementsPanel",
							"T_Blueshirt_Core_Crm_MarketingAcknowledgementTemplatePanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_38?cs=.|vb=.|cpp=::|nu=.|fs=.\");MarketingAcknowledgementTemplatePanel",
							"T_Blueshirt_Core_Crm_MultiEventPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_39?cs=.|vb=.|cpp=::|nu=.|fs=.\");MultiEventPanel",
							"T_Blueshirt_Core_Crm_PackagesPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_40?cs=.|vb=.|cpp=::|nu=.|fs=.\");PackagesPanel",
							"T_Blueshirt_Core_Crm_Panels_QueryPanel.htm": "Blueshirt.Core.Crm.PanelsAddLanguageSpecificTextSet(\"LST7F1E7F6D_41?cs=.|vb=.|cpp=::|nu=.|fs=.\");QueryPanel",
							"T_Blueshirt_Core_Crm_PlanPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_42?cs=.|vb=.|cpp=::|nu=.|fs=.\");PlanPanel",
							"T_Blueshirt_Core_Crm_PledgePanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_43?cs=.|vb=.|cpp=::|nu=.|fs=.\");PledgePanel",
							"T_Blueshirt_Core_Crm_PledgeSubtypePanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_44?cs=.|vb=.|cpp=::|nu=.|fs=.\");PledgeSubtypePanel",
							"T_Blueshirt_Core_Crm_ReceiptsPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_45?cs=.|vb=.|cpp=::|nu=.|fs=.\");ReceiptsPanel",
							"T_Blueshirt_Core_Crm_RecurringGiftPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_46?cs=.|vb=.|cpp=::|nu=.|fs=.\");RecurringGiftPanel",
							"T_Blueshirt_Core_Crm_RegistrantPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_47?cs=.|vb=.|cpp=::|nu=.|fs=.\");RegistrantPanel",
							"T_Blueshirt_Core_Crm_RevenueRecordPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_48?cs=.|vb=.|cpp=::|nu=.|fs=.\");RevenueRecordPanel",
							"T_Blueshirt_Core_Crm_SegmentPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_49?cs=.|vb=.|cpp=::|nu=.|fs=.\");SegmentPanel",
							"T_Blueshirt_Core_Crm_SegmentsPanel.htm": "Blueshirt.Core.CrmAddLanguageSpecificTextSet(\"LST7F1E7F6D_50?cs=.|vb=.|cpp=::|nu=.|fs=.\");SegmentsPanel"
						},
						"lower_syntax_text": "The Panel type exposes the following members.",
						"namespace": {
							"N_Blueshirt_Core_Crm.htm": "Blueshirt.Core.Crm"
						},
						"assembly": " Blueshirt.Core (in Blueshirt.Core.dll) Version: 1.0.647.3 (1.0.647.3)",
						"syntax": {
							"C#": "public class Panel : BaseComponent",
							"VB": "Public Class Panel\n\tInherits BaseComponent",
							"C++": "public ref class Panel : public BaseComponent"
						},
						"constructors": {
							"Panel": {
								"link": "M_Blueshirt_Core_Crm_Panel__ctor.htm",
								"description": "Initializes a new instance of the Panel class",
								"public": "",
								"declared": "",
								"notNetfw": ""
							}
						},
						"methods": {
							"AdditionalDatalistPagesExist": {
								"link": "M_Blueshirt_Core_Crm_Panel_AdditionalDatalistPagesExist.htm",
								"description": "\n            Check if additional pages exist for a datalist to load.  If so load the page.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"GetHashCode": {
								"link": "http://msdn2.microsoft.com/en-us/library/zdee4b3y",
								"description": "Serves as a hash function for a particular type.  (Inherited from Object.)",
								"public": "",
								"inherited": "",
								"notNetfw": ""
							},
							"GetType": {
								"link": "http://msdn2.microsoft.com/en-us/library/dfwy45w9",
								"description": "Gets the Type of the current instance. (Inherited from Object.)",
								"public": "",
								"inherited": "",
								"notNetfw": ""
							},
							"getXDataListColumnValue": {
								"link": "M_Blueshirt_Core_Crm_Panel_getXDataListColumnValue.htm",
								"description": "\n            Given the DOM index of a datalist column and the value for that column, return an XPath\n            to append to a datalist XPath for finding that value in the requested column index.\n            \n            No element will be found if the value does not exist in this column.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"getXDiv": {
								"link": "M_Blueshirt_Core_Crm_Panel_getXDiv.htm",
								"description": "\n            Given the unique HTML element ids of a dialog and div, return a unique identifier XPath\n            to find the DIV field.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"getXDuplicateSectionDatalistColumnHeaders": {
								"link": "M_Blueshirt_Core_Crm_Panel_getXDuplicateSectionDatalistColumnHeaders.htm",
								"description": "\n            XPath to get the TR row of column headers for a section's datalist when multiple sections with matching\n            captions exists for a single panel on different tabs.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"getXPanelHeaderLink<span id=\"LST7F1E7F6D_4\"></span><script type=\"text/javascript\">AddLanguageSpecificTextSet(\"LST7F1E7F6D_4?cs=()|vb=|cpp=()|nu=()|fs=()\");</script>": {
								"link": "M_Blueshirt_Core_Crm_Panel_getXPanelHeaderLink.htm",
								"description": "\n            Format an XPath for finding a context link located in the header of a panel.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"GridRowExists(IDictionary<span id=\"LST7F1E7F6D_5\"></span><script type=\"text/javascript\">AddLanguageSpecificTextSet(\"LST7F1E7F6D_5?cs=&lt;|vb=(Of |cpp=&lt;|fs=&lt;'|nu=(\");</script>String, String<span id=\"LST7F1E7F6D_6\"></span><script type=\"text/javascript\">AddLanguageSpecificTextSet(\"LST7F1E7F6D_6?cs=&gt;|vb=)|cpp=&gt;|fs=&gt;|nu=)\");</script>, String)": {
								"link": "M_Blueshirt_Core_Crm_Panel_GridRowExists.htm",
								"description": "\n            Check if a grid/datalist row exists.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
							"SectionDatalistRowExists(IDictionary<span id=\"LST7F1E7F6D_7\"></span><script type=\"text/javascript\">AddLanguageSpecificTextSet(\"LST7F1E7F6D_7?cs=&lt;|vb=(Of |cpp=&lt;|fs=&lt;'|nu=(\");</script>String, String<span id=\"LST7F1E7F6D_8\"></span><script type=\"text/javascript\">AddLanguageSpecificTextSet(\"LST7F1E7F6D_8?cs=&gt;|vb=)|cpp=&gt;|fs=&gt;|nu=)\");</script>, String)": {
								"link": "M_Blueshirt_Core_Crm_Panel_SectionDatalistRowExists.htm",
								"description": "\n            Check whether a row exists in a section's datalist.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
						},
						"fields": {

							"getXTabsBar": {
								"link": "F_Blueshirt_Core_Crm_Panel_getXTabsBar.htm",
								"description": "\n            Constant XPath for getting an element that indicates the top Tab bar has loaded an active Tab.\n            ",
								"public": "",
								"static": "",
								"declared": "",
								"notNetfw": ""
							},
						},
						"properties": {
							"Title": {
								"link": "P_Blueshirt_Core_Base_BaseComponent_Title.htm",
								"description": " (Inherited from BaseComponent.)",
								"public": "",
								"inherited": "",
								"notNetfw": ""
							}
						},
						"references": {
							"N_Blueshirt_Core_Crm.htm": "Blueshirt.Core.Crm Namespace"
						}
					}
				},
```
#####Notes on Class JSON Format: <a name="Class Notes"></a>
- All extracted date from the HTML files are inserted into the `params` object.  Some objects already have a `param` section, but this only contains parameters accepted by methods.  It is content extracted from the XML.

- The `name` is simply the name of the class.  This holds true for any other page for methods, fields, properties, events, overload methods, enumerations, etc. <a name="namenote"></a>

- The `summary` section is the text that appears at the top of the page which describes the class.  This exists in other objects as well.

- The `inheritance` key marks all information on the Classes Inheritance Heirarchy
  - Each key in `inheritance` is a link the the class, and each value is the text on the page representing that link
  - A key marked as `#` means that is the current page and so shouldn't be a link (`<a>`)
  - Some values may contain HTML code.  This is because some text is only populated `onLoad()` and so the HTML is needed.  A     list of scripts are included in the output JSON for this purpose.

- The `lower_syntax_text` tag is exactly that, the text placed below the Syntax box.

- Both the `namespace` and `assembly` hold the text for this information.  The `namespace` object has a key which is a link to the namespace page.

- Within the `syntax` object there are two bits of information to know
  - Each key is a tab within the Syntax section, named for the language that tab represents.
  - Each value is the text within that tab.

- Next there are the `constructors`, `methods`, `fields`, and `properties` sections.  These are lumped together because they're all formatted similarly
  - Each key within these sections is the name of an item in that list.  For example, `"Panel": {}` is the name of the constructor for `T:Blueshirt.Core.Crm.Panel`.  
  - Within this object is the `link` key whose value is the url to the page which coordinates to this object.  So `M_Blueshirt_Core_Crm_Panel__ctor.htm` is a link for the `Panel` constructor.  
  - The `description` key gives the text in the description column under the respective section for that item. The description for `Panel` is `Initializes a new instance of the Panel class`.  
  - Each subsequent key is related to the access and/or visibility of the item.  So `Panel` is `public`.  Others can be `public`, `private`, `static`, or `inherited`.  Other items are less important such as `declared` and `notNetfw`.
  - It's worth noting that some of the keys of items in the list of `methods`, `fields`, `properties`, or `constructors` might have HTML in them because there is text that doesn't show until the page is loaded.  Similarly to the 3rd bullet point under the inheritance section above.

- The `references` section has any references for that class.  It is formatted like the `inheritance` section in that the keys are the links and the value is the text on the page.  The `reference` section exists in many other JSON objects within the file.

## Method JSON Format <a name='Method'></a>
######(Files beginning in M_, generally pages with all information regarding a class)
```
`{
					"name": "M:Blueshirt.Core.Crm.Panel.getXDataListColumnValue(System.Int32,System.String)",
					"summary": "\r\n            Given the DOM index of a datalist column and the value for that column, return an XPath\r\n            to append to a datalist XPath for finding that value in the requested column index.\r\n            \r\n            No element will be found if the value does not exist in this column.\r\n            ",
					"param": [
						{
							"_": "The DOM index for the TD element representing the desired column.",
							"name": "columnIndex"
						},
						{
							"_": "The value corresponding the provided column.  ",
							"name": "columnValue"
						}
					],
					"params": {
						"syntax": {
							"C#": "public static string getXDataListColumnValue(\n\tint columnIndex,\n\tstring columnValue\n)",
							"VB": "Public Shared Function getXDataListColumnValue ( \n\tcolumnIndex As Integer,\n\tcolumnValue As String\n) As String",
							"C++": "public:\nstatic String^ getXDataListColumnValue(\n\tint columnIndex, \n\tString^ columnValue\n)"
						},
						"arguments": {
							"columnIndex": {
								"type": "&#xA0;<a href=\"http://msdn2.microsoft.com/en-us/library/td2s409d\" target=\"_blank\">Int32</a>",
								"description": "The DOM index for the TD element representing the desired column."
							},
							"columnValue": {
								"type": "&#xA0;<a href=\"http://msdn2.microsoft.com/en-us/library/s1wwdcbf\" target=\"_blank\">String</a>",
								"description": "The value corresponding the provided column.  "
							}
						},
						"return_val": {
							"type": "&#xA0;<a href=\"http://msdn2.microsoft.com/en-us/library/s1wwdcbf\" target=\"_blank\">String</a>",
							"description": "[Missing <returns> documentation for \"M:Blueshirt.Core.Crm.Panel.getXDataListColumnValue(System.Int32,System.String)\"]"
						},
						"references": {
							"T_Blueshirt_Core_Crm_Panel.htm": "Panel Class",
							"N_Blueshirt_Core_Crm.htm": "Blueshirt.Core.Crm Namespace"
						}
	}
```
#####Notes on Method JSON Format: <a name="Method Notes"></a>
- For information on the `name` and `summary` keys, see [Class Notes](#namenote)
