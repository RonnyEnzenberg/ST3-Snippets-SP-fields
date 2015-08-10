The ultimate Sharepoint fields Snippets for Sublime Text 3
==========================================================

Sublime text 3 Snippets for inserting SharePoint fields in a page layout without using SharePoint Designer of microsoft.

The usage is quite simple. Just get yourself the snippets located in the snippets folder and paste them into your Sublime Text 3 snippet folder. 
Normally you will find it under C:\Users\*you*\AppData\Roaming\Sublime Text 3\Packages\User\*put all your snippets here*

If you don't see the AppData-Folder you set hidden folders to visible in your explorer settings.

### How To

1. Type sp-field-`fieldname`
2. Hit the "tab"-Key
3. Enter your fieldname

The Snippets add your field with field name to your code. 

**Important:**
As Sharepoint shows your field only as plain data in display mode (whithout label and div containers as wrappers) which it will normally do,  but you want your pagelayout to show also a label in display mode you can use the same snippet with the post-fix "-dspl"
f.E.: `sp-field-datetime-dspl`

It will render your Sharepoint field with the same div's and CSS-classes like Sharepoint would do in edit mode so you only have to style your CSS once. 

`div class="ms-formfieldcontainer">
	<div class="ms-formfieldlabelcontainer">
		<span class="ms-formfieldlabel">
			<SharePointWebControls:FieldLabel runat="server" FieldName="" />
		</span>
	</div>
	<div class="ms-formfieldvaluecontainer">
		<SharePointWebControls:DateTimeField FieldName="" runat="server"/>
	</div>
</div>`

I hope you enjoy this. Let me know if you find some issues.

Best regards,
Ronny




