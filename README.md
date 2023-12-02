## Aims

- [ ] Make life easier for admin at a college by downloading zoom
  recordings and uploading to vimeo

Three components to the project:
- Downloading the videos
- Uploading the videos
- Renaming the videos (and automation of it)
- User interface

JavaScript is what I am most familiar with, so we shall use node. And it
might be better in the long term to just shove everything into an
electron app, rather than making the user run it as a script

## Downloading the videos

- Check if Zoom has an API
  - That allows you to download a video
    - This exists see [here](https://developers.zoom.us/docs/api/rest/reference/zoom-api/methods/#operation/recordingGet)
    - There seems to be two APIs that we can use (GQL and REST)
      - I am familiar with GQL - so we shall make use of it
