# Sprout 🌱

Not on GitHub as much as you'd like to be, but still want your contributions to show green? Sprout tends your GitHub contribution garden by writing the current date to a text file and committing it on a schedule. It uses cron to run automatically, planting a little green in your contribution graph one commit at a time.

## Installation

First, clone the repository. In order to git push via cron, you'll need to use SSH instead of HTTPS. You can change that in your directory using:

```
git remote set-url origin git@github.com:username/repo.git
```

Then, make a cron by typing the command below into your shell.

```
crontab -e
```

Below is an example of my cron job. The first section `23 0-20 * * *` designates the time the command will be executed. Mine runs every 23rd minute of the hour I am on my computer from Midnight to 8PM. For help scheduling your own cron the website [Cron Guru](https://crontab.guru/) is excellent.

```
23 0-20 * * * cd PATH_TO_YOUR_CODE/sprout; ./script.sh
```

The second part is the command you would like to run at that specific time. This one directs you to the code and executes the file. Be sure to put your own path in.

## Additional Options

If you want to make it looking like you're working even harder, when you clone this repository, change the name to something like `proxy-server-package`. No one will be the wiser.

## Contributing

If you'd like to contribute to this repository feel free to fork/submit a pull request, and if you have any suggestions feel free to email me at itsprinterscanner@gmail.com.
