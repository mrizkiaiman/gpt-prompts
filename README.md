## Guide

1. First, go to the website https://chatbot.mrizkiaiman.com in your preferred browser.
2. Create a prompt by clicking on the **New Prompt** button present on the home screen.
3. Open your browser's **DevTools** by right-clicking on the page and select **Inspect** or by using the `Ctrl+Shift+I` keyboard shortcut.
4. In DevTools, switch to the **Console** tab.
5. Then, type the below command but make sure to change the data in the `obj` variable with the data from `index.json`. Copy-paste the data in the `obj` variable.

  ```js
    const obj = [
      {
        "id": "db7c1fb0-ad3e-42f7-9023-5f4384a22c62",
        "name": "English - Fix grammar mistakes, typos, and factual errors.",
        "description": "",
        "content": "I want you to act as my English and improver. I will write down a sentence below and you will improve it. I want you to strictly correct my grammar mistakes, typos, and factual errors.\n\n{{sentence}}",
        "model": {
          "id": "gpt-3.5-turbo",
          "name": "GPT-3.5",
          "maxLength": 12000,
          "tokenLimit": 4000
        }
      },
      ...
    ]
    
    localStorage.setItem("prompts", JSON.stringify(obj))
  ```
  
6. Finally, check the `localStorage` of your browser by refreshing the page or by typing `localStorage` in the console to make sure the new data is set.