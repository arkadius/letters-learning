# letters-learning
Simple bash script for purpose of learning of letters and vocabulary using speech synthesizer

## Usage

Just run script and start typing words. It pronounce each letter. After pressing space it also pronounce typed word. You can repeat words pressing space again.

```
./letters-learning
```

## Limitation

It currently using polish speech synthesizer http://milena.polip.com . If you want to use it, you need to install it. Installation instruction is available on project's site.

If you want to use other speech synthesizer just change 4th line of script.

If you will see this error while using milena for some letters:
```
play WARN alsa: under-run
```
You can fix it chaning tempo. Just create file `~/.milena_bookrc` with this content:
```
tempo=1.4
pitch=0.8
```
