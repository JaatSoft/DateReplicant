Date v0.01 for Haiku
==

![Screenshot](DateReplicant.png)

This is a simple replicant application. It shows date info.  You may change program settings by editing "~/config/settings/Date_settings" file.  Settings file will be created automatically after first launch of "Date". Default background image is from OBOS GUI prototype (OBOS_UI_v2_2 image).

Email contact: _sl@mail.ru

Special thanks to: Sergei Dolgov, Roman Kopko, Ilya Nedoluzhko

Example settings file:

```
Background_AM "/boot/beos/documentation/graphics/belogo.jpg"
	-- path for AM image (default "")
Background_PM "" 
	-- path for PM image (default "")
FontDay "Courier10 BT" "Bold Italic" 20.1 150 50 60 0 "On"
	-- font information family, style, size, rgb color, transparent, antialiasing
FontMonth "Courier10 BT" "Bold Italic" 10.1 150 50 60 0 "On"
FontYear "Courier10 BT" "Bold Italic" 10.1 150 50 60 0 "Off"
PositionDay 14 10
	-- x, y
PositionMonth 10 35
PositionYear 30 35
DayVisible "On"
	-- visible "On"/"Off"
MonthVisible "On"
YearVisible "On"
DayString "%d"
	-- format string for strftime function (ex: "%p %a")
		%a short name of day week
		%A full name of day week
		%b short name of month
		%B full name of month
		and other
MonthString "%b"
YearString "%y"
```
