

# Font face 
The @font-face CSS at-rule specifies a custom font with which to display text;
the font can be loaded from either a remote server or a locally-installed font
on the user's own computer.



1. - Use font-fact to load font

```css
@font-face {
  font-family: 'YourFontName';  // Replace with your desired font name
  src: url('./fonts/your-font-file.woff2') format('woff2'),  // Replace with your actual font file path
       url('./fonts/your-font-file.woff') format('woff');  // Add additional lines if you have more file formats
  font-weight: normal;
  font-style: normal;
}
```

2. - Apply style
```css
body {
  font-family: 'YourFontName', sans-serif;  // Use the font family you defined
}
```

# Font MIME Types


| Font Type                   | MIME Type   |
|-----------------------------|-------------|
| TrueType                    | font/ttf    |
| OpenType                    | font/otf    |
| Web Open Font Format        | font/woff   |
| Web Open Font Format 2      | font/woff2  |
