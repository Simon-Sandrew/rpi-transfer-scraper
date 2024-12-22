# RPI Transfer Class Scraper

Spreadsheet from a run on Dec 22nd, 2024: [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1ufciRyXItZgLiQv5-lFR-pyhxhZX8vUkGVVRPe9WTIE/edit?usp=sharing)

# Background
RPI's [class transfer list](https://tes.collegesource.com/publicview/TES_publicview01.aspx?rid=f080a477-bff8-46df-a5b2-25e9affdd4ed&aid=27b576bb-cd07-4e57-84d0-37475fde70ce) is not very good. This is a short script that scrapes every class on the webpage.

# Running this scraper Yourself
The current configuration is set up to run four sessions at once, which will more than likely result in getting rate-limited by the captcha. You'll know this has happened when the scraping stops for around 5-10 seconds. If/when this happens, complete the following:
1. Refresh the page.
2. Complete the captcha.
3. Navigate back to the previous page (if you don't remember, I print out the page number and the action that it failed on; CTRL + F "failed" in the output).
4. Wait upwards of 90 seconds.

When this happens, we pause for 90 seconds so you can complete the above. Simply wait for it to continue after you've navigated to the correct spot, and you should be all set. This happens about 1-2 times if you are running four sessions at once for a complete run.

# How to improve this scraper
1. Use some multi-modal LLM to solve the captchas automatically (or however captchas are solved nowadays).
2. Enable proxies of some kind so you can skirt the captcha more often.
3. Run in headless mode or something.
