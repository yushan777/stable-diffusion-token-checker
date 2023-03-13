<table style="width:100%" text-align:center >
  <tr>
    <td>
      <a target="_blank" href="https://colab.research.google.com/github/yushan777/stable-diffusion-token-checker/blob/main/sddb_token_checker.ipynb">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
      </a>
    </td>
  </tr>

</table>

# Stable Diffusion Dreambooth Token Checker

Inspired and adapted from scripts and ideas by 2kpr

https://www.reddit.com/r/StableDiffusion/comments/zc65l4/rare_tokens_for_dreambooth_training_stable/

https://arxiv.org/pdf/2208.12242

The purpose of this notebook is to check what a given token / token+class pair might generate from the model you are planning to train on. It will also show a breakdown of how your token is tokenized.   

A 3x3 grid of images will be generated prompted with a given token from a list.  You can also include class words so that each token will be paired with the class and also added to the list.

You can add a series of token words (comma separated). 

Output will include a breakdown of your token - i.e. so that long, convoluted token you came up with might actually be broken up into subtokens, and having a very strong prior association in the model. 

## What to look for:

* If outputs show a consistent theme, then the token you are using probably has strong associations in the model. (worse)
* If outputs appear random then it will probably have weaker associations in the model. (better)
---
![token1](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/resources/Unknown-2.jpeg)
---
![token2](https://github.com/yushan777/stable-diffusion-token-checker/raw/main/resources/Unknown-3.jpeg)
