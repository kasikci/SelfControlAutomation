SelfControlAutomation
=====================

A customized script to automate SelfControl. The original script is due to: http://hints.macworld.com/article.php?story=20100801214648362. I simply modified the time to fit my need and run for 23 hours (1380 minutes) once I activate it.

To automate the script:

1. Export the script as a app from the Apple script editor (I exported it as SelfControlAutomate-23.app)
2. Create a crontab entry

```console
$ crontab -e
```

3. Add the entry you want. I want the script to execute every day at 22 and run for 23 hours

```console
07 22 * * * open /Applications/SelfControlAutomate-23.app
```