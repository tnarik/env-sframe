# About this environment

This environment includes **GraphLab Create** and **SFrame** to support the [Coursera Machine Learging specialization](https://www.coursera.org/specializations/machine-learning) which I am tracking as the `course-coursera-Washington_machine_learning` repository.

## The course

The course notebooks, code and documentation is tracked in its own repository. To simplify reusability (and because of the way Direnv works, which doesn't sit well with Dropbox and sharing the environment across multiple computers with different versions of macOS), the course is shared, the environment is not (it is synchronized via GIT).

The course folder is linked as `course`. This is a recommendation, obviously, and you can do as you please.

## Direnv

When using `direnv`, the virtualenv environment is setup and activated upon accessing the directory.

`pip install -r requirements.txt`

Additionally, you'll need to install the requirements (see below about **GraphLab Create**)

## GraphLab Create

The `requirements.txt` file can be modified to include an entry for the URL, but because the URL includes the e-mail address and the product key, that is not recommended for shared repositories. Installation can take place manually via the following `pip` command (replacing the e-mail address and product key tokens):

```
pip install --upgrade --no-cache-dir https://get.graphlab.com/GraphLab-Create/2.1/<registered email address>/<product key>/GraphLab-Create-License.tar.gz
```

Please note the package is currently only supported in Python 2.7.x. You might need an up to date version due to issue like TLS context (for the installation it required 2.7.12 as of 2016-12-11).