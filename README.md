# TableList

<a href="https://ci.appveyor.com/project/bantikyan/tablelist"><img src="https://ci.appveyor.com/api/projects/status/ectnla0f5r58yg2m/branch/master?svg=true" alt="Build status"></a>

This package gives ASP.Net developers easy way of editing list of items with model binding. This means you can edit elements of your list inline, and all changes will be submited with form. For this purpose ```Html.TableListFor``` HTML helper was developed both for ASP.NET Core and ASP.NET MVC.

Usage is very simple. If your ```Model``` is a ```List``` or you have any ```List``` properties in your ```Model``` you want to make them editable, you simple need to derive them from ```TableListItem``` class and use ```Html.TableListFor``` HTML helper on your ```View```. All CRUD operations are supported.

## Table of contents

* <a href="#user-content-installation">Installation</a>
* <a href="#user-content-basic-usage">Basic Usage</a>
* <a href="#user-content-aspnet-mvc-syntax">ASP.NET MVC syntax</a>
* <a href="#user-content-color-schemes">Color schemes</a>
* <a href="#user-content-license">License</a>

## Installation

Library consist of back-end  and front-end parts.

Front-end components can be installed one of the following sources:
* Install with [Bower](https://bower.io): <code>bower install tablelist-mvc</code>
* Install with [npm](https://www.npmjs.com/package/tablelist-mvc): <code>npm install tablelist-mvc</code>
* Install with [Nuget](https://www.nuget.org/packages/tablelist-mvc): <code>Install-Package tablelist-mvc</code>
* Use CDN [jsDelivr](https://www.jsdelivr.com/package/npm/tablelist-mvc)

Back-end components for ASP.NET Core:
* Install with [Nuget](https://www.nuget.org/packages/TableList.Mvc.Core): <code>Install-Package TableList.Mvc.Core</code>

Back-end components for ASP.NET MVC:
* Install with [Nuget](https://www.nuget.org/packages/TableList.Mvc): <code>Install-Package TableList.Mvc</code>

Also you can download the latest release: 
* [Download the latest release](https://github.com//bantikyan/icheck-bootstrap/archive/3.0.1.zip)

## Basic Usage

First make sure you have linked css and js files: ```tablelist-mvc.css``` and ```tablelist-mvc.js``` or minimized versions. We use JQuery so link to jquery file must be before link of ```tablelist-mvc.js```. Also if you have some validation attributes, validation js files needed to be linked.

Your page may look like this: 
```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
    <link rel="stylesheet" href="tablelist-mvc.css" />
</head>
<body>
    ...

    <script src="jquery.js"></script>
    <script src="jquery.validate.js"></script>
    <script src="jquery.validate.unobtrusive.js"></script>
    <script src="~/js/tablelist-mvc.js"></script>
</body>
</html>
```

## License

TableList released under the [MIT license](https://github.com/bantikyan/TableList/blob/master/LICENSE). Feel free to use it in personal and commercial projects.
