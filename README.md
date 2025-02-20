Image Open Social Links How-To:

## About:
Image Open Social links is an old "gadget" feature of Google Sites that a lot  of web bl0ckers ignore for whatever reason


## How to Make One:
First make an XML file in a GitHub Repo:
```xml
<?xml version="1.0" encoding="UTF-8" ?>
<Module>
<ModulePrefs title="Your_Title_Here" />
<Content type="html"><![CDATA[

HTML HERE!

]]></Content>
</Module>
```

With html code in between the `<Content type="html"><![CDATA[` and `]]></Content>` tags (make sure to use a CDN for ALL external recources, like images, styles, or JS

Copy the link to the file in your *public* GitHub repo and go to [JSDelivr](https://www.jsdelivr.com/github) and get your JSDelivr CDN link

Then make an Image Open Social link using the format below:

`https://WHATEVERYOUWANT-opensocial.googleusercontent.com/gadgets/ifr?url=YOUR_JSDELIVR_XML_LINK&container=ig`

Replace `WHATEVERYOUWANT` with any string of characters and `YOUR_JSDELIVR_XML_LINK` with your JSDelivr XML file

You're good to go!
