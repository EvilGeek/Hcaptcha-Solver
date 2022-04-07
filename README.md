# Hcaptcha-Solver
artificial intelligence to solve hcaptcha

`Currently, hcaptcha has added some additional topics, so this code is not available on some sites or in certain cases - Patching`


# Key Features
- Fast and accurate AI (Learned with more than 30,000 images in total)
- Proxy support (http)


# Quick Example
```py
import hsolver, requests

s = requests.session()
# s.proxies.update({"http": "proxy", "https": "proxy"}) # If you want to generate many correct answer tokens due to request restrictions, we recommend using a proxy.

print(hsolver.HcaptchaSolver(s).solve("site key", "url"))  # Ex. '4c672d35-0701-42b2-88c3-78380b0db560', 'discord.com'
```
