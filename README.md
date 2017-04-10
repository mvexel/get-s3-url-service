# Get S3 URL

A Mac OSX service to get the public S3 URL for a file in a folder on your Mac that is synced with an S3 bucket

## Use case

Say you have a folder on your Mac that you sync with an S3 bucket using something like this:

`aws s3 sync ~/Screenshots/ s3://diary-image-hosting`

This syncs my `Screenshots` folder to an S3 bucket so I can link to them when I write a blog post. While I am writing, I want to be able to access that link quickly. That is where this Service comes in.

## Installation

* Download the `Get Public S3 URL`
* Double-click
* When asked, click `Open with Automator`
* In the `Run Shell Script` part of the workflow, find the `https://diary-image-hosting.s3.amazonaws.com/` bit and change it to your S3 bucket root URL.
* Save

## Usage

* Right-click on the file you want to link for
* Go to `Services` > `Get Public S3 URL`
* The URL is now on the clipboard.


