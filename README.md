# As of 03//07//25 I am sad to announce that Image Open Social Links no longer are supported on any platform.

Image Open Social Links How-To:

## About:
Image Open Social links is an old "gadget" feature of Google Sites that a lot  of web bl0ckers ignore for whatever reason


## How to Make One:

[Video Tutorial](https://youtu.be/52dn2tt5Lhg)

First make an XML file in a public GitHub Repo:
```xml
<?xml version="1.0" encoding="UTF-8" ?>
<Module>
<ModulePrefs title="Your_Title_Here" />
<Content type="html"><![CDATA[

HTML HERE!

]]></Content>
</Module>
```

With html code in between the `<Content type="html"><![CDATA[` and `]]></Content>` tags (make sure to use a CDN for ALL external recources, like images, styles, or JS, I reccomend JSDelivr)

Copy the link to the XML file in your *public* GitHub repo (the best thing to do is to copy te __permalink__) and go to [JSDelivr](https://www.jsdelivr.com/github) and get your JSDelivr CDN link

Then make an Image Open Social link using the format below:

`https://WHATEVERYOUWANT-opensocial.googleusercontent.com/gadgets/ifr?url=YOUR_JSDELIVR_XML_LINK&container=ig`

Replace `WHATEVERYOUWANT` with any string of characters and `YOUR_JSDELIVR_XML_LINK` with your JSDelivr XML file. Make sure to keep `&container=ig` at the end or it won't work

## Example:
This is the `gnspn.xml` file in this repo:
```url
https://psd0620-pssis-opensocial.googleusercontent.com/gadgets/ifr?url=https://cdn.jsdelivr.net/gh/LupineVault/imageopensocial@9f1eff6ce4e7a418ad4783259673b2e9b71aca19/gnspn.xml&container=ig
```

You're good to go!
