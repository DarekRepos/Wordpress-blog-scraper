# Ski-jump-scraper
copies contents from the ski jump website and save to external file

# Run Python script at startup in Ubuntu


## Copy repository files to your Desktop

## Copy the python file to /bin:

sudo cp -i  ~/Desktop/scrapeskisite.py /bin

## Add A New Cron Job:

sudo crontab -e

## Scroll to the bottom and add the following line (after all the #'s):

@reboot python ~/Desktop/scrapeskisite.py &

The “&” at the end of the line means the command is run in the background and it won’t stop the system booting up.

## Test it:

sudo reboot
