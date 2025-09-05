# telegram_id_multi_parser
Python script for parsing Telegram IDs from public chats.

Hello, world! In this article, I’d like to add another case to the collection of so-called “privacy” in Telegram. I am not a cybersecurity specialist, but I would like to point out that during my small Data Science project, where I was practicing data parsing from public Telegram chats with open user information, I discovered the possibility of extracting the so-called Telegram ID, which is supposedly considered confidential information.

My script, written with the help of AI tools (GPT-model 5.0), Python, Telethon, Pandas, and others, makes it possible to retrieve the ID of any user in the messenger if you know their @username, as well as to export into a tabular CSV file the list of all participants of chats/channels. Along with the TG-ID, the file may also include first names, last names, and—if you are an admin of the chat/channel or if you have a link to a public chat where this information is visible to everyone—the phone numbers that users made public in their privacy settings.

It is important to note that when exporting data from chats with an open member list, the script collects unique user identifiers for absolutely all participants—even for those who do not have @usernames. If the chat/channel only displays a list of administrators, it is possible to collect information about the entire admin team.

I have no intention of spreading other people’s personal data, which is why I did not develop my script into a full-fledged application (especially since Telegram already has similar bots for retrieving a user’s unique identifier). My only goal was to demonstrate, through my own experience, the vulnerability of one of the most popular messengers. This tool, which I literally wrote in half an hour, is yet another proof that Telegram’s ecosystem is not really about privacy or confidentiality, and its level of information security is no better than that of an average social network—meaning it’s not a good idea to store personal data, trade secrets, or other sensitive information there.

Telegram ID remains constant throughout the entire lifecycle of a user account. Even if you change your @username, first name, last name, or phone number in your account settings, the unique identifier can only be changed by deleting the old account and creating a new one. If this information falls into the hands of third parties, it may be used for malicious purposes.

I would also like to remind you that several human rights projects and cybersecurity specialists have already proven the fact that Telegram shares information with Russian security services, which form the backbone of the criminal Putin regime.

You can review a demo version of the script code, as well as attached files with exported databases containing open data (except for Telegram IDs) of users from one of the public chats. To avoid personal data leaks, all unique user identifiers have been partially hidden.
