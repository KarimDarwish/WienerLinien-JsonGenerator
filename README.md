WienerLinien - Json Generator
=================

This simple C# class combines the 3 static CSV files with data from the Wiener Linien and parses them to 1 single JSON string.

It is used in the [WienerLinien.NET](https://github.com/KarimDarwish/WienerLinien.NET) library.


Usage
-------------

Simply call the `GetJsonAsync()` method and have the JSON string returned to you.
You can change the model/schema of the JSON file by editing the `WienerLinienModel` class.

You'll need [Json.Net](www.newtonsoft.com/json) for this, if you dont want to use a 3rd party library you can replace the serialization of the object with a 
`System.Web.Extensions.JavaScriptSerializer`



Example
-------------------
Sample JSON:

    [{
    		"StationId": 214461177,
    		"Typ": "stop",
    		"Diva": "60201095",
    		"Name": "Reumannplatz",
    		"Municipality": "Wien",
    		"MunicipalityId": 90001,
    		"Wgs84Lat": 48.174154518495,
    		"Wgs84Lon": 16.3781920579012,
    		"Stand": null,
    		"Platforms": [{
    				"Line": "214433687",
    				"Realtime": true,
    				"MeansOfTransport": 1,
    				"RblNumber": 4101,
    				"Area": "1",
    				"Direction": "H",
    				"Order": "1",
    				"PlatformName": "214689583",
    				"PlatformWgs84Lat": 48.1748733834472,
    				"PlatformWgs84Lon": 16.3779854453859,
    				"StationId": 214461177
    			}, ...





Credits
-------------

 - [Json.NET](http://www.newtonsoft.com/json) 


License
--------------

MIT License

Copyright (c) 2016 Karim Darwish

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.




