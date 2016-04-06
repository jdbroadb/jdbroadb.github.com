---
title: Dais Dropbox Syncing
date: 2014-09-04 09:20 AM
categories: Dais
---

When I decided to try out Heroku I quickly learned that the only access to the file system is through Git pushes of your application. That works great for the actual Ruby code but it very limiting for content. So I decided to sync Dais with my Dropbox account. It was a logical choice because I already store and access all my posts in Dropbox through Editorial on my iOS devices.

### Dropbox API

I had never used the Dropbox API so I wasn't sure how complicated it would be. Thankfully they have a Ruby SDK that made the process extremely simple.

	require 'dropbox_sdk'

	ACCESS_TOKEN = #Get from Dropbox App settings

	# Create Dropbox client
	dropbox = DropboxClient.new(ACCESS_TOKEN)

	# Cursor to sync changes
	@db_cursor = nil

	# Directory to sync
	@posts_dir = '/posts'

	# Grab changes
	db_data = dropbox.delta(@db_cursor, @posts_dir)

That's all it took to start syncing content.

### Account Setup

Now it also required some setup from my Dropbox account. Go to the [Dropbox developer app site](https://www.dropbox.com/developers/apps) to setup a new app with your account.

![Dropbox access token](../Images/dropbox-access-token.jpg)

Dropbox provides a personal authentication token that you can use when only needing to access your own account. Just push the "Generate access token" button. This is incredibly handy for a project like this so I can avoid performing an Oauth cycle. I simply enabled the option in my account and copied the token into my application.

### Refreshing

Once I could access the data I set up a simple thread to re-access the data at a set interval. This allowed me to push updates by simply copying files to Dropbox and I know the changes will take affect within a certain amount of time. Also, the API provides for me to only grab changes so I don't need to reread every file on every update.
