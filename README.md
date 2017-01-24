# Arnaud Templates for SAP NetWeaver 2-tier template based on Marketplace image

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https://raw.githubusercontent.com/arnaudlh/SAP-2tiers/master/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https://raw.githubusercontent.com/arnaudlh/SAP-2tiers/master/azuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template takes a minimum amount of parameters and deploys a VM that is customized for use with SAP NetWeaver, using the latest patched version of the selected operating system. 
This is a template for a 2-tier configuration. It deploys 1 server on either Standard or Premium Storage.

There is not suitable configuration for X-Large with Standard Storage. If you select this configuration, the template will deploy a Large configuration.

<table>
	<tr>
		<th>Size</th>
		<th>Premium Storage</th>
		<th>Standard Storage</th>
	</tr>
	<tr>
		<td>Small < 2.000 SAPS</td>
		<td>1xDS11 (2xP20 1xP10)</td>
		<td>1xD11</td>
	</tr>
	<tr>
		<td>Medium < 9.000 SAPS</td>
		<td>1xDS13 (3xP20 1xP10)</td>
		<td>1xD13</td>
	</tr>
	<tr>
		<td>Large < 18.000 SAPS</td>
		<td>1xDS14 (3xP30 + 1xP20)</td>
		<td>1xD14</td>
	</tr>
	<tr>
		<td>X-Large < 40.000 SAPS</td>
		<td>1xGS5 (4xP30 1xP20)</td>
		<td>1xD14</td>
	</tr>
</table>				