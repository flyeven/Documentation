---
title: GitHub
---
{% include cloud_storage.md %}

Go to *Storage Providers* in your website configuration and click *Connect* next to GitHub.

![Storage Providers](/img/cloud_storage/github/1.png){: .screenshot}

This will redirect you to GitHub. Log in and authorise CloudCannon access to your GitHub Account.

![GitHub](/img/cloud_storage/github/2.png){: .screenshot}

You'll be redirected back to CloudCannon to pick a repository to connect. If you don't have one for this website, create a new one in GitHub and refresh this page.

A dialog box will appear asking for the master source for the initial synchronisation. This only matters if you have existing files in CloudCannon or your repository. The arrow shows the direction of file transfer and points to the source that will be overwritten. Click *Connect GitHub*.

![Inital Transfer](/img/cloud_storage/github/5.png){: .screenshot}

GitHub is now connected. Changes you push to the Git repository are pulled in by CloudCannon. Any changes made on CloudCannon are automatically committed and pushed.

![Inital Transfer](/img/cloud_storage/github/6.png){: .screenshot}

### Adding a new GitHub Organisation

If you add a GitHub Organisation after you have granted access to CloudCannon you'll need to manually allow access.

To do this open the settings for the Organisation on GitHub and go to the *Third-party access* tab. Click on *your own authorised applications* under the *No pending requests* header.

![Inital Transfer](/img/cloud_storage/github/7.png){: .screenshot}

Click on *CloudCannon*.

![Inital Transfer](/img/cloud_storage/github/8.png){: .screenshot}

Click **Grant Access** next to your new organization.
![Inital Transfer](/img/cloud_storage/github/9.png){: .screenshot}
