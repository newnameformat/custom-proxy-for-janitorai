Updated 09.28.2025 | Created 04.06.2025

![Badge](https://hitscounter.dev/api/hit?url=https%3A%2F%2Fgithub.com%2Fnewnameformat%2Fcustom-proxy-for-janitorai&label=Readers&icon=person-check-fill&color=%230d6efd&message=&style=flat&tz=UTC)

# Update Regarding Deepseek Models via OpenRouter
Many of Deepseek's models are provided by Chutes. As of recent changes, users will experience frequent 429 rate-limited upstream errors when attempting to use most Deepseek models. This is because [Chutes](https://chutes.ai/app) is prioritizing their paid tier customers (rightfully so) over Openrouter users (whether or not you have the free/paid tier through Openrouter). Currently, the [V3.1 (free)](https://openrouter.ai/deepseek/deepseek-chat-v3.1:free) model is the only Deepseek model that is mostly uneffected at this time and is a great model overall. Occasionally you may need to refresh or wait a minute before sending another prompt. My suggestion would be to use the V3.1 (free) Deepseek model (or any other LLM, it does NOT have to be Deepseek) unless you would rather subscribe to Chutes / get directly setup with [Deepseek](https://api-docs.deepseek.com/). Just remember that if you have charged the 10$ in credits to your Openrouter account, it is not WASTED money! You still get 1000 requests per day (which is a lot for Janitor) and you still have access to so many LLMs. So you can continue to use the 10$ to maintain your 1000 requests or you can go ahead and spend it on paid models (Deepseek paid models still receive 429 errors but aren't entirely disruptive). To those of you who are unfamiliar with Openrouter, the 10$ in credits is NOT required! You can still use the free models. I will also be updating the following steps to reflect V3.1 as our example model.

## Using Deepseek (& Other Models) on Janitor 
Please note that as of this day, 09.28.2025, this is a current and up-to-date guide. I do not anticipate any changes that could potentionally alter the required steps and/or render this guide inaccurate or irrelevant. I will keep this guide as up-to-date as possible. This guide will give you step by step instructions on how to use Deepseek-V3.1 on [Janitor.ai](https://janitorai.com/) (our example model) and will work with any model offered by [openrouter.ai](https://openrouter.ai/) platform. Refer to the steps below to get started. 

## Step by Step Guide

1. Type openrouter.ai in your browser or [click here](https://openrouter.ai/) and register for an account. 

2. Click on settings (upper right corner) THEN scroll down to Default Model and select Deepseek V3.1 (free) or your preferred model.

3. Click the Privacy tab (left menu) and enable Model Training. If you do not enable this, you will be thrown an error when generating a response. 

4. Open a new tab and click on the API Keys tab (left menu) and create a new API key. SAVE the key because once you copy it, you will not be able to see it again.

   4.1 If you lose your key, you can always create a new one. 


5. Return to [Janitor.ai](https://janitorai.com/) and find a proxy compatible bot. 

   5.1 Proxy compatible bots will usually have 'Proxy ✅' if they are compatible or 'Proxy ❌' is they are not. You will find this indicator 
        above your persona selector and the "start chat" feature. Compaitble bots usually have visible character definitions. 

6. After choosing a bot, open the API Settings from the menu (top right corner) and choose Proxy.

7. Under the Proxy Model settings, choose 'Add Configuration' and choose your Config Name (anything you want it to be).
   
8. Under 'Model Name' paste deepseek/deepseek-chat-v3.1:free in the box (MUST be all lowercase).

    8.1 When you determine the model you want to use, there is a clipboard icon you can press to copy your model name.

    8.2 For example, mistralai/mistral-medium-3.1 would be the model name for Mistral: Mistral Medium 3.1

9. Under Other API/Proxy URL type/paste this **EXACT** link https://openrouter.ai/api/v1/chat/completions

    9.1 This WILL NOT change regardless of the model you use. Only if you use a different API provider. 

10. Finally, under API Key, paste the API key you generated and saved in step 4; Otherwise create and paste a NEW API key.

    10.1 Note that while API Keys are listed as 'OPTIONAL,' failure to provide an API key will only throw you errors. 

11. If you do not have any custom prompts you would like to add, click Save Settings. When/if the pop up asks if you 
    would like to set generation settings to openai's default, click yes. 

12. Open Generation Settings from the in chat menu (top right corner) and set your temperature and tokens to your preference. 

13. Close all Janitor.ai tabs and reopen them (or simply refresh). Now you can start chatting!


<br>
<br>

## Making Changes/Adjustments
Please note that whenever you make changes to your prompts, temperature/tokens/context and/or models, as briefly touched up on below, you will be required to REFRESH the page OR close and reopen the chat. This is because the LLM needs to register these changes in order to execute them and if not refreshed, your requests will get hung up and you will recieve errors. 


<br>

## Model Note 
Openrouter.ai supports dozens of other models so you are not limited to deepseek. You can follow these exact steps to use other models of your choice. You do not need a new API key, you just need to change the path in step 7 to the model's respective path which can be copied directly from the models page. For example, if you would like to use [xAI: Grok 3 Beta](https://openrouter.ai/x-ai/grok-3-beta), you would select the clipboard icon under its name to copy the path ( x-ai/grok-3-beta ) and paste it into the custom field.



<br>

## Temperature, Token & Context Note
NOTE: With the changes made to Janitor's chat settings, I have noticed that I have not had to reset my generation settings. HOWEVER, I do recommend checking before you start chatting and read the following:

Different models will yield different results, you may prefer certain models to others in their ability to produce responses that appeal to your style and liking while also delivering an amazing roleplay experience. Janitor.ai is known for its NSFW content, and some models will not support NSFW content without jailbreaking and custom prompts, even then, it is not guranteed you will receive a decent response. Qwen and Deepseek are decent NSFW models from personal experience. You may also need to adjust the temperature, token and context sliders to receive better responses. I normally set tokens at 0 for deepseek and preferred 1000 (max) when using qwen. So please remember to adjust these settings when trying different models. Each time you change your model, you will be reverted to JLLM's default settings which is a temperature of 1.1 and tokens are 260. You can use the default settings with your new model, but I recommend starting out with a temperature of at least 0.9 and go from there. These settings are accessed in chat under Generation Settings!
