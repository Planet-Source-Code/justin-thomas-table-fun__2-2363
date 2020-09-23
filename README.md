<div align="center">

## Table Fun :\)


</div>

### Description

Fun with tables, make your boring old tables actually do something fun, this code will do onmouseover, onclick events, that will expand and contract a table, highlight it etc..

View a working sample here: http://65.4.131.57/Justin/tableDrop.asp
 
### More Info
 
To add multiple ones, just rename the ID's to like BorderMain1, BorderMain2, etc...

Going to have to do simple modifications to the code, as it prolly wont display properly and it isnt really long enough to upload a zip, anyhow pretty simple. If you have any questions email me.

Some user's may experience faint or dizziness from being overly impressed. :)

Disclaimer:

Im tired and that was a joke.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Justin Thomas](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/justin-thomas.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/justin-thomas-table-fun__2-2363/archive/master.zip)





### Source Code

```
<html>
<head>
<title>Table Drop</title>
<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
<!-- CSS Styles -->
<style type="text/css">
.tblContracted {
	cursor			: hand;
}
.tblExpanded {
	cursor			: hand;
}
.DescContracted {
	display			: none;
}
.DescExpanded {
	color			: #FFFFFF;
}
</style>
<!-- create the function to expand and contract the table -->
<script langauge="JavaScript">
<!--hide incase the browser doesnt support javascript
function tblExpand(objItem,objDesc) {
//check the current status of the table
	if (objItem.className == "tblContracted") {
	//then expand it
		objItem.className = "tblExpanded"
		objDesc.className = "DescExpanded"
		}
	else {
	//or contract it
		objItem.className = "tblContracted"
		objDesc.className = "DescContracted"
		}
	}
//-->
</script>
<!--e n d  s c r i p t -->
</head>
<body bgcolor="#FFFFFF" text="#000000">
<TABLE ID="BorderMain" width="16%" border="0" cellspacing="1" cellpadding="0" bgcolor="#65B1FF">
 <TR>
  <TD>
   <TABLE ID="Main" width="100%" border="0" cellspacing="0" cellpadding="0" height="0" bgcolor="#D5EAFF" class="tblContracted" onClick="tblExpand(this,tblDesc)">
    <TR>
     <TD height="21" valign="middle" align="center" onMouseOver="Main.style.backgroundColor='#EAF5FF'; BorderMain.style.backgroundColor='#0066FF';" onMouseOut="Main.style.backgroundColor=''; BorderMain.style.backgroundColor='#65B1FF';">
      <font face="Verdana" size="2" color="#0B84FF">Click here</font>
     </TD>
    </TR>
    <TR>
     <TD ID="tblDesc" valign="top" align="left" class="DescContracted" style="background-color:#FFFFFF; border-top:#65B1FF solid 1px;" onMouseOver="Main.style.backgroundColor='#EAF5FF'; BorderMain.style.backgroundColor='#0066FF';" onMouseOut="Main.style.backgroundColor=''; BorderMain.style.backgroundColor='#65B1FF';">
<font face="Verdana" size="1" color="#0B84FF">Your text goes here.font>
     </TD>
    </TR>
   </TABLE>
  </TD>
 </TR>
</TABLE>
</body>
</html>
```

