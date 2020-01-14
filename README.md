# Flutter Community Transfer Guide 
Thank you for your interest in the Flutter Community! We look forward to receiving and featuring your package. 

To ensure all packages added are listed properly, there are a few steps you must take before your package can be added to the Flutter Community.  

With these steps, you can migrate your package over to the Flutter Community GitHub organization. 

1. [Create an issue on Flutter Community](#1)
2. [Get approval from a moderator](#2)
3. [Update pubspec.yaml](#3)
4. [Update the CHANGELOG.md and README.md](#4)
5. [Add Flutter Community as Pub uploader](#5)
6. [Publish your changes to Pub](#6)
7. [Notify the Flutter Community Team](#7)
8. [Transfer the package to Flutter Community](#8)

## <a name="1"></a> 1: Create an issue on Flutter Community
Before you can move your package over to the community organization, you first need to submit it by [creating an issue and filling out the template](https://github.com/fluttercommunity/community/issues/new?assignees=jeroen-meijer&labels=package+proposal&template=----package-proposal.md&title=Package+Proposal%3A+%5BPACKAGE+NAME%5D).

Once you’ve completed the submission form, verify that all fields have been properly filled out and then submit the ticket.

## <a name="2"></a> 2: Get approval from a moderator
After you’ve opened a ticket, a member of the Flutter Community team will review your package and decide whether to accept or reject your submission. Don’t worry, if it gets rejected, you’ll get feedback and will know what changes you could make to get it re-reviewed.

**Factors such as code quality, documentation and comments all determine whether or not your package is accepted, so please make sure your package looks its best when submitting your request!**

## <a name="3"></a> 3: Update pubspec.yaml
Now that your package has been accepted to Flutter Community, there are a few changes you need to make to your `pubspec.yaml` file.

### First, add the `maintainer` field to your `pubspec.yaml`.
Only one maintainer is currently supported. Format the value like the example below:
```yaml
...
maintainer: YOUR-NAME (@YOURGITHUBUSERNAME)
...
```

### Next, you need to modify the authors field to be an array (if it’s not already). This array should contain the author “Flutter Community” with the email address “community@flutter.zone” as the **first entry** like below:
```yaml
...
authors:
    - Flutter Community <community@flutter.zone>
    - YOUR-NAME <YOUR@EMAIL.COM>
...
```

*For an example on what a complete* ***pubspec.yaml*** *should look like, check out* [*this file from the package after_layout*](https://github.com/fluttercommunity/flutter_after_layout/blob/master/pubspec.yaml)*.*

## <a name="4"></a> 4: Update the CHANGELOG.md and README.md
Congratulations, you’ve updated your package and you’re almost finished.

(If you don’t yet have a CHANGELOG.md file in your package’s repository, please create one now. For an example on how to use and keep a changelog, check [keepachangelog.com](https://keepachangelog.com/en/0.3.0/).)

### Update the CHANGELOG.md to include the following entry (or something similar to it):
```markdown
- Moved package to Flutter Community
```

### Next, in your package’s README.md, add the Flutter Community package banner by adding the following piece of text **at the top of the file and change `PACKAGE_NAME` to the title of your package**:
```markdown
[![Flutter Community: PACKAGE_NAME](https://fluttercommunity.dev/_github/header/PACKAGE_NAME)](https://github.com/fluttercommunity/community)
```
*(If the banner doesn't display properly, don't worry - It will show up properly at a later date.)*

Once you’ve done that, **add your changes and commit them back to your repository**.

## <a name="5"></a> 5: Add Flutter Community as Pub uploader
Last but not least, add `community@flutter.zone` as an uploader on Dart Pub. This can be done using the following command: 
```sh
flutter packages pub uploader add community@flutter.zone
```

## <a name="6"></a> 6: Publish your changes to Pub
Finally, save you changes and push your updated files to Pub.
(Usually, this is done through running `flutter packages publish`.)

## <a name="7"></a> 7: Notify the Flutter Community team
Once you've made all the necessary changes above, please notify the member of the team who reviewed your package in the original package proposal issue. They will review your changes and add you as a member of the Flutter Community's GitHub.

## <a name="8"></a> 8: Transfer the package to Flutter Community
Now that you’re a member of Flutter Community’s GitHub organization, you can transfer your package repository.

Navigate to settings in your package GitHub’s repository, scroll to “Danger Zone” then select “Transfer repository”. After selecting this option, you will be presented with a pop up dialog prompting you to enter your repository name and the name of the GitHub organization you’d like to move the package to. For the second option, enter the name `fluttercommunity`.

If you would like a more detailed guide for transferring GitHub repositories, please see https://help.github.com/en/articles/transferring-a-repository

Once you have transferred your package, please contact us on the package transfer issue from before.

## You’re done!

Thank you for taking the time to transfer your package.

If you have any questions, feel free to ask for help in your package transfer issue or [open a new issue on the /community repository](https://github.com/fluttercommunity/community/issues/new/choose).

Sincerely,<br/>
\- The Flutter Community Team.

![](https://raw.githubusercontent.com/fluttercommunity/community/resources/banner.png)
