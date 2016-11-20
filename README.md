# alexa_flash_briefing
Create Alexa Flash Briefing API compatible json feed.
https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/flash-briefing-skill-api-feed-reference

## configuration

set these Environment variables on lambda function.

### S3_DATA_BUCKET

S3 bucket with public access for json data.

### FEED_URL

Source RSS feed URL.

## Installation

```
cd alexa_flash_briefing
pip install -r requirements.txt -t $(pwd)
```

compress all files in to zip.
```
zip -r func.zip .
```

upload to lambda function

This function use long time to convert data.
Set the timeout to 5 minuets.
