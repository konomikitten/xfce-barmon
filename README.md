# xfce-barmon

## Description

A system information display for Xfce panel.

## Setup

When you first launch xfce-barmon via genmon it will complain that 
`xfce-barmon.template` is missing, this is normal. Either create your own 
template or smylink one the existing templates provided. The templates uses 
[Pango Markup](https://developer.gnome.org/pango/stable/pango-Markup.html). 
Whitespace at the start and end of all lines is removed and then the new 
lines themselves are removed when reading the template. You can use 
`${new_line}` as a place holder for where you want new lines to appear.

## Template Variables
 * `${new_line}`
 * `${tooltip}`
 * `${cpu_usage}`
 * `${cpu_temperature}`
 * `${cpu_frequency_current}`
 * `${memory_used_percentage}`
 * `${memory_used_size}`
 * `${memory_used_size_suffix}`
 * `${gpu_usage}`
 * `${gpu_fan_speed}`
 * `${gpu_temperature}`
 * `${gpu_memory_used_percentage}`
 * `${gpu_memory_used_size}`
 * `${gpu_memory_used_size_suffix}`
 * `${gpu_memory_total_size}`
 * `${gpu_memory_total_size_suffix}`
 * `${swap_used_percentage}`
 * `${swap_used_size}`
 * `${swap_used_size_suffix}`
 * `${net_received_size}`
 * `${net_received_size_suffix}`
 * `${net_sent_size}`
 * `${net_sent_size_suffix}`

## Dependancies

`Genmon` [Debian](https://packages.debian.org/bullseye/xfce4-genmon-plugin) [Xfce](https://goodies.xfce.org/projects/panel-plugins/xfce4-genmon-plugin)

`python3-pynvml` [Debian](https://packages.debian.org/bullseye/python3-pynvml) [PyPi](https://pypi.org/project/nvidia-ml-py3/)

## ScreenShots

![xfce-barmon](/screenshots/xfce-barmon.png?raw=true)

![Configuration](/screenshots/configuration.png?raw=true)

