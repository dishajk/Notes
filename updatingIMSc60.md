# Updating the IMSc60 webpage

## Lectures

Lectures are automatically sorted into *Next*, *Upcoming* and *Past*. For making changes, edit
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
"zoom": null,
"youtubeLink": "livestream url"
}
```
If the talk is happening over zoom use `"zoom": 1` and provide a link to matsciencechannel for `"youtubeLink"`

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
