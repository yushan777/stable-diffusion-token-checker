
<table style="width:100%">
  <tr>
    <td>
      <a target="_blank" href="https://colab.research.google.com/github/yushan777/stable-diffusion-token-checker/blob/main/sddb_token_checker.ipynb">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" width="250"/>
      </a>
    </td>
    <td>
      Join The <a href="https://discord.gg/wNNs2JNF7G">Stable Diffusion Dreambooth Discord Server</a>
    </td>
  </tr>
</table>



# Stable Diffusion Dreambooth Token Checker

Adapted from scripts and ideas by 2kpr

https://www.reddit.com/r/StableDiffusion/comments/zc65l4/rare_tokens_for_dreambooth_training_stable/

https://arxiv.org/pdf/2208.12242

Purpose: to check what a given token / token+class pair might generate from the model you are planning to train on. It will also show a breakdown of how your token is tokenized into subwords. So that long, convoluted token you came up with might actually be broken up into subtokens which are very common words themselves and so having a very strong prior association in the model.

There is no rule to say you can't just use someone's regular name. You can use `tomcruise` if you want but you'll just end up pulling weights associated with him to the subject you are training and erasing old tomcruise from the model's memory. 

A 3x3 grid of images will be generated from prompts using token(s) you specify.  You can also include class words so that each token will be paired with the selected class(es) which will also be added to the list.

## What to look for:

* If outputs show a consistent theme, then the token you are using probably already has strong associations in the model. (not ideal)
* If outputs appear random then it will probably have weaker associations in the model. (better)

## Just 4 Main Cells to run.  Only 3 and 4 require any user input. 
![cells](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/cells.jpg)

---
## Some Example Outputs
![supercalifragilisticexpialidocious](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/supercalifragilisticexpialidocious.jpg)
---
![sks](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/sks.jpg)
---
![sks-woman](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/sks-woman.jpg)
---
![sks-artstyle](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/sks-artstyle.jpg)
---
![http](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/http.jpg)
---
![http-person](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/http-person.jpg)
---
![rune](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/rune.jpg)
---
![rune-person](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/images/rune-person.jpg)
