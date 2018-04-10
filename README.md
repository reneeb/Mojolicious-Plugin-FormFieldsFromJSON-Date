# Mojolicious::Plugin::FormFieldsFromJSON::Date

[Mojolicious::Plugin::FormFieldsFromJSON::Date](Mojolicious::Plugin::FormFieldsFromJSON::Dat://metacpan.org/pod/Mojolicious::Plugin::FormFieldsFromJSON::Date)
is an extension to the [Mojolicious](https://metacpan.org/pod/Mojolicious)
plugin
[Mojolicious::Plugin::FormFieldsFromJSON](https://metacpan.org/pod/Mojolicious::Plugin::FormFieldsFromJSON)
for the creation of date fields.

## Usage

```
# Mojolicious
$self->plugin('FormFieldsFromJSON::Date');
$self->plugin('FormFieldsFromJSON' => {
  types => {
    date => 1,
  },
});

# Mojolicious::Lite
plugin 'FormFieldsFromJSON::Date';
plugin 'FormFieldsFromJSON' => {
  types => {
    date => 1,
  },
};
```

## Installation

The simplest way to install the module is via `cpanm`:

```
$ cpanm Mojolicious::Plugin::FormFieldsFromJSON::Date
```

Alternatively, you could download the distribution tarball and install it
in the traditional manner by using `make`:

```
$ tar -xvzf Mojolicious-Plugin-FormFieldsFromJSON-Date-<version>.tar.gz
$ cd Mojolicious-Plugin-FormFieldsFromJSON-Date-<version>
$ perl Makefile.PL
$ make
$ make test
$ make install
```

## Development

The distribution is contained in a Git repository, so simply clone the
repository

```
$ git clone git@github.com:reneeb/Mojolicious-Plugin-FormFieldsFromJSON-Date.git
```

and change into the newly-created directory.

```
$ cd Mojolicious-Plugin-FormFieldsFromJSON-Date
```

The project uses [`Dist::Zilla`](https://metacpan.org/pod/Dist::Zilla) to
build the distribution, hence this will need to be installed before
continuing:

```
$ cpanm Dist::Zilla
```

To install the required prequisite packages, run the following set of
commands:

```
$ dzil authordeps --missing | cpanm
$ dzil listdeps --author --missing | cpanm
```

The distribution can be tested like so:

```
$ dzil test
```

To run the full set of tests (including author and release-process tests),
add the `--author` and `--release` options:

```
$ dzil test --author --release
```
