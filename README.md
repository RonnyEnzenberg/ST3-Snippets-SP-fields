The ultimate Sharepoint field Snippets for Sublime Text 3
==========================================================

I was tired of still using microsofts Sharepoint Designer for editing pagelayouts and inserting the fields in SharePoint. So i created some Sublime Text 3 Snippets which do that for me.

The usage is quite simple. Just get yourself the snippets located in the snippets folder and paste them into your Sublime Text 3 snippet folder. 
Normally you will find it under C:\Users\USER\AppData\Roaming\Sublime Text 3\Packages\User\PUT-ALL-YOUR-SNIPPETS-HERE

If you don't see the AppData-Folder you set hidden folders to visible in your explorer settings.

### How To

1. Type `sp-field-"fieldtype"`
2. Hit the `tab` - Key
3. Enter your fieldname

The Snippets add your field with field name to your code. 

**Important:**
As Sharepoint shows your field only as plain data in display mode (whithout label and div containers as wrappers) which it will normally do,  but you want your pagelayout to show also a label in display mode you can use the same snippet with the post-fix "-dspl"
f.E.: `sp-field-datetime-dspl`

It will render your Sharepoint field with the same div's and CSS-classes Sharepoint uses in edit mode, so you only have to style your CSS once. 

`<div class="ms-formfieldcontainer">  
	<div class="ms-formfieldlabelcontainer">  
		<span class="ms-formfieldlabel">  
			<SharePointWebControls:FieldLabel runat="server" FieldName="" />  
		</span>  
	</div>  
	<div class="ms-formfieldvaluecontainer">  
		<SharePointWebControls:DateTimeField FieldName="" runat="server"/>  
	</div>  
</div>`

**Available Snippets are:**
* Boolean Field : `sp-field-bool` for edit-mode and `sp-field-bool-dspl` for display-mode
* Datetime Field : `sp-field-datetime` for edit-mode and `sp-field-datetime-dspl` for display-mode
* Lookup Field : `sp-field-lookup` for edit-mode and `sp-field-lookup-dspl` for display-mode
* Number Field : `sp-field-num` for edit-mode and `sp-field-num-dspl` for display-mode
* Taxonomy Field : `sp-field-taxonomy` for edit-mode and `sp-field-taxonomy-dspl` for display-mode
* Text Field (single line) : `sp-field-text` for edit-mode and `sp-field-text-dspl` for display-mode
* Note Field (text multi line) : `sp-field-textarea` for edit-mode and `sp-field-textarea-dspl` for display-mode
* User Field (people picker) : `sp-field-user` for edit-mode and `sp-field-user-dspl` for display-mode

I hope you enjoy this. Let me know if you find some issues.

Best regards,
Ronny




