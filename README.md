# Jailbreaking Censored/Aligned LLMs

## Jailbreaking Aligned LLMs with ArtPrompt:

![Image-1792x1024](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/47d918b6-326b-4ed0-923e-572d9057cd5c)

> :warning: On February 22, 2024 a research paper was released on ASCII Art based Jailbreak attaches agains aligned (aka censored) LLMs. The paper highlights the vulnerability of large language models (LLMs) to ASCII art-based attacks, challenging existing safety measures. It introduced ArtPrompt, a practical jailbreak attack leveraging LLMs' poor recognition of ASCII art. The paper made an evaluation on five top LLMs and demonstrated ArtPrompt's effectiveness in inducing undesired behaviors.

## Lets do this!!

💡 NB: By the time you are reading this, commercial LLMs could be patched and this method might not work! So we thought it might be fun for you to try out this technique. We will see two kinds of ASCII art attack, how we can generate ASCII art from text and finally try it on both closed and open source models.

> :warning: Remember, this is for educational purpose only and we trust you to use it responsibly.

### Method 1

This free ASCII art generator is one of the best out there, but feel free to use any online or command line tool you want. For example [PyFiglet](https://pypi.org/project/pyfiglet) and [FigLet](http://www.figlet.org)

*Description:* Spice up your robots.txt file with creative ASCII art using our generator tool. Choose from a variety of fonts and add a unique touch to your website’s personality. [ASCII art generator](https://seotoolbelt.co/tools/ascii-art-generator)  


![image-16](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/cb97ac04-db2e-4790-bde3-e87713515472)

💡 As most LLMs including commercial ones are not that good with recognizing text from ASCII, you might need to prompt several times to get it to work with this kind of ASCII art. However, the higher the model, the higher the chance of getting it to work.

### Example prompt with this kind of ASCII art.

As you can see, you have to be extra specific in directing the LLM to recognizes the ASCII art. The below is an example from the paper.

![image-17](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/e2d92f69-bac5-440f-b7fc-5e2ff06f41ef)

Page 15 of [the paper](https://arxiv.org/pdf/2402.11753.pdf)

### Method 2

This method is quite simple. You only need to follow the below format in preparing your prompt. Note the way the characters are separated with |

![image-18](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/4c441eea-e451-41e4-9d58-0b0cedbf24df)
[ChatGPT](https://example.com)  

**This technique is credited to [Daedalus](https://x.com/daedalus_here/status/1763821384394830240?s=20)**

#### Example on Open Source Models

Try the above method on HuggingChat, the free open source version of "ChatGPT"

*Description:* Making the community’s best AI chat models available to everyone. [HuggingChat](https://huggingface.co/chat) 

*Example:*  

![image-22](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/b7fe198c-57e4-451d-b073-fee1013f60d3)
- **Mistral 7B : With Direct Prompt**  

![image-20](https://github.com/mejbass/Jailbreaking-Censored-Aligned-LLMs/assets/130122304/954fa76f-3b5c-4952-ac0e-9dd5e4c350b2)
- **Mistral 7B on Hugging Chat with ASCII Art Attack**

> :warning:  Remember: Use this for educational and research purpose only!


## Questions? Feedback? Requests? Discord: Samej2023
