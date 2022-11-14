# Updating the IMSc60 webpage

## Lectures

Lectures are sorted into *Next*, *Upcoming* and *Past*. For making changes, edit
```
/imsc60/html/pages/lectureData.json
```
and update the following information.
```
{
"poster": "<path to the image file>",
"title": "title of the talk",
"speaker": "name of the speaker",
"affiliation": "speaker's affiliation",
"abstract":"abstract of the talk",
"dateTime":"yyyy-mm-dd hh:mm"
"time": "hh:mm - hh:mm",
"zoom": null				//change the value to 1 if the talk is happening offline
"youtubeLink": "livestream url"		//if zoom, then provide a link to matsciencechannel
}
```

## Gallery

to update the gallery with new photos, one has to edit
```
/imsc60/html/gallery/mediaData.json
```
and update the following information.
```
{
"caption": "<insert the caption that will be displayed in the bottom of the image when viewed in the gallery > lightbox>",
"url": "<insert relative url to the image file>",
"alt": "<insert alt text for the image>"
}
```
