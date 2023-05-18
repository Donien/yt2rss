# What it does

This script takes in one or more URLs to YouTube Channels and returns their respective RSS feed URL (https://www.youtube.com/feeds/videos.xml?channel_id=**CHANNEL_ID**).

**Overview:**

- RSS feed URLs are printed to stdout.
- When being provided with an **invalid URL** this script will print to **stderr** and keep going.

# Usage

**Using CLI arguments:**

```
python3 yt2rss https://youtube.com/@YOUTUBER1 https://youtube.com/@YOUTUBER2 https://youtube.com/@YOUTUBER3 ... https://youtube.com/@YOUTUBERn
```

**Using stdin (newlines and whitespaces as separators):**

```
echo https://youtube.com/@YOUTUBER1 https://youtube.com/@YOUTUBER2 https://youtube.com/@YOUTUBER3 ... https://youtube.com/@YOUTUBERn | python3 yt2rss 
```

or

```
printf "https://youtube.com/@YOUTUBER1\nhttps://youtube.com/@YOUTUBER2\nhttps://youtube.com/@YOUTUBER3\n ... https://youtube.com/@YOUTUBERn" | python3 yt2rss 
```

or

```
cat url_list.txt | python3 yt2rss
```
