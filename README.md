#tumblr-vim-skeleton

Vim skeleton files for use with [mwunsch](http://markwunsch.com)'s [Tumblr gem](http://github.com/mwunsch/tumblr).

## Installation

Put all of the .skel files somewhere. I have them in `~/.vim/tumblr/`, but you know, whatever floats your boat.

Then map them all in your .vimrc like so:

	augroup Tumblr
		au BufNewFile *.ttext	0r ~/.vim/tumblr/text.skel
		au BufNewFile *.tphoto	0r ~/.vim/tumblr/photo.skel
		au BufNewFile *.tquote	0r ~/.vim/tumblr/quote.skel
		au BufNewFile *.tlink	0r ~/.vim/tumblr/link.skel
		au BufNewFile *.tconvo	0r ~/.vim/tumblr/convo.skel
		au BufNewFile *.tvideo	0r ~/.vim/tumblr/video.skel
		au BufNewFile *.taudio	0r ~/.vim/tumblr/audio.skel
	augroup end
	
From here on out, any time you open vim to edit a new file that matches one of the above extensions, it will pre-fill the document with all of the various parameters that you can pass to [tumblr](http://github.com/mwunsch/tumblr) when posting to [Tumblr](http://www.tumblr.com).