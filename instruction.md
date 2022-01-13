# Functionality
The Bot is Capable of Scraping Last Message from A Specific Telegram Group/Channel/Message

Translating The Scraped Message into Simplified Chinese Using Deepl Translator

And Forward The Translated Message to One or More Group

Speciality of The Bot is : You Don't Need to be admin of the group to scrape message.

# Configuration
```JSON
{
    "last_id":"10",
    "first_run":false,
    "source":"https://t.me/tup2022",
    "scrape":"https://web.telegram.org/z/#-1784046691",
    "forward":["https://web.telegram.org/z/#-657341998"]
}
````

- last_id : number
  - indicates the id of the scraped message

- first_run: boolean
  - indicates if the bot is running for the first time
  - if first_run : true, a chrome window will popup , so that can bot user can login to the account which will be used for botting.

- source : string
    - The channel link from which we will scrape message
- scrape: string
    - The telegram web-version channel link from which we will scrape message
- forward : List of String
    - Telegram web-version channel link/links to which we will forward scraped & translated message


# Installation
- Download And Install Chrome
  - If Already Installed Verify Chrome.exe exists in this Directory C:\\Program Files\\Google\\Chrome\\Application
- Install NodeJS from [here](https://nodejs.org/en/download/).
- Extract Bot.zip Which I Submitted
- Double Click install.bat & wait for installation complete
- Double Click Start.bat
  - A chrome window will appear 
  - login to the account which will be used for botting
  - collect the weblinks and channel links
  - close chrome browser
  -  edit config.json and modify source,scrape,forward field with collected weblink and channel links
- Again Double Click Start.bat to Run The Bot
- If Everything Done Correctly You can Observe Bot in Action

[Note: The Account Which will be Used for Botting Must Join Both Group/Channels From Which You will Scrape and To Which You will Forward]


# Hosting in Cloud
* Signup For AWS Account [Free-Tier](https://aws.amazon.com/free/) to Get 1 year free VM
* Follow This [Video](https://www.youtube.com/watch?v=Q76IP7fHWCI) Instruction to Spinup a Windows EC2 Instance
* Now Follow Above Installation to Install and Run the Bot

# FAQ
- Q. Where To Get Web Links?
- A. Make Sure The Account You want to Use For Botting is Joined to Both Source and Target Group
, Now Login to Telegram Web and Go The Groups and Copy the Links From Chrome Address Bar
