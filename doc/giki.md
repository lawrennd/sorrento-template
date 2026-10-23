# The Giki Philosophy

The Giki Philosophy is an approach to making it easier to decentralise the work of the maintaining the website, even allowing conference
attendees to fix errors they find in your site, whilst maintaining central control.

The trick is to make it convenient for people to edit your pages directly in github's on line editor, and provide you with a pull request.

This is relatively simply done through a set of 'edit' links that appear on relevant pages. Just below the initial title on each page you will find an [edit] link. This leads directly to the relevant source file on GitHub, opening the edit page. If a user is not logged into their GitHub account, they will be asked to do so. Editing automatically forks the repo into their GitHub account, and they can then submit a pull request to request updates.

The giki philosophy uses this convenience to share the workload of correcting errors and maintaining the site. If you encourage attendees to make use of the giki links then you can significantly reduce the maintenance load. You may also find the giki links helpful yourself for making minor fixes to errors that you spot. Such fixes can even be made from mobile phones or tablets.

Edit links use `ghub.branch` from `_config.yml`. New year repos should set this to `main`. Workshop organisers who prefer a form can use the [Decap admin](./decap.md) instead.
