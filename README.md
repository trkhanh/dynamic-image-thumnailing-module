Installation & Config
The thumbnailer utilizes Intervention/Image (http://image.intervention.io/) for thumbnail processing. To get started:

Install Intervention/Image in the Directus root by running composer require intervention/image
Clone the thumbnailer in the Directus root by running git clone git@github.com:directus/thumbnailer.git
Modify settings as needed in. config.json
Examples
The follwing examples can executed by copying the url into the browser.

Crop Best 200x300
URL: directus.example.com/thumbnail/200/300/crop/best/my-file.jpg
RESULT: Cropped file of best quality
FILE LOCATION: thumbnail/200/300/crop/best/my-file.jpg
200x300
URL: directus.example.com/thumbnail/200/300/my-file.jpg
RESULT: Cropped (default) file of good (default) quality
FILE LOCATION: thumbnail/200/300/my-file.jpg
Contain 100x100
URL: directus.example.com/thumbnail/100/100/contain/my-file.jpg
RESULT: Resized file (aspect ratio preserved) of good (default) quality
FILE LOCATION: thumbnail/100/100/contain/my-file.jpg