# Mailhide2

A replacement of Google's [Mailhide](https://www.google.com/recaptcha/mailhide/d) (deprecated due to the shutdown of reCAPTCHA v1) using [reCAPTCHA](https://developers.google.com/recaptcha/intro) v2. 


## Usage

1. [Sign up](http://www.google.com/recaptcha/admin) for your own reCAPTCHA key from Google. Both regular and invisible keys are supported.
2. Replace `<site_key>` in `email.html` (`email_invisible.html` for invisible reCAPTCHA) and `<secret_key>` and `<email>` in `email.php` with your own.
3. Put `email.html` and `email.php` under the same directory on your website.
4. Include a link to `email.html` in the web page where your masked email address is shown. If an element with id `mailhide` exists, its contents will be replaced by a link to the revealed email address. See `index.html` for an example.


## Notes

The code uses `www.recaptcha.net` instead of `www.google.com` to enable access from places where Google is blocked. See the [FAQ](https://developers.google.com/recaptcha/docs/faq#can-i-use-recaptcha-globally) of reCAPTCHA for details on global access. 


## Acknowledgments

The code was inspired by this [example](https://codeforgeek.com/2014/12/google-recaptcha-tutorial/) on Codeforgeek.  