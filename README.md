# mcp-gradio-ads-b-example
Example showing how to use MCP (Model Context Protocol) with ADS-B (plane location) data. This project is a demo of MCP capabilities. MCP has made waves in the data science community lately with the rise of agentic LLMs. Recently, [Gradio announced](https://www.gradio.app/guides/building-mcp-server-with-gradio) that they would support MCP natively in their applications. This one-line change is a game changer for developers exploring this capability. 

![demo](/mcp-demo-no-audio.gif)

## Setup
There is some setup to make sure everything goes smoothly. 

### Clone the repo
```
git clone https://github.com/WaughB/mcp-gradio-ads-b-example.git
cd mcp-gradio-ads-b-example
```


### Virtual environment
```
python -m venv venv
# Activate it:
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

### Install required packages
```
pip install -r requirements.txt
```

### API keys
This project does depend on ADS-B data coming in from RapidAPI. I won't show how to get the keys, but I will provide a link to the vendor: https://rapidapi.com/adsbx/api/adsbexchange-com1 . 


### Downloading & updating Claude Desktop
Please install Claude Desktop before attempting this project. You do not need to use the paid for version, I was able to create this project with the free-tier version. I used these guides [1](https://www.gradio.app/guides/building-mcp-server-with-gradio), [2](https://www.gradio.app/guides/using-docs-mcp) from Gradio to change the config files. The first one was more similar to my application, but the config file on the second link worked better for me. 


## Credits
Could not have done this without the contributions by the [ADS-B Exchange Community](https://www.adsbexchange.com/). I accesses the data through the [RapidAPI](https://rapidapi.com/adsbx/api/adsbexchange-com1).

[Claude Desktop](https://claude.ai/download) was something I hadn't previously used. This was a very refreshing way to interact with LLMs. It does make me wonder why other companies haven't made something similar yet... 