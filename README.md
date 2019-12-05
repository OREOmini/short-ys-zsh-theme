# short-ys-zsh-theme
Short-ys is a [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) theme，based on [ys.zsh-theme](https://github.com/robbyrussell/oh-my-zsh/blob/master/themes/ys.zsh-theme).

With short-ys, you can:

* Get rid of `user @ machine` in the prompt

* Show an emoji of "🥑" instead. Or any other emojis you like if modify the code

  ```bash
  user_prompt_info() {
  	# if username is not the default name (which can be set in .zshrc)
  	if [[ "$USER" != "$DEFAULT_USER" || -n "$SSH_CLIENT" ]]; then
  		echo -n "$DEFAULT_USER_PROMPT"
  	else
  		# customization
  		echo "🥑 "
    	fi
  }
  ```


## Preview

![Screenshot](/Users/wangyunwen/Desktop/short-ys-zsh-theme/Screenshot.png)







## Usage

Just clone this repository into your `~/.oh-my-zsh/themes` directory.

```
git clone https://github.com/OREOmini/short-ys-zsh-theme.git ~/.oh-my-zsh/themes/short-ys
```

And then select this theme in your `~/.zshrc`

```
ZSH_THEME="short-ys/short-ys"
```



Set your `DEFAULT_USER` in `~/.zshrc` as well, you can use `whoami` to find your username:

```
DEFAULT_USER="your_user_name"
```

