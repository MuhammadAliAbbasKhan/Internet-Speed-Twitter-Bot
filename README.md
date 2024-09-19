# Internet Speed Twitter Bot

A Python-based bot that checks your internet speed using Speedtest.net and tweets your internet service provider (ISP) if the speed is slower than what you’re paying for. This bot automates the process of speed testing and notifying your ISP on Twitter, helping you hold them accountable for slow speeds.

## Features:
- Automatically checks your internet speed using Speedtest.net.
- Tweets at your ISP if the speeds are below the promised rates.
- Easy to customize with your own speed thresholds and Twitter account.

## Requirements:
- Python 3.x
- Selenium WebDriver
- Google Chrome Browser and ChromeDriver

## Installation:

1. **Clone the repository**:

    git clone https://github.com/yourusername/internet-speed-twitter-bot.git
    Install the required libraries:
    pip install selenium
    Download and install ChromeDriver: Download the version of ChromeDriver that matches your installed Google Chrome browser from here.



Set up environment variables: Replace the placeholders in the script with your own credentials:

PROMISED_DOWN: The download speed promised by your ISP.
PROMISED_UP: The upload speed promised by your ISP.
CHROME_DRIVER_PATH: The file path where ChromeDriver is installed.
TWITTER_EMAIL: Your Twitter login email.
TWITTER_PASSWORD: Your Twitter password.
Example:
PROMISED_DOWN = 150
PROMISED_UP = 10
CHROME_DRIVER_PATH = "path_to_your_chromedriver"
TWITTER_EMAIL = "your_twitter_email"
TWITTER_PASSWORD = "your_twitter_password"

Usage:
Run the script:
    python internet_speed_bot.py
How the script works:
    The bot opens Speedtest.net in a Chrome browser and runs a speed test.

If the download or upload speed is below the specified thresholds, it logs into Twitter and tweets your ISP about the slow speed.

Customization:
    Speed Thresholds: Modify the PROMISED_DOWN and PROMISED_UP variables to match the speeds promised by your ISP.
    Tweet Message: Customize the tweet message in the tweet_at_provider() method to say whatever you'd like when the speed is too slow.

Troubleshooting:
    Element not found errors: If you encounter NoSuchElementException, it might be because the XPaths in the script no longer match the website. You can update the XPaths by inspecting       the elements on Speedtest.net or Twitter.

ChromeDriver issues:
      Ensure that the version of ChromeDriver you're using matches the version of Chrome installed on your system.

Legal Disclaimer:
      This project is for educational purposes only. Automating interactions with Speedtest.net and Twitter may violate their terms of service, and using this bot could result in your          account being restricted. Use at your own risk.

License:
      This project is licensed under the MIT License - see the LICENSE file for details.

          You can use this **LinkedIn** description, **GitHub** description, and **README** file to provide a comprehensive overview of the Internet Speed Twitter Bot.






