## Submission System

One of the decisions you will make (if the Sorrento Meeting has a call for abstracts) is which submission system to use.

This system is used for managing abstract submissions and reviewer allocation.

There is no perfect submission system — they each have strong points and weak points. It is worth speaking to colleagues who have recently organised a meeting to check their experience.

Some common systems are

* [Microsoft CMT3](https://cmt3.research.microsoft.com/About)
* [Open Review](https://openreview.net/about)
* [EasyChair](https://easychair.org/)



Once you have made your choice, you will need to request a URL for your submissions. Once you have that URL you can edit the following fields in the [`_config.yml`](_config.yml) file:

```
conference:
  submission:
    # Whether to show the submission site.
    show: 
    # The URL of the submission site.
    url: 
    # The name of the submission site (e.g. Microsoft CMT Website)
    name: 
```

That will auto generate some text on the `submission.html` page. You can fill in details around submission on that page and it will appear below. 
