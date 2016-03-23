#dot-files-weechat

[roaet's](http://roaet.com) weechat configurations.

##How to install

1. Backup your current .weechat conf:

```
cp -r ~/.weechat ~/.weechat.bk
```

2. Clone this directory somewhere:

```
git clone https://github.com/roaet/dot-files-weechat
```

3. Change into that new directory:

```
cd dot-files-weechat
```

4. Run sync

```
./sync
```

5. Copy your old irc.conf back to get your connections back

```
cp ~/.weechat.bk/irc.conf ~/.weechat
```

> What did this do?
> This copied .weechat directory to your home from this repo and, if you put it
> back, restored all your connections!

##Holy mother of hot keys

I am a vim developer so I stuck to those hotkeys for a vast majority of things:

* `C-h` - select buffer to the left of this one
* `C-j` - select buffer below this one
* `C-k` - select buffer above this one
* `C-l` - select buffer to the right of this one
* `C-x` - rotate between merged buffers down
* `C-q` - rotate between merged buffers up
* `C-z` - zoom in on a buffer (press again to zoom back out)

> `this one` refers to the buffer with the cursor in it


##Workflow

I generally keep all private messages in a merged window (single window with
many buffers):

```
/buffer merge <buffer id>  # where buffer id is the integer in the left pane
```

Sometimes I cant show all the merged buffers at the same time, so I swap
between sets:

```
/b <buffer id>
```

Also there are times where the highlights just never go away and I get sick of
them. There is an alias to reset all the things:

```
/ok
```
