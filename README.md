# smooth-dim
Smoothly decreases the brightness using brightnessctl
### Dependencies
* Brightnessctl
## Usage
```
$ bash smoothDim [bright/dim] [number to stop dimming (optional)]
```
Edit the speed of the dimming by edting the sleep and brightnessctl values in the script
### Using hypridle
```
listener {
    timeout = 250                             
    on-timeout = bash ~/light.sh dim      
    on-resume = pkill -f ~/light.sh  || bash ~/light.sh bright                
}
```
