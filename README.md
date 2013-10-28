POC-NCCGROUP-API-WRITE
======================

Description:
Proof of Concept for using the write functionality of the NCC Group Web Performance API.

These web pages have been developed as a desktop display aimed at providing a simple and easy-read means to change the monitoring status of an organisation's web sites.

To be used for Proof-of-Concept, prototype and demonstration purposes by authorised customers of the NCC Group Web Performance API service.

Created through an agile and evolutionary development method and maintained on an ad-hoc basis.

Technologies:
- HTML 5 canvas, JavaScript, jQuery, AJAX, PHP, XML, SteelSeries Javascript library.

Installation instructions:
- Unzip all files into a web server directory

Installation Pre-Requisites:
- PHP 5.3+ with PHP cURL installed (PHP v5.2 won't work correctly)

Operation instructions:
- open "api_monstat2.htm" from the web server location
- enter your NCC Group Portal username and password
- click "Get accounts"
- select 1 or more accounts from the listbox
- optionally enter a list of comma separate monitor ids - normally leave blank to view all monitors
- click "Get data"
- check the "Confirm Write Enabled" checkbox (you won't be able to use API write functions without this)
- once displayed:
    - set toggle indicator on one or more pages or user journeys
      - optionally select all or none of the monitors (feature not yet fully implemented)
    - set timer 1, and optionally timer 2, to automatically change the monitoring status of the toggled monitors
      - set the number of minutes ahead of current time at which toggle is to be made 
- view the monitors that are temporarily toggled
    - monitors with a changed monitoring status are highlighed in blue

Features for the future:
- to enhance the page to provide additional configuration capability
- to save the monitor selection as a profile
- to load a saved monitor profile
- to write an application to use the profile and update monitoring status indepenently (to cover maintenance windows)
- to add additional alerting reading/setting capability, particularly for steps of a user journey

Browsers:
- Google Chrome
- Mozilla Firefox
- Microsoft Internet Explorer 10 (earlier versions may not work as expected)
- Tablets partially supported (media types added):
    - 1280x800 resolution screens (typical Android tablets)
    - 1024x768 resolution screens (iPad)

Notes:
- XML data is pulled back from the API by PHP pages using cURL
- each toggle of each monitors will utilise an API call and will count against your daily API call allowance
- these pages should only be used if you have not already developed a solution to change monitor status


Copyright (c) 2013 Tim Daish BA(Hons) MBCS CTAL-TM

    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the "Software")
    the rights to use, copy, modify, merge, publish and distribute copies of the Software,
    and to permit persons to whom the Software is furnished to do so.
    The Software may not be sold or rented. Modification is encouraged to meet individual needs.
    Support from the Author will only be provided against the original Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
    OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
    IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
    CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
    TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
    OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
