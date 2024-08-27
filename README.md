# myshell_tagging_platform

# Requirement
- The bot has an interactive button that allows users to input article URLs.
- Tags can be added to the bot via LLM.
- The tags and corresponding URLs are saved in the context.
- Based on tags and related content, users can search for corresponding article URLs.
# analysis
1. Based on the user's URL, hand it over to LLM for analysis of the content and output tags.
2. Based on the previously saved context, let LLM generate existing results based on user searches.
# Flowchart

![image](https://github.com/user-attachments/assets/be0323de-f9bf-48a7-b2af-36fe4e02fd12)

The final proconfig is: [link](total_pro_config.json)

Experience link
https://app.myshell.ai/bot/NFJB3y/1724669564

# JsonLink
The following are two core components, each of which can be independently deployed for testing and debugging based on existing JSON.
1. Upload Url 
upload Url Component [link](upload_url_pro_config.json)
   Based on user input URL, output JSON, the content of JSON includes the URL and tags analyzed by LLM.


2. Search By Tag Component 
search Url Component [link](search_url_pro_config.json)
   Based on the JSON list output by the previous component, let LLM perform tag and related content search based on this.
