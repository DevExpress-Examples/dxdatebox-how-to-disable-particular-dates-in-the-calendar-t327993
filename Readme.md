# dxDateBox - How to disable particular dates in the calendar


<p>Currently, dxDateBox does not provide API that allows you to disable specific dates: <a href="https://www.devexpress.com/Support/Center/p/T260958">T260958: dxDateBox - Is it possible to disable dates?</a>. However, it is possible to implement a workaround. The main idea is to select elements with necessary content by using jQuery and disable them. To get the information about a particular calendar cell, use the "aria-label" attribute (this is the most convenient way to determine the day of the week for a particular cell) or any other HTML attribute that meets your requirements (for instance, "data-value").</p>
<p> </p>
<p>To determine the appropriate attribute, inspect the elements in the calendar like it is described in the <a href="https://www.devexpress.com/Support/Center/p/K18570">K18570: How to inspect CSS rules</a> article.<br><br></p>
<p>P.S. If you are localizing your dxDateBox widget with Globalize or other localization tools, make sure that you update the code in our example with the corresponding localized month names in the disableDates function. In other words, replace 'Saturday' with your localized month name.</p>

<br/>


