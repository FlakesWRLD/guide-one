## ⚠️ Disclaimer ⚠️

### <p align="justify">I will not be responsible for what you will do with the following guide and how you will use bot. You will be responsible for your own actions.</p>

## 🥺 Humble Request 🥺

### <p align="justify">I request you all please don't abuse this beautiful platform heroku or overload it with large numbers of data we all know it's a free platform which provides us amazing features but some users will uses bot for large numbers of groups please don't do that i prefer if you have friends just make small groups or use yourself privately.</p>

# Guide for Deployment of Torrent Drive Bot

<p align="justify">This guide I have invented myself to avoid the suspension of our app because Heroku has banned peer-to-peer services and they have included in their new terms and services that any kind of peer-to-peer activity if they detect them in their apps they will ban it immediately.</p>

### Peer 2 Peer Services are like:

```Torrent and Many More```

<p align="justify">Downloading of files & torrents in linux based os specifically we only use Aria2c. Basically, most of the bots nowadays use only aria2c to provide users a better experience.</p>

## Follow The Guide:

- Clone the repo:
```
git clone https://github.com/usmanmughalji/drive-bot-ultimate
cd drive-bot-ultimate
```
- Setting up config file (You should know, how to fill them) [Click Here To Know More](https://github.com/usmanmughalji/drive-bot-ultimate#setting-up-config-file)
```
cp config_sample.env config.env
```
- Remove following files
```
rm -rf .git Dockerfile README.md extract heroku.yml netrc requirements.txt config_sample.env
```
- Now run following command to tar following files
```
tar -cvf galaxy.tar .
```
- Click on following link and download the following zip

* [Download](https://github.com/usmanmughalji/guide-one/raw/main/files.zip)

Extract that zip in another folder and absolutely it will extract in `files` folder after extracting you will see following number of files
```
* app.json
* Dockerfile
* extract
* heroku.yml
* netrc
* README.md
* requirements.txt
```
Now Make new private repo on your github and add following files manually to your repo

Most important thing here is that you also have to add that `galaxy.tar` file to the repo

Now deploying part

We have to edit now `README.md` file to put your own github user name and repo link

Example:

`template=https://github.com/put-your-git-user-name/put-your-repo-name-here-where-did-you-uploaded-your-bot-files/tree/main`

By doing this only your specified repo will be deployed on heroku

You should have once authorize your git account to heroku for deployment of private repos

* [Click Here To Know More](https://devcenter.heroku.com/articles/github-integration)

Once you have authorized your git account to heroku you will be easy to deployed any private repo

Now click on deployment button and deploy

After deployment is complete now go to resources section and `turn on dynos` if you have done everything properly it will run properly
