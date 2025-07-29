You will find the English ReadMe at the end of the document.

## Grove RGB-LCD Display (mit I2C), Version 4.0

Das Grove RGB-LCD Display ist ein 16x2-Zeichen-Display mit hintergrundbeleuchtetem RGB-LED-Modul, das sich über I²C ansprechen lässt.
Die Besonderheit: Die Hintergrundbeleuchtung lässt sich per Software in Rot, Grün und Blau mischen – so sind beliebige Farben möglich.

Es eignet sich ideal für Projekte, bei denen einfache Texte angezeigt werden sollen (z. B. Statusanzeigen, Sensorwerte, einfache Menüsysteme)


[ Grove RGB LCD Wiki](http://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/)

## MakeCode Erweiterung

Text anzeigen mit automatischem Scrollen

```
//% block="write | %str | to | row | %row | with speed | %speed | ms"
```

Farbe der Hintergrundbeleuchtung setzen

Setze nur Rot
```
//% block="set red to | %r"
```

Setze nur Grün
```
//% block="set green to | %g"
```

Setze nur Blau
```
//% block="set blue to | %b"
```

Setze alle drei Farben gleichzeitig (RGB)
```
//% block="set RGB to | red |  %r | green |  %g | blue |  %b"
```

# Beschreibung:

Diese Blöcke steuern die Hintergrundfarbe des Displays. Die Werte r, g, b können von 0 bis 255 eingestellt werden.
So lassen sich z. B. Farben wie Weiß (255,255,255), Blau (0,0,255) oder Grün (0,255,0) erzeugen.


# Beispielnutzung in MakeCode (JavaScript)

```
rgblcd.setRGB(100, 100, 255); // Lila Hintergrundfarbe
rgblcd.writeString("Hallo Calliope!", 0, 200); // Zeile 0, Scrollgeschwindigkeit 200ms
rgblcd.writeString("Sensorwert: 23°C", 1, 0);  // Zeile 1, kein Scrollen
```




## Grove RGB-LCD Display (with I2C), Version 4.0

The Grove RGB-LCD Display is a 16x2 character display with an RGB LED backlight module that communicates via I²C.
What makes it special: the backlight color can be mixed in software using red, green, and blue components – allowing for virtually any color.

It’s ideal for projects that require simple text output, such as status displays, sensor readings, or basic menu systems.


[ Grove RGB LCD Wiki](http://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/)


## MakeCode Extension

# Display text with automatic scrolling
```
//% block="write | %str | to | row | %row | with speed | %speed | ms"
```

Set backlight color

Set red only
```
//% block="set red to | %r"
```

Set green only
```
//% block="set green to | %g"
```

Set blue only
```
//% block="set blue to | %b"
```

Set all three colors at once (RGB)
```
//% block="set RGB to | red |  %r | green |  %g | blue |  %b"
```

## Description:

These blocks control the display’s backlight color. The values for r, g, and b can range from 0 to 255.
This allows you to create colors like white (255, 255, 255), blue (0, 0, 255), or green (0, 255, 0).

## Example usage in MakeCode (JavaScript)
```
rgblcd.setRGB(100, 100, 255); // Purple backlight
rgblcd.writeString("Hello Calliope!", 0, 200); // Line 0, scroll speed 200ms
rgblcd.writeString("Sensor value: 23°C", 1, 0);  // Line 1, no scrolling
```

## Supported target

* for PXT/calliope

## License

MIT
