# Using Deepseek on Janitor 
Please note that as of the creation date of this repository, 04.06.2025, this is a current and up-to-date guide. I do not anticipate any changes that could potentionally alter the required steps and/or render this guide inaccurate or irrelevant. I will keep this guide as up-to-date as possible. This guide will give you step by step instructions on how to use Deepseek-r1 on [Janitor.ai](https://janitorai.com/) but will work with any model offered by [openrouter.ai](https://openrouter.ai/) platform. Refer to the steps below to get started. 

## Step by Step Guide

1. Type openrouter.ai in your browser or [click here](https://openrouter.ai/) and register for an account. 

2. Click on settings (upper right corner) THEN scroll down to Default Model and select Deepseek R1 Zero (free).

3. Click the Privacy tab (left menu) and enable Model Training. If you do not enable this, you will be thrown an error when generating a response. 

4. Click on the API Keys tab (left menu) and create a new API key. SAVE the key because once you copy it, you will not be able to see it again.
   4.1 If you lose your key, you can always create a new one. 

6. Return to [Janitor.ai](https://janitorai.com/) and find a proxy compatible bot. 
   5.1 Proxy compatible bots will usually have 'Proxy ✅' if they are compatible or 'Proxy ❌' is they are not. You will find this indicator 
        above your persona selector and the "start chat" feature. Compaitble bots also have visible character definitions. 

7. After choosing a bot, open the API Settings from the menu (top right corner) and choose Proxy.

8. Under the Proxy Model settings, choose 'custom' and type deepseek/deepseek-r1:free in the box (MUST be all lowercase).  

9. Under Other API/proxy URL type/paste this **EXACT** link https://openrouter.ai/api/v1/chat/completions

10. Finally, under API Key, paste the API key you generated and saved in step 4 otherwise create and paste a NEW API key. 

11. If you do not have any custom prompts you would like to add, click Save Settings. When the pop up asks if you 
    would like to set generation settings to openai's default, click yes. 

12. Open Generation Settings from the in chat menu (top right corner) and set your temperature and tokens to your preference. 

13. Close all Janitor.ai tabs and reopen them (or simply refresh). Now you can start chatting!


## Model Note 
Openrouter.ai supports dozens of other models so you are not limited to deepseek. You can follow these exact steps to use other models of your choice. You do not need a new API key, you just need to change the path in step 7 to the model's respective path which can be copied directly from the models page. For example, if you would like to use [xAI: Grok 3 Beta](https://openrouter.ai/x-ai/grok-3-beta), you would select the clipboard icon under its name to copy the path ( x-ai/grok-3-beta ) and paste it into the custom field.

## TEMPERATURE/TOKEN/CONTEXT NOTE
Different models will yield different results, you may prefer certain models to others in their ability to produce responses that appeal to your style and liking while also delivering an amazing roleplay experience. Janitor.ai is known for its NSFW content, and some models will not support NSFW content without jailbreaking and custom prompts, even then, it is not guranteed you will receive a decent response. Qwen and Deepseek are decent NSFW models from personal experience. You may also need to adjust the temperature, token and context sliders to receive better responses. I normally set tokens at 0 for deepseek and preferred 1000 (max) when using qwen. So please remember to adjust these settings when trying different models. Each time you change your model, you will be reverted to JLLM's default settings which is a temperature of 1.1 and tokens are 260. You can use the default settings with your new model, but I recommend starting out with a temperature of at least 0.9 and go from there. These settings are accessed in chat under Generation Settings!
