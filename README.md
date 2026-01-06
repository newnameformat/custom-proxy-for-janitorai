Updated 12.24.2025 | Created 04.06.2025

![Badge](https://hitscounter.dev/api/hit?url=https%3A%2F%2Fgithub.com%2Fnewnameformat%2Fcustom-proxy-for-janitorai&label=Readers&icon=person-check-fill&color=%230d6efd&message=&style=flat&tz=UTC)

## Simple Guide (Bookmark this Site)
To view the simple and easy-to-follow guide, along with tips for generation settings, you can [visit this link](https://custom-proxy-for-janitorai.vercel.app/) and feel free to open an issue or reach out via Discord @ newnameformatsucks for additonal assistance! Otherwise, refer to the steps below. 

## Step-by-Step Guide
1. Type openrouter.ai in your browser or click here and register for an account.
2. Click on settings (upper right corner) THEN scroll down to Default Model and select TNG: DeepSeek R1T2 Chimera (free) or your preferred model.
3. Click the Privacy tab (left menu) and enable Model Training. If you do not enable this, you will be thrown an error when generating a response.
4. Open a new tab and click on the API Keys tab (left menu) and create a new API key. SAVE the key because once you copy it, you will not be able to see it again.
  4.1 If you lose your key, you can always create a new one.
5. Return to Janitor.ai and find a proxy compatible bot.
  5.1 Proxy compatible bots will show "proxy allowed" text above the persona selector/start chat feature. Compatible bots usually have visible character definitions.
6. After choosing a bot, open the API Settings from the menu (top right corner) and choose Proxy.
7. Under the Proxy Model settings, choose 'Add Configuration' and choose your Config Name (anything you want it to be).
  7.1 You can create multiple configurations which is great for experimenting without changing your current configuration.
8. Under 'Model Name' paste tngtech/deepseek-r1t2-chimera:free in the box (MUST be all lowercase).
  8.1 When you determine the model you want to use, there is a clipboard icon you can press to copy your model name.
  8.2 For example, mistralai/mistral-medium-3.1 would be the model name for Mistral: Mistral Medium 3.1
9. Under Other API/Proxy URL type/paste this EXACT link: https://openrouter.ai/api/v1/chat/completions
  9.1 This WILL NOT change regardless of the model you use. Only if you use a different API provider.
10. Finally, under API Key, paste the API key you generated and saved in step 4; Otherwise create and paste a NEW API key.
    10.1 Note that while API Keys are listed as 'OPTIONAL,' failure to provide an API key will only throw you errors.
11. If you do not have any custom prompts you would like to add, click Save Settings. When/if the pop up asks if you would like to set generation settings to openai's default, click yes.
12. Open Generation Settings from the in chat menu (top right corner) and set your temperature and tokens to your preference.
13. Close all Janitor.ai tabs and reopen them (or simply refresh). Now you can start chatting!
