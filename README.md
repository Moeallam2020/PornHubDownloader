# PornHubDownloader
A pornhub.com downloader that allows you to login so you can download everything you have access to, including but not limited to private videos, 1080p or higher resolutions, premium videos and even paid videos that you own.

#### Supports the following things:

* Premium videos
* 1080p and higher resolution
* Private videos (not working since: 22nd of December 2020, ETA for fix: None until PH builds back a working catalogue of content)
* Paid videos (untested)

#### How does it work?

The script logs in on the account you supplied, then visits the link you supplied and downloads sthe video in the highest resolution availabe.

Logging in is optional however in order to enjoy the features that other downloaders seem to lack it is necessary.

Cookies will be stored locally in an encrypted manner so you don't have to worry about people stealing your account nor pornhub blocking your account for suspicious activity after X logins.

Downloading too many videos too quickly will result in the failure of the script, you need to visit the url in such case and do the captcha before you can resume to download again.

#### Examples

Regular URL: https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7

Premium url: https://www.pornhubpremium.com/view_video.php?viewkey=ph5cc5d3bdc5b02

Downloading a single video

```PHDownloader.exe -URL=https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7```

This would result in a file called: ```little black dress and pink hair quick jillin off before party.mp4``` to be downloaded, the 720P version in this case.


However if you login with a premium account:

```PHDownloader.exe -URL=https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7 -username=darfttygkbhn -pasword=adcfvhbgfsdg```

Now it downloads a file called: ```little black dress and pink hair quick jillin off before party.mp4``` but it would be the 1080P version.


You can also add the flag -withuploader=true like this:

```PHDownloader.exe -URL=https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7 -username=darfttygkbhn -pasword=adcfvhbgfsdg -withuploader=true```

Or:

```PHDownloader.exe -URL=https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7 -withuploader=true```

This would affect the filename, now the file will be called ```Euro Coeds - little black dress and pink hair quick jillin off before party.mp4``` because ```Euro Coeds``` is the uploader of the video


Alternatively you can save the links into a file in this fasion:

```
https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7
https://www.pornhubpremium.com/view_video.php?viewkey=ph5cc5d3bdc5b02
https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7
https://www.pornhubpremium.com/view_video.php?viewkey=ph5cc5d3bdc5b02
https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7
https://www.pornhubpremium.com/view_video.php?viewkey=ph5cc5d3bdc5b02
https://www.pornhub.com/view_video.php?viewkey=ph5ca48baebd5d7
https://www.pornhubpremium.com/view_video.php?viewkey=ph5cc5d3bdc5b02
```

Save the file in the folder with the executable (or know the path to the file u just saved)

For this example let's say I saved it next to the executable with the name ```listofvids.txt```

Then now I can download all the videos using this command:

```PHDownloader.exe -list=listofvids.txt```

As mentioned above you can add the other flags to login and to save files with uploader names prepended.


## Disclaimer

Use at own risk.

#### My experience
The downloader seems to be able to do 60+ videos of decent size without getting captchas but this was with a temporary premium account.

The program automatically crosses off the videos it managed to download from your list in case some fail you don't have to URL hunt

This is by far the most complete downloader around.

#### Future
I don't plan on actively working on this project, I will update when I have time in case bugs occur caused by pornhub updating their services.

Feel free to try to crack the .cookies file, if you succeed and can tell me how you did it it would be appreciated because I could always use tips on how to improve security.

If a feature is missing let me know.

If you think this program automatically does cool things and you get mad it can only download the files that your account has access to, please gkys.
